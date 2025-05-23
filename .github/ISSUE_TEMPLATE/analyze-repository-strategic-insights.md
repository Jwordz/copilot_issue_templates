---
name: Analyze Repository Strategic Insights
about: Generate executive-level analysis of issues, discussions, and innovation patterns
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will edit or change no other files other than the single output file

# Analyze Repository Strategic Insights

## Objective:
You will analyze a repository's issues, pull requests, and discussions to generate an executive-level strategic report identifying macro trends, innovation patterns, and strategic opportunities from the perspective of an Engineering VP and Distinguished Engineer.

Start by analyzing the relevant context.

## Context that you will analyze and its locations:
- **Issues**: All open issues + closed issues from last 90 days
- **Pull Requests**: All merged PRs from last 90 days
- **Discussions**: All discussion threads (if enabled)
- **Labels**: Frequency and co-occurrence patterns
- **Contributors**: Unique contributors and their activity patterns

# Your output
- Deliver the analysis as a **markdown file** saved in "/reports" directory
- The filename should be: 'strategic_analysis_[repository_name]_[YYYYMMDD].md'

## Analysis Requirements:

### 1. **Executive Summary**
   - Top 3 actionable insights based on data
   - Issue resolution rate (closed/opened ratio)
   - PR merge velocity (median time to merge)
   - Contributor growth rate (new contributors per month)

### 2. **Quantitative Health Metrics**
   - **Issue Metrics**
     - Total open issues + 90-day trend
     - Median time to first response
     - Median time to close
     - Stale issue count (>30 days no activity)
   
   - **PR Metrics**
     - Weekly PR merge count + trend
     - Median review cycles before merge
     - PR size distribution (lines changed)
   
   - **Engagement Metrics**
     - Unique contributors (last 30 vs 90 days)
     - Comments per issue/PR average
     - Most active discussion topics

### 3. **Pattern Recognition**
   - **Recurring Themes** (issues/discussions mentioning same concepts 5+ times)
   - **Feature Clusters** (group feature requests by similarity)
   - **Bug Patterns** (common failure modes from bug reports)
   - **Performance Concerns** (issues mentioning speed/scale/memory)

### 4. **Technical Debt Indicators**
   - Count of issues labeled "bug" vs "feature"
   - Issues mentioning "refactor", "technical debt", "legacy"
   - Long-open bugs (>90 days)
   - Regression mentions in last 30 days

### 5. **Community Signals**
   - **New Contributor Success**
     - First PR success rate
     - Time to first merged PR
   
   - **Core Team Bandwidth**
     - Response time by maintainer
     - Number of PRs waiting for review >7 days
   
   - **Knowledge Distribution**
     - Top 5 contributors by merged PRs
     - Percentage of work by top 5 vs rest

### 6. **Strategic Opportunities**
   Based on data patterns, identify:
   - **Quick Wins**: High-frequency, low-complexity requests
   - **Architecture Discussions**: Issues proposing structural changes
   - **User Journey Gaps**: Common user frustrations
   - **Automation Opportunities**: Repetitive issues that could be automated

### 7. **Risk Indicators**
   - **Maintainer Burnout Signals**
     - Increasing response times
     - Declined PR review quality (reverts, hotfixes)
   
   - **Project Momentum**
     - PR merge rate trajectory
     - New contributor retention (return after first PR)
   
   - **Critical Gaps**
     - Security issues age and count
     - Breaking change discussions

### 8. **Actionable Recommendations**
   For each recommendation, provide:
   - Specific metric driving the recommendation
   - Expected impact if addressed
   - Link to relevant issues/discussions as evidence

## Data Visualization Requirements:
```mermaid
# Include these charts:
1. Issue/PR volume over time (line chart)
2. Top 10 issue labels by frequency (bar chart)
3. Contributor activity distribution (pie chart)
4. Time-to-close distribution (histogram)
```

## Output Structure:
- Lead with numbers that matter
- Support with specific issue/PR examples
- Focus on trends, not snapshots
- Highlight outliers that indicate systemic issues
- Keep recommendations tied to measurable outcomes
