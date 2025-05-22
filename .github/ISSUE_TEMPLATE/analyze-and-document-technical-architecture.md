---
name: Analyze and Document Technical Architecture
about: Ask Copilot to analyze codebase and create architectural documentation
title: "[ARCH]"
labels: documentation
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will edit or change no other files other than the single output file

# Analyze and Document Technical Architecture

## Objective:
You will analyze a codebase or technical system and create comprehensive architectural documentation suitable for onboarding new engineers and technical decision-making.

Start by analyzing the relevant context.

## Context that you will analyze and its locations:
- **Source Code**: Repository root and all subdirectories
- **Existing Documentation**: Check `/docs`, `/README.md`, and inline code comments
- **Configuration Files**: Analyze all config files for infrastructure and deployment patterns

# Your output
- Deliver the documentation as a **markdown file** saved in "/documentation" directory
- The filename should be: 'architecture_analysis_[YYYYMMDD].md'

## Analysis Requirements:
1. **System Overview**
   - High-level architecture diagram (in mermaid syntax)
   - Key components and their relationships
   - Technology stack breakdown

2. **Component Deep Dive**
   - Purpose of each major component
   - Dependencies and interactions
   - Data flow between components

3. **Critical Paths**
   - Identify and document critical user journeys
   - Performance considerations
   - Failure points and resilience patterns

4. **Technical Debt Assessment**
   - Areas needing refactoring
   - Security considerations
   - Scalability limitations

5. **Recommendations**
   - Priority improvements
   - Migration strategies if applicable
   - Resource requirements
