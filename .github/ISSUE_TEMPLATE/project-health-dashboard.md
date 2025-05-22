---
name: Project Health Dashboard
about: Ask AI to analyze project status and generate executive-ready health metrics
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Project Health Dashboard Generator

## Objective:
Generate comprehensive project health metrics by analyzing issues, milestones, and activity patterns.

## Context:
- **Data Sources**: All issues, PRs, milestones, labels, comments
- **Time Period**: Current month + 90-day trend
- **Health Indicators**: Velocity, risk, blockers, team capacity

# Your output
- Save as **markdown file** in "/dashboards" directory
- Filename: 'project_health_[YYYYMMDD].md'

## Dashboard Structure:

### 1. **Executive Summary**
```markdown
## Overall Health: 🟡 MODERATE RISK

**Critical Insights:**
1. **Delivery Risk**: 2 critical features behind by 8 days
2. **Team Capacity**: 140% allocated, burnout risk
3. **Blockers**: External dependency blocking 5 features
4. **Quality**: Bug rate increased 35% this month

**Required Actions:**
- Escalate: Data team API blocking $2M feature
- Decide: Cut feature X or extend timeline 2 weeks
- Resource: Need +2 engineers or reduce scope
