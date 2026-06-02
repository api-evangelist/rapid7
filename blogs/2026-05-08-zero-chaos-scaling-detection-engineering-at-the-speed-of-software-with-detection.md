---
title: 'Zero Chaos: Scaling Detection Engineering at the Speed of Software, with Detection
  As Code'
url: https://www.rapid7.com/blog/post/dr-scaling-engineering-detection-as-code
date: '2026-05-08'
author: Zachary Zeid
feed_url: https://www.rapid7.com/rss.xml
---
Every engineering team in your organization ships code through a pipeline. They branch, test, review, and deploy. If something breaks, they roll back. If someone asks "what changed?", the answer is in the commit history. This isn't heroic discipline to process; it's just how software gets built. Now think about how your detection engineering team works. Rules get written in a UI. Maybe copied and pasted from a wiki. There's no peer review; someone clicks "save," and it's live. No test cases validate the logic before deployment. No rollback if something breaks. When an alert suddenly floods your SOC, good luck figuring out what changed and when. When a detection stops firing, you might not notice for weeks. This is, by definition, a process gap . And it's one that the rest of engineering solved years ago. The gap becomes manageable through the five custom rules, listed below. As your detections grow, you need the same discipline that every other engineering team already has. Process Stage How it works in software engineering How it works in detection engineering Storage Git / Version Control UI / Wiki / "Tribal Knowledge" Validation Automated CI/CD Tests "Wait and see if it fires" Review Peer-reviewed Pull Requests Single-user "Save" button Rollback One-click git revert Manual query deletion How does this help my security team? Detection as Code gives your team a structured, repeatable way to build and manage detections with confidence. Instead of relying on manual updates and guesswork, every change is tested, reviewed, and tracked before it reaches production. Before we get into the how , here's why Detection as Code changes the way your team works: A more reliable process. Every change goes through version control and peer review before it goes live. When something goes wrong, you know exactly what changed, when it changed, and who approved it. Roll back in seconds if needed. A safety net of tests. Inline test cases validate detection logic before deployment. Positive tests prove it catches the threat; negative tests prove it doesn't fire on legitimate activity. Confidence in what's deployed. terraform plan previews every change before anything touches production. Terraform state is the authoritative record of your detection estate, not some spreadsheet. The result is a detection workflow your team can trust. Changes are predictable, validated, and fully traceable, so security teams don’t get caught up in troubleshooting and can focus on improving coverage and overall posture. The anatomy of a detection Here is what a detection rule looks like using Rapid7’s Terraform provider . It offers a practical view of how detection engineering teams can use Detection as Code in practice: resource "rapid7_siem_detection_rule" "encoded_powershell" {
  name        = "Encoded PowerShell Command Execution"
description = "Detects PowerShell launched with base64-encoded commands"
techniques  = ["T1059.001"]
  action   = "CREATES_ALERTS"
priority = "HIGH"
logic = {
    leql = <<-LEQL
      from(event_type = process_start_event)
      where(
        (process.exe_path = /.*\\powershell\.exe$/i
         OR process.exe_path = /.*\\pwsh\.exe$/i)
        AND process.cmd_line ICONTAINS " -e"
AND process.cmd_line ICONTAINS-ANY [
" JAB", " SUVYI", " SQBFAFgA", " aWV4I"
]
      )
    LEQL
    testcases = [
      {
        matches = true
        payload = jsonencode({
          process = {
            exe_path = "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
cmd_line = "powershell.exe -ep bypass -e JABjAGwAaQBlAG4AdAA="
}
        })
      },
      {
        matches = false
        payload = jsonencode({
          process = {
            exe_path = "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
cmd_line = "powershell.exe -File C:\\Scripts\\backup.ps1"
}
        })
      }
    ]
  }
} Why this works: Version-controlled logic: The LEQL query defines the threat logic in a text format that Git can track. MITRE ATT&CK ® untegration: The techniques field ensures your coverage map updates automatically. Inline testing: We aren't just deploying a query, but a validated unit of logic . The pipeline won't let this reach production if the logic fails to fire on the matching" payload or accidentally fires on the un-matching payload. Why Terraform? Because it's the industry standard for managing infrastructure as code. We didn't invent a proprietary CLI; we built on the tool that thousands of platform teams already run daily. If your organization uses Terraform for cloud infrastructure, your detection engineers now use the same tool, the same workflow, and the same review process. Governance happens naturally in this model. Open a pull request. Your team sees the logic, the test cases, and the expected behavior. They comment, suggest improvements, and approve. Every change is traceable in your commit history. This isn't a separate compliance exercise bolted onto your workflow. It is the workflow. Already have rules built in the UI? One command imports them all: terraform query -generate-config-out imports.tf AI-assisted detection writing The quick-start repo ships with IDE configurations for Claude Code, Cursor, VS Code Copilot, and Kiro . These configs give your AI assistant full context on the Terraform provider schema, LEQL syntax, and MITRE ATT&CK mappings. In practice: open your editor, describe a threat in plain English, such as ‘write me a detection for lateral movement via RDP from non-admin workstations,’ and get back a complete Terraform resource ready for review. The AI accelerates the engineer; it doesn't replace them. The time from "I need a detection" to "this is ready for review" drops from hours to minutes. Start building detections as code today Rapid7’s Terraform provider for Detection as Code is now available across all Incident Command and InsightIDR tiers. To get to work, use the Getting Started guide for a walkthrough as you setup, authenticate, and run your first deployment. Clone the quick-start template, run terraform plan , and see your detection estate as code. For more information on Incident Command, visit Our hub page for SIEM.
