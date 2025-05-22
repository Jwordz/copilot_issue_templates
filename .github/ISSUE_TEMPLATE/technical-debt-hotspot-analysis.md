---
name: Technical Debt Hotspot Analysis
about: Ask AI to analyze codebase and identify high-impact technical debt
title: "[debt]"
labels: documentation
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Technical Debt Hotspot Analysis

## Objective:
You will analyze the codebase to identify technical debt hotspots, quantify their impact, and create a data-driven remediation roadmap.

Start by analyzing the relevant context.

## Context that you will analyze and its locations:
- **Source Code**: Full repository scan, prioritize `/src`, `/lib`, `/app` directories
- **Git History**: Analyze commit frequency, bug fix patterns, and churn rates
- **Issue Tracker**: Check for recurring bugs, performance issues, feature blockers
- **CI/CD Logs**: Review build times, test failures, deployment issues

# Your output
- Deliver analysis as a **markdown file** saved in "/tech-debt-analysis" directory
- The filename should be: 'tech_debt_hotspots_[YYYYMMDD].md'

## Analysis Framework:

### 1. **Hotspot Identification**
Calculate and rank by composite score:
- **Change Frequency**: Files modified > 10 times in 90 days
- **Bug Density**: Issues per 1000 LOC
- **Complexity**: Cyclomatic complexity > 10
- **Team Impact**: Number of developers touching file
- **Size**: Files > 500 LOC

Output format:
```markdown
| File | Change Freq | Bug Density | Complexity | Impact Score | Priority |
|------|-------------|-------------|------------|--------------|----------|
| auth/manager.js | 47 | 8.2 | 15 | 89 | CRITICAL |
```

### 2. **Debt Categories**
Classify each hotspot:
- **Architectural**: Violates design principles, coupling issues
- **Code Quality**: Duplication, naming, readability
- **Testing**: Coverage < 60%, brittle tests
- **Performance**: Known bottlenecks, inefficient algorithms
- **Security**: Outdated dependencies, vulnerable patterns
- **Documentation**: Missing or outdated docs

### 3. **Impact Analysis**
For each hotspot, calculate:
- **Development Velocity Impact**: Extra hours per sprint
- **Bug Introduction Rate**: New bugs per change
- **Onboarding Friction**: Time to understand for new devs
- **Operational Risk**: Production incident correlation

### 4. **Root Cause Analysis**
Identify patterns:
- Technical decisions that led to debt
- External pressure points (deadlines, pivots)
- Knowledge gaps or skill mismatches
- Process failures

### 5. **Remediation Roadmap**

**Quick Wins** (< 1 week effort, high impact):
```markdown
## Q1: Immediate Actions
- [ ] Refactor auth/manager.js - split into 3 modules (3 days)
- [ ] Add integration tests to payment flow (2 days)
- [ ] Update critical dependencies in user service (1 day)

Estimated velocity gain: 15%
```

**Strategic Initiatives** (1-3 month efforts):
```markdown
## Q2-Q3: Major Refactors
1. **API Gateway Redesign**
   - Current state: 5 services with circular dependencies
   - Target state: Clean gateway pattern
   - Effort: 6 weeks
   - Risk: Medium (feature flag rollout)
   - ROI: 30% reduction in API errors

2. **Database Schema Migration**
   - [Details...]
```

### 6. **Metrics & Tracking**
Define success metrics:
- Lead time reduction target
- Bug rate improvement
- Build time optimization
- Test stability increase

### 7. **Investment Analysis**
```markdown
## Cost/Benefit Analysis
| Initiative | Dev Weeks | Weekly Savings | Payback Period | 1-Year ROI |
|------------|-----------|----------------|----------------|------------|
| Refactor auth | 2 | 0.5 | 4 weeks | 24 weeks |
```

### 8. **Risk Mitigation**
For each major initiative:
- Rollback strategies
- Feature flag approach
- Parallel running plans
- Team knowledge transfer

## Output Requirements:
- Be specific with file paths and line numbers
- Include code snippets showing problematic patterns
- Provide refactoring examples for top 3 hotspots
- Generate mermaid diagrams for architecture issues
- Create quarterly milestone checkpoints
