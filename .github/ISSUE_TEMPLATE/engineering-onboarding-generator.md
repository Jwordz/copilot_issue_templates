---
name: Engineering Onboarding Generator
about: Ask AI to analyze codebase and create personalized onboarding materials
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Generate Engineering Onboarding Program

## Objective:
You will analyze the codebase, team structure, and tools to create a comprehensive, role-specific onboarding program that gets engineers productive in days, not weeks.

Start by analyzing the relevant context within this repo.

## Context that you will analyze and its locations:
- **Codebase Structure**: Analyze repository architecture, key systems, dependencies
- **Team Context**: I will provide role details, team structure, and project focus in comments
- **Existing Docs**: Check `/docs`, `/wiki`, `README.md`, `CONTRIBUTING.md`
- **Development Workflow**: Review `.github/workflows`, CI/CD configs, deployment patterns, issues, pull requests, etc.

# Your output
- Deliver onboarding guide as a **markdown file** saved in "/onboarding" directory
- The filename should be: 'onboarding_[role]_[team]_[YYYYMMDD].md'
