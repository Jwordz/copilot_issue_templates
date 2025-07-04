---
name: SOP / Ticket Resolution Documentation Creation
about: Ask Copilot to create Standard Operating Procedures (SOP) or ticket resolution documentation for support and incident management
title: "[SOP]"
labels: documentation
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will edit or change no other files other than the single output file

# SOP / Ticket Resolution Documentation Creation

## Objective:
You will create step-by-step Standard Operating Procedures (SOP) or ticket resolution documentation to support efficient handling of recurring issues, incidents, or support requests.

Start by analyzing the relevant context.

## Context that you will analyze and its locations:
- **Source Materials**: I will provide all the relevent contect in the comments of this issue.
- **Existing SOPs and Knowledge Base**: Check `/docs/sop`, `/docs`, `/README.md`, and related documentation directories or hyperlinks within the comment
- **Purpose of context**: Use these materials as your base for the content to create a draft of the SOP / ticket resolution documentation.


# Your output
- Deliver the documentation as a **markdown file** saved in "/documentation" directory
- The filename should be: 'sop_ticket_resolution_[YYYYMMDD].md'

## Documentation Requirements:
1. **Purpose and Scope**
   - Brief summary of the SOP or ticket resolution guide
   - Applicable systems, teams, or ticket types

2. **Trigger Events**
   - List of symptoms, alerts, or ticket subjects that initiate this SOP

3. **Step-by-Step Resolution Process**
   - Chronological, detailed steps to diagnose and resolve the issue or fulfill the request
   - Include commands, screenshots (if applicable), and links to relevant tools or dashboards
   - Decision points and what to do at each fork

4. **Escalation and Handoff**
   - Criteria for escalation to higher-level support or engineering
   - Contact information or ticket assignment rules
   - Required information to include when escalating

5. **Post-Resolution Actions**
   - Verification steps to confirm resolution
   - Documentation and ticket closure instructions
   - Communication/notification requirements

6. **Best Practices and Troubleshooting Tips**
   - Common pitfalls and solutions
   - Links to related SOPs or external resources

7. **Revision History**
   - Date and summary of changes or updates to the SOP

---
