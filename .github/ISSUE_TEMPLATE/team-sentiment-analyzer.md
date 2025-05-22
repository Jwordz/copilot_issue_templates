---
name: Team Sentiment Analyzer
about: Ask AI to analyze team health through observable repo behaviors and communication
  patterns
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Team Sentiment Analyzer

## Objective:
Identify team health signals through measurable repository behaviors and communication patterns.

## Context:
- **Data Sources**: PR velocity, review patterns, issue resolution times, commit patterns
- **Time Period**: 90 days with weekly breakdowns
- **Key Principle**: Measure behaviors, not feelings

# Your output
- Save as **markdown file** in "/team-analytics" directory
- Filename: 'team_health_signals_[YYYYMMDD].md'

## Analysis Framework:

### 1. **Team Health Indicators**
```markdown
## Observable Signals (Last 30 Days)

| Metric | Value | Baseline | Signal |
|--------|-------|----------|--------|
| PR Cycle Time | 72h | 24h | 🔴 3x slower |
| Review Depth | 1.2 comments/PR | 4.5 | 🔴 Rubber stamping |
| After-hours commits | 34% | 12% | 🔴 Overwork |
| PR Abandonment | 18% | 3% | 🟡 Frustration |
| Solo work % | 78% | 45% | 🟡 Silos forming |

**Key Finding**: Team is shipping slower with less collaboration
