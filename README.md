# Copilot Issue Templates

A collection of GitHub issue templates designed to leverage GitHub Copilot and AI to automate common software development and documentation tasks. Created and maintained by [@mattnigh](https://github.com/mattnigh).

## About This Repository

This repository contains GitHub issue templates that use AI to help you with various tasks such as:
- Technical documentation generation
- Repository analysis
- Project health monitoring
- Engineering onboarding
- Dependency analysis
- And more!

Each template provides step-by-step instructions for Copilot to follow, ensuring consistent, high-quality outputs with minimal effort. Simply create an issue using one of the templates, and let AI do the heavy lifting.

## Available Templates

### Technical Documentation

| Template | Description | Create Issue |
|----------|-------------|-------------|
| [Analyze and Document Technical Architecture](/.github/ISSUE_TEMPLATE/analyze-and-document-technical-architecture.md) | Analyzes your codebase to produce architectural documentation with system overviews, component details, and critical paths. Includes architecture diagrams, data flows, technical debt assessment, and improvement recommendations. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=analyze-and-document-technical-architecture.md) |
| [Generate API Documentation from Code](/.github/ISSUE_TEMPLATE/generate-api-documentation-from-code.md) | Creates comprehensive API documentation from source code, featuring endpoint details, request/response examples, authentication guides, data models, and integration tutorials. Follows OpenAPI/Swagger standards. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=generate-api-documentation-from-code.md) |
| [Documentation Gap Analysis](/.github/ISSUE_TEMPLATE/documentation-gap-analysis.md) | Identifies missing documentation across APIs, code, and operational procedures. Generates templates for the top 5 documentation gaps and provides a priority matrix based on impact vs. effort. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=documentation-gap-analysis.md) |

### Analysis and Insights

| Template | Description | Create Issue |
|----------|-------------|-------------|
| [Analyze Repository Strategic Insights](/.github/ISSUE_TEMPLATE/analyze-repository-strategic-insights.md) | Provides executive-level analysis of 90 days of repository activity, identifying macro trends and strategic opportunities. Includes metrics on issue resolution, PR velocity, contributor growth, and technical debt indicators with actionable recommendations. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=analyze-repository-strategic-insights.md) |
| [Previous Month Repository Activity Analysis](/.github/ISSUE_TEMPLATE/previous-month-repository-activity-analysis.md) | Analyzes the previous month's repository activity compared to a 3-month baseline. Tracks commit patterns, PR velocity, contributor behavior, bug trends, and code quality indicators with weekly breakdowns. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=previous-month-repository-activity-analysis.md) |
| [Repository Health Check](/.github/ISSUE_TEMPLATE/repository-health-check.md) | Assesses repository health across code velocity, quality indicators, collaboration patterns, and technical metrics over 90 days. Delivers prioritized recommendations with effort/impact scores. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=repository-health-check.md) |
| [Discussion Analytics for Internal Communications](/.github/ISSUE_TEMPLATE/discussion-analytics-for-internal-communications.md) | Analyzes 90 days of GitHub Discussions to reveal communication patterns. Reports on engagement velocity, content effectiveness, participation distribution, and recommends specific improvements for team communication. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=discussion-analytics-for-internal-communications.md) |

### Project Management

| Template | Description | Create Issue |
|----------|-------------|-------------|
| [Project Health Dashboard](/.github/ISSUE_TEMPLATE/project-health-dashboard.md) | Creates an executive dashboard highlighting delivery risks, team capacity, external blockers, and quality trends. Includes actionable insights about at-risk features, resource allocation needs, and dependencies requiring attention. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=project-health-dashboard.md) |
| [Monthly Communications Work Impact Report](/.github/ISSUE_TEMPLATE/monthly-communications-work-impact-report.md) | Tracks communications team performance via issue analysis, showing items delivered, cycle times, and on-time rates. Breaks down work by content type, identifies process bottlenecks, and recommends specific improvements with success targets. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=monthly-communications-work-impact-report.md) |

### Code Analysis

| Template | Description | Create Issue |
|----------|-------------|-------------|
| [Technical Debt Hotspot Analysis](/.github/ISSUE_TEMPLATE/technical-debt-hotspot-analysis.md) | Identifies technical debt using metrics like change frequency, bug density, and complexity. Classifies debt by type, quantifies business impact, and creates a remediation roadmap with quick wins and strategic initiatives. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=technical-debt-hotspot-analysis.md) |
| [Dependency Security and Freshness Audit](/.github/ISSUE_TEMPLATE/dependency-security-and-freshness-audit.md) | Audits project dependencies for security vulnerabilities (CVEs), outdated packages, and optimization opportunities. Provides a prioritized upgrade path with safety assessments and migration strategies. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=dependency-security-and-freshness-audit.md) |

### Team and Collaboration

| Template | Description | Create Issue |
|----------|-------------|-------------|
| [Team Sentiment Analyzer](/.github/ISSUE_TEMPLATE/team-sentiment-analyzer.md) | Assesses team health through 90 days of observable behaviors like PR cycle times, review depth, and work patterns. Identifies potential issues such as overwork, knowledge silos, and collaboration breakdowns without relying on subjective measures. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=team-sentiment-analyzer.md) |
| [Engineering Onboarding Generator](/.github/ISSUE_TEMPLATE/engineering-onboarding-generator.md) | Creates a structured onboarding program based on your codebase and team structure. Includes environment setup, learning modules, progressive hands-on projects, and validation checkpoints to accelerate new engineer productivity. | [Create Issue](https://github.com/mattnigh/copilot_issue_templates/issues/new?template=engineering-onboarding-generator.md) |

## How to Use These Templates

1. Click on the "Create Issue" link next to the template you want to use
2. Follow any additional instructions in the template
3. Submit the issue
4. Copilot will analyze your repository and generate the requested output

## Directory Structure

Each template will create output files in specific directories. Make sure these directories exist in your repository or Copilot will create them. Or simply change the endpoint directory to one you prefer:

- `/documentation` - For architectural documentation
- `/reports` - For strategic analysis
- `/audits` - For dependency audits
- `/docs/analysis` - For documentation gap analysis
- `/onboarding` - For engineering onboarding materials
- `/api-documentation` - For API documentation
- `/analytics/monthly` - For monthly repository activity analysis
- `/dashboards` - For project health dashboards
- `/team-analytics` - For team health signals
- `/tech-debt-analysis` - For technical debt analysis
- `/.github/health-reports` - For repository health reports

## Contributing

Feel free to fork this repository and adapt these templates to your specific needs. This repo will be sporatically maintained.

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.