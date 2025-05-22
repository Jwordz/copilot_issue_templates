---
name: Discussion Analytics for Internal Communications
about: Ask AI to analyze this repo's discussions
title: ''
labels: ''
assignees: ''

---

Analyze the last 90 days of GitHub Discussions to reveal communication patterns and engagement health.

## Your Mission:
Extract actionable insights from discussion data to help communications teams understand what's working and what's not.

## Available Data:
- Discussion titles, body content, timestamps
- All comments with authors and timestamps  
- Categories/labels assigned
- Answer status (marked as answered or not)

## Generate These Reports:

### 1. **Engagement Velocity**
Track momentum and response patterns:
- **Response time**: Hours until first comment by category
- **Conversation depth**: Avg comments per discussion
- **Participation spread**: Unique contributors per week
- **Dead zones**: Categories with <2 comments average

```markdown
| Category | Avg Response Time | Avg Comments | Participation Trend |
|----------|------------------|--------------|-------------------|
| Announcements | 18h | 1.2 | ↓ Declining |
| Questions | 2.3h | 5.4 | → Stable |
| Ideas | 4.1h | 8.7 | ↑ Growing |
```

### 2. **Content Effectiveness**
What generates discussion vs silence:
- **High engagement**: Topics with 10+ comments
- **No response**: Discussions with zero engagement
- **Question resolution**: % marked as answered within 7 days
- **Revival patterns**: Old discussions that reactivated

Key finding format:
- **Working well**: Technical how-tos (87% get responses)
- **Failing**: Policy announcements (71% no comments)
- **Opportunity**: Feature requests need faster responses

### 3. **Participation Health**
Who's carrying the conversation load:
- **Active voices**: People commenting 5+ times
- **New contributors**: First-time participants
- **Knowledge holders**: Who answers most questions
- **Silent teams**: Groups not participating

Red flags to highlight:
- 80% of answers from 3 people
- Zero participation from [specific teams]
- Increasing time to first response

## Output Requirements:
- **Time frame**: Last 90 days with week-over-week trends
- **Focus**: Patterns that affect communication effectiveness
- **Format**: Clear tables, specific percentages, named examples
- **Recommendations**: 3 specific actions with success metrics

## Do NOT:
- Guess at sentiment or feelings
- Make assumptions about offline impact
- Create complex network diagrams
- Analyze individual performance

## DO:
- Count observable behaviors
- Identify clear patterns
- Highlight bottlenecks
- Suggest specific improvements

Example recommendation:
"Create dedicated Q&A category - currently mixed with announcements, causing 64% of questions to get buried with 4.2x longer response times."
```
