---
name: Dependency Security and Freshness Audit
about: Ask AI to audit all dependencies in this repo
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Dependency Audit Report

## Objective:
Analyze all dependencies for security vulnerabilities, outdated packages, and optimization opportunities.

## Context:
- **Files to analyze**: package.json, requirements.txt, go.mod, Gemfile, pom.xml, etc.
- **Lock files**: Include all lock files for exact version analysis

# Your output
- Save as **markdown file** in "/audits" directory
- Filename: 'dependency_audit_[YYYYMMDD].md'

## Audit Sections:

### 1. **Critical Security Issues**
CVEs with CVSS score > 7.0

### 2. **Outdated Dependencies**
- Major versions behind
- Unmaintained packages
- Better alternatives available

### 3. **Optimization Opportunities**
- Duplicate functionality
- Bundle size impact
- Unused dependencies

### 4. **Upgrade Path**
- Safe immediate updates
- Breaking changes requiring work
- Migration strategies

### 5. **Action Items**
Prioritized by risk and effort
