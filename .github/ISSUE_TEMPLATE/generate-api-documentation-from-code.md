---
name: Generate API Documentation from Code
about: Ask AI to analyze code and create comprehensive API documentation
title: ''
labels: documentation
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Generate API Documentation

## Objective:
You will analyze API code and create comprehensive, developer-friendly API documentation following OpenAPI/Swagger standards.

Start by analyzing the relevant context.

## Context that you will analyze and its locations:
- **API Source Code**: I will specify directories containing API endpoints
- **Existing Docs**: Check for inline comments, decorators, or `/api-docs/`
- **Authentication**: Review auth middleware and security implementations

# Your output
- Deliver documentation as a **markdown file** saved in "/api-documentation" directory
- The filename should be: 'api_docs_v[version]_[YYYYMMDD].md'

## Documentation Requirements:
1. **API Overview**
   - Purpose and capabilities
   - Base URL and versioning
   - Authentication methods
   - Rate limiting

2. **Endpoint Documentation**
   For each endpoint:
   - HTTP method and path
   - Description and use cases
   - Request parameters (path, query, body)
   - Request/response examples
   - Status codes and errors
   - Code samples (curl, Python, JavaScript)

3. **Data Models**
   - Schema definitions
   - Field descriptions and types
   - Validation rules
   - Example payloads

4. **Authentication Guide**
   - Auth flow diagrams
   - Token management
   - Permission scopes
   - Security best practices

5. **Integration Guide**
   - Quick start tutorial
   - Common workflows
   - SDKs and libraries
   - Troubleshooting guide

6. **API Changelog**
   - Version history
   - Breaking changes
   - Deprecation notices
   - Migration guides
