---
name: Repository Health Check
about: Ask AI to analyze a single repo's health metrics and practices
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Repository Health Assessment

## Objective:
Analyze this repository's health indicators and generate actionable improvement recommendations.

## Context:
- **Repository**: Current repository only
- **Analysis Scope**: All branches, commits, issues, PRs from last 90 days

# Your output
- Deliver report as **markdown file** saved in "/.github/health-reports" directory
- Filename: 'repo_health_[YYYYMMDD].md'

## Analysis Metrics:

### 1. **Code Velocity**
- Commit frequency and patterns
- PR merge times
- Release cadence
- Bottleneck identification

### 2. **Quality Indicators**
- Test coverage trends
- Bug discovery rate
- Code review depth
- Documentation freshness

### 3. **Collaboration Health**
- PR review distribution
- Issue response times
- Bus factor analysis
- Knowledge silos

### 4. **Technical Indicators**
- Dependency age
- Security vulnerability count
- Build performance
- Tech debt markers

### 5. **Recommendations**
Prioritized list with effort/impact scores
