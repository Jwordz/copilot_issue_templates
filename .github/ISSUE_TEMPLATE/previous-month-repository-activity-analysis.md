---
name: Previous Month Repository Activity Analysis
about: Ask AI to analyze last month's repo activity and generate insights
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Monthly Repository Activity Analysis

## Objective:
Analyze all repository activity from the previous calendar month to identify trends, bottlenecks, and opportunities.

## Context:
- **Analysis Period**: Previous calendar month (1st to last day)
- **Data Sources**: Commits, PRs, issues, reviews, deployments, contributor activity
- **Comparison Baseline**: Previous 3-month average

# Your output
- Save as **markdown file** in "/analytics/monthly" directory
- Filename: 'monthly_activity_[YYYY]_[MM].md'

## Report Structure:

### 1. **Executive Summary**
```markdown
## Key Metrics vs 3-Month Average
- **Velocity**: 47 PRs merged (+12%)
- **Quality**: 3.2 bugs/week (-23%)
- **Participation**: 18 active contributors (+3)
- **Efficiency**: 14hr median PR cycle time (-4hrs)

## Critical Insights
1. Feature velocity increased but review bottleneck emerging
2. Bug rate improvement from new testing requirements
3. Documentation debt growing - 68% of PRs lack docs
```

### 2. **Development Velocity**
```markdown
## Commit & PR Activity
| Week | Commits | PRs Opened | PRs Merged | Avg Cycle Time |
|------|---------|------------|------------|----------------|
| 1 | 142 | 12 | 10 | 18h |
| 2 | 168 | 15 | 14 | 12h |
| 3 | 134 | 11 | 9 | 22h |
| 4 | 189 | 18 | 14 | 8h |

## Velocity Blockers
- Code review bandwidth (5 PRs waiting >48hrs)
- CI flakiness caused 23% of builds to retry
- Dependency on external team delayed 4 PRs
```

### 3. **Contributor Patterns**
```markdown
## Contribution Distribution
| Contributor | Commits | PRs | Reviews | Bus Factor Risk |
|------------|---------|-----|---------|-----------------|
| @user1 | 87 | 12 | 34 | HIGH - owns auth |
| @user2 | 62 | 8 | 28 | Medium |
| @user3 | 41 | 15 | 12 | Low |

## New Contributors
- @newuser1: First PR merged, assigned mentor
- @newuser2: Struggling with setup, 3 PRs abandoned

## Review Load Distribution
- 67% of reviews by 2 people (bottleneck risk)
- Average review response: 6.2 hours
```

### 4. **Issue & Bug Trends**
```markdown
## Issue Metrics
- **Opened**: 34 (23 bugs, 11 features)
- **Closed**: 29 (19 bugs, 10 features)
- **Backlog Growth**: +5 issues
- **Median Resolution**: 4.2 days

## Bug Analysis
| Category | Count | Avg Fix Time | Root Cause |
|----------|-------|--------------|------------|
| API | 8 | 2.1 days | Missing validation |
| UI | 6 | 1.2 days | State management |
| Data | 5 | 5.8 days | Schema mismatch |
| Perf | 4 | 3.4 days | N+1 queries |
```

### 5. **Code Quality Indicators**
```markdown
## Quality Metrics
- **Test Coverage**: 72% (-2% from last month)
- **Lint Violations**: 143 new, 89 fixed
- **Tech Debt Markers**: 18 new TODOs added
- **Documentation**: 32% of functions undocumented

## Hotspots (files changed >5 times)
1. `auth/provider.js` - 11 changes (refactor needed)
2. `api/handlers.js` - 8 changes (growing complexity)
3. `utils/validation.js` - 7 changes (extract library?)
```

### 6. **Release & Deployment Health**
```markdown
## Deployment Frequency
- **Production Deploys**: 12 (3/week average)
- **Rollbacks**: 1 (API timeout issue)
- **Hotfixes**: 2 (both data-related)

## Release Quality
| Release | Features | Bugs Found | User Impact |
|---------|----------|------------|-------------|
| v2.3.0 | 4 | 2 | Low |
| v2.3.1 | 1 | 0 | None |
| v2.4.0 | 6 | 4 | Medium |
```

### 7. **Actionable Recommendations**

```markdown
## Immediate Actions (This Week)
1. **Add 2nd reviewer** to auth components - reduce bus factor
2. **Fix CI flakiness** - 23% retry rate costs 8 dev-hours/week
3. **Document hotspot files** - prevent knowledge loss

## Process Improvements (This Month)
1. **Review SLA**: Implement 24hr review target
2. **Bug Triage**: Add severity labels for prioritization
3. **New Contributor Onboarding**: Create setup automation

## Strategic Initiatives (This Quarter)
1. **Refactor auth/provider.js** - 11 changes indicates design issue
2. **Test Coverage Push** - Target 80% before feature freeze
3. **Documentation Sprint** - Dedicate 1 sprint to docs debt
```

### 8. **Month-over-Month Trends**
```markdown
## Trending Up ✅
- PR merge rate: +12%
- New contributors: +3
- Bug fix time: -1.3 days

## Trending Down ⚠️
- Test coverage: -2%
- Documentation: -8%
- Review response time: +2hrs

## Stable ➡️
- Deployment frequency
- Issue resolution time
- Active contributor count
```

## Analysis Requirements:
- Include sparkline trends where applicable
- Flag statistical anomalies
- Compare to repository's historical baselines
- Identify correlation between metrics
- Provide specific, actionable recommendations
