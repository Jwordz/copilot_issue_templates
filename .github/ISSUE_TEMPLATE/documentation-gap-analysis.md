---
name: Documentation Gap Analysis
about: Ask AI to assess documentation completeness
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Documentation Coverage Report

## Objective:
Identify missing or outdated documentation and generate templates.

## Context:
- **Code files**: All source files for inline docs
- **Doc files**: README, docs/, wiki/
- **API definitions**: OpenAPI, GraphQL schemas

# Your output
- Save as **markdown file** in "/docs/analysis" directory
- Filename: 'doc_coverage_[YYYYMMDD].md'

## Coverage Analysis:

### 1. **Public API Documentation**
- Undocumented endpoints
- Missing parameter descriptions
- No example requests/responses

### 2. **Code Documentation**
- Functions without docstrings
- Complex logic without comments
- Missing type definitions

### 3. **Operational Docs**
- No runbooks for critical services
- Missing deployment guides
- Outdated architecture diagrams

### 4. **Generated Templates**
For top 5 gaps, provide filled templates

### 5. **Priority Matrix**
Impact vs effort for documentation tasks
