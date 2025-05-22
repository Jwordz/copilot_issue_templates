---
name: Engineering Onboarding Generator
about: Ask AI to analyze codebase and create personalized onboarding materials
title: ''
labels: ''
assignees: ''

---

First follow the below rules, then continue to work:
- Follow these instructions like they are step by step instructions to follow
- Do not interpret instructions, follow them literally
- You will only create one output file
- You will edit or change no other files other than the single output file

# Generate Engineering Onboarding Program

## Objective:
You will analyze the codebase, team structure, and tools to create a comprehensive, role-specific onboarding program that gets engineers productive in days, not weeks.

Start by analyzing the relevant context.

## Context that you will analyze and its locations:
- **Codebase Structure**: Analyze repository architecture, key systems, dependencies
- **Team Context**: I will provide role details, team structure, and project focus in comments
- **Existing Docs**: Check `/docs`, `/wiki`, `README.md`, `CONTRIBUTING.md`
- **Development Workflow**: Review `.github/workflows`, CI/CD configs, deployment patterns, issues

# Your output
- Deliver onboarding guide as a **markdown file** saved in "/onboarding" directory
- The filename should be: 'onboarding_[role]_[team]_[YYYYMMDD].md'

## Onboarding Structure:

### 1. **Day 1: Environment Setup**
Generate executable checklist:
```markdown
## Setup Checklist (Target: 2-3 hours)
- [ ] **Development Environment**
  ```bash
  # Clone repositories
  git clone [repo-urls]
  
  # Install dependencies
  make setup  # or detailed commands
  ```
- [ ] **Access Verification**
  - [ ] GitHub org access
  - [ ] AWS/Cloud console (read-only initially)
  - [ ] Monitoring dashboards
  - [ ] Slack channels: #eng, #[team], #incidents

- [ ] **First Code Change**
  - Task: Update team roster in `/docs/team.md`
  - Purpose: Verify git workflow, CI/CD pipeline
  - Success: PR merged within 2 hours
```

### 2. **Week 1: Core Learning Path**
Based on codebase analysis, create priority-ordered modules:

```markdown
## Learning Modules

### Module 1: Architecture Overview (Day 2)
**Goal**: Understand system boundaries and data flow

**Reading** (2 hours):
- System architecture diagram
- Service communication patterns
- Database schema overview

**Hands-on** (3 hours):
- Trace a user request through the system
- Add logging to observe flow
- Document one undocumented flow

**Validation**:
- [ ] Can diagram the auth flow
- [ ] Identifies 3 service boundaries
- [ ] Explains data persistence strategy
```

### 3. **Technical Deep Dives**
Analyze codebase complexity and generate focused sessions:

```markdown
## Week 2-3: Domain Expertise

### Critical Path 1: [Feature Area]
**Why Critical**: Handles 60% of production traffic

**Pre-reading**:
- `/src/payments/README.md`
- Recent postmortem: [link]

**Code Tour**:
1. Start at `api/handlers/payment.ts`
2. Follow to `services/payment-processor.ts`
3. Understand retry logic in `utils/resilience.ts`

**Mini-Project**: Add metric for payment processing time
```

### 4. **Progressive Challenges**
Generate role-appropriate tasks with increasing complexity:

```markdown
## Onboarding Projects

### Starter (Day 3-5): Bug Fix
- **Issue**: #1234 - Validation error message unclear
- **Skills**: Codebase navigation, testing, PR process
- **Success Criteria**: Fix deployed to staging

### Intermediate (Week 2): Feature Enhancement  
- **Issue**: #5678 - Add filtering to admin dashboard
- **Skills**: Frontend/backend integration, API design
- **Mentor Check-in**: Design review before implementation

### Stretch (Week 3-4): System Improvement
- **Options**: 
  1. Improve test coverage for [module] from 45% to 80%
  2. Refactor [legacy component] with modern patterns
  3. Add observability to [black-box service]
```

### 5. **Knowledge Verification**
Create self-assessment checkpoints:

```markdown
## Week 1 Checkpoint
Rate yourself 1-5:
- [ ] Can explain our deployment pipeline
- [ ] Knows where to find architecture decisions
- [ ] Can debug common issues independently
- [ ] Understands our testing philosophy

Red flags: Any 1-2 ratings require mentor discussion
```

### 6. **Relationship Building**
Map key connections:

```markdown
## Key Relationships

### Direct Team
| Person | Role | Expertise | First Meeting Topic |
|--------|------|-----------|-------------------|
| [Name] | Tech Lead | System design | Architecture overview |

### Cross-functional Partners
- **Product**: [Name] - Feature prioritization process
- **SRE**: [Name] - Production access and monitoring
- **Security**: [Name] - Security review process
```

### 7. **Production Readiness**
Progressive production access:

```markdown
## Production Access Ladder
- **Week 1**: Read-only logs and metrics
- **Week 2**: Staging deployment access
- **Week 3**: Production deployment (with buddy)
- **Week 4**: On-call shadow rotation
- **Week 6**: Primary on-call eligible
```

### 8. **30-Day Success Metrics**
Define clear success criteria:

```markdown
## 30-Day Goals
### You will have:
- [ ] Merged 5+ PRs of increasing complexity
- [ ] Led one design discussion
- [ ] Documented one system component
- [ ] Fixed one customer-reported bug
- [ ] Improved one metric by 10%

### Your manager will see:
- Independent debugging capability
- Proactive communication
- Code review participation
- Team culture contribution
```

### 9. **Resources & References**
Curated, role-specific resources:

```markdown
## Essential Resources
### Daily Use
- [Runbook]: Link to operational procedures
- [Metrics Dashboard]: Primary system health view
- [Team Playbook]: How we work document

### Deep Learning
- [Video]: Architecture deep dive recording
- [Blog]: Our approach to [key technology]
- [Course]: Internal [skill] workshop

### Emergency Contacts
- Incident: Page via #incidents
- Blocked: DM your buddy first, then team lead
- Questions: #[team]-questions is judgment-free
```

## Analysis Requirements:
- Identify top 10 most critical code paths
- Map complexity levels to week-by-week progression
- Generate role-specific focus areas
- Include team-specific conventions and patterns
- Create measurable checkpoint criteria
