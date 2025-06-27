# Standard Operating Procedures (SOP) - Compliance Category Ticket Resolution

## Purpose and Scope

This Standard Operating Procedure (SOP) provides step-by-step guidance for GitHub Support personnel (Supportocats) to efficiently handle compliance-related customer inquiries and ticket resolution. This document covers common compliance topics including security certifications, business continuity planning, data residency requirements, and regulatory compliance standards.

**Applicable Systems:** GitHub Enterprise Cloud (GHEC), GitHub.com Services  
**Target Teams:** Support Squad, Customer Success, Enterprise Support  
**Ticket Categories:** Compliance, Security, Certifications, Regulatory Requirements

## Trigger Events

This SOP should be initiated when customers submit tickets or inquiries related to:

- **Security Certifications:** ISO 27001, SOC 1/2/3 reports, security attestations
- **Business Continuity:** RTO/RPO requirements, disaster recovery planning, BCDR documentation
- **Data Management:** Data residency requirements, data location inquiries
- **Regulatory Compliance:** PCI-DSS requirements, industry-specific compliance standards
- **Confidential Documentation:** Requests for documents requiring NDA or confidentiality agreements
- **Trust Portal Access:** Questions about accessing compliance reports via Customer Compliance tab

**Common Ticket Subjects/Keywords:**
- "ISO 27001", "SOC report", "compliance documentation"
- "RTO", "RPO", "disaster recovery", "business continuity"
- "data residency", "data location", "where is data stored"
- "PCI-DSS", "PCI compliance", "payment card industry"
- "NDA", "confidential", "under NDA", "attestation of compliance"

## Step-by-Step Resolution Process

### Step 1: Initial Assessment and Classification

1. **Read the ticket carefully** to identify the specific compliance requirement
2. **Classify the request** into one of the main categories:
   - Security Certifications (ISO 27001, SOC reports)
   - Business Continuity/Disaster Recovery
   - Data Residency
   - Regulatory Compliance
   - NDA-required documentation

### Step 2: Determine Customer Eligibility and Access Requirements

1. **Check customer's enterprise status**:
   - Verify if customer has GitHub Enterprise Cloud (GHEC)
   - Confirm access to Customer Compliance tab in enterprise settings

2. **Assess NDA requirements**:
   - Check if requested documentation requires confidentiality agreement
   - Use Microsoft's Contract Experience site to verify existing NDA status
   - Reference: https://github.com/github/support-squad-compliance/blob/main/docs/misc/nda%20procedures.md

### Step 3: Category-Specific Resolution

#### A. ISO 27001 Certificates

**Customer Self-Service Options:**
1. Direct customer to GitHub Trust Portal: https://ghec.github.trust.page/
2. Guide to Customer Compliance tab in Enterprise account:
   - Top-right corner → Profile photo → "Your enterprise"
   - Select enterprise → "Compliance" tab
   - Locate ISO/IEC 27001:2013 certification
   - Download or View options available

**Alternative Access:**
- Reference Customer Security Trust repo
- Use Slack command `.rem iso 27001` for latest version link
- Provide Statement of Applicability (SoA) if requested

#### B. RTO & RPO Requirements

**Provide Definitions:**
- **RTO (Recovery Time Objective):** Maximum acceptable downtime before system must be restored
- **RPO (Recovery Point Objective):** Maximum acceptable data loss measured in time

**Customer Resources:**
- Direct to Customer Security Trust FAQ: https://github.com/github/customer-security-trust/blob/main/FAQ/FAQ.md#does-github-have-an-rto-rpo-or-document-how-it-manages-backups-and-exercise-frequency
- Provide context-appropriate examples and explanations

#### C. Business Continuity and Disaster Recovery (BCDR/BCP)

**Explain Distinction:**
- **Business Continuity Plan (BCP):** Comprehensive plan for entire organization operations during disruption
- **Disaster Recovery (DR):** IT-focused subset for restoring technology systems and infrastructure

**Customer Resources:**
- Reference Customer Security Trust FAQ for BCDR guidance
- For customers on appropriate terms, share: GitHub.com Services Continuity and Incident Management Plan
- Document location: https://github.com/github/customer-security-trust/blob/main/BCDR%20Plans/

#### D. Data Residency

**Standard Response:**
Use the canned response for most inquiries:

"Details about how our data is stored and compliance for audit reports are complex (because they involve multiple sites and partners) and subject to change, so my recommendation is to review the [compliance reports for your enterprise](https://docs.github.com/en/enterprise-cloud@latest/admin/overview/accessing-compliance-reports-for-your-enterprise) which cover the details you need for many common audits.

If you need to guarantee data residency in a specific region, we do offer [GitHub Enterprise Cloud with data residency](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/about-github-enterprise-cloud-with-data-residency) which is a separate product and something that you would need to migrate to. If you're interested in this, you can find more information in '[Getting started with data residency for GitHub Enterprise Cloud](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/getting-started-with-data-residency-for-github-enterprise-cloud)' and let me know if you have any questions."

**Note:** This does not apply to Proxima/GHEC-DR customers who have region-specific instances.

#### E. Regulatory Compliance

**PCI-DSS Requests:**
- For customers under NDA: Share PCI-DSS AOC (Attestation of Compliance)
- Use Slack command `.rem pci-dss` for latest version
- For Shared Responsibility Matrix: `.rem pci-srm`

**SOC Reports:**
- **SOC 1:** Financial reporting controls (`.rem SOC1`)
- **SOC 2:** Security, availability, confidentiality controls (`.rem SOC2`)  
- **SOC 3:** Public summary of SOC 2 (`.rem SOC3`)
- SOC 3 publicly available at: https://ghec.github.trust.page/resources

#### F. NDA-Required Documentation

**Process:**
1. Check Microsoft's Contract Experience site for existing NDA
2. If no existing NDA, customer must sign NDA via Microsoft
3. Reference GitHub CELA NDA guide: https://github.com/github/CELA/blob/main/Non-Disclosure%20Agreements%20(NDA).md
4. Use Microsoft standard agreements (covers GitHub as subsidiary)
5. For template changes, direct to Microsoft's Global Contracting Office

### Step 4: Provide Documentation and Resources

1. **Always provide self-service options first**
2. **Include relevant links and documentation paths**
3. **Use Slack commands for internal document retrieval when appropriate**
4. **Explain any limitations or requirements clearly**

## Escalation and Handoff

### Escalation Criteria

Escalate to Level 2 Support or Engineering when:
- Customer requires documentation not covered in standard resources
- NDA process encounters complications or disputes
- Data residency requirements exceed standard GitHub offerings
- Custom compliance requirements outside standard certifications
- Legal or contractual questions arise

### Required Information for Escalation

When escalating, include:
- **Customer Details:** Enterprise name, contact information, support tier
- **Specific Requirement:** Exact compliance standard or documentation needed
- **Business Context:** Why the information is needed (audit, procurement, etc.)
- **Timeline:** Customer's required response timeframe
- **Previous Actions:** Steps already taken and resources provided
- **NDA Status:** Whether NDA is in place or required

### Contact Information

- **Support Squad Compliance:** Via GitHub internal Slack channels
- **Legal Team (CELA):** For NDA and contractual questions
- **Customer Success:** For enterprise-level compliance discussions

## Post-Resolution Actions

### Verification Steps

1. **Confirm customer received required documentation**
2. **Verify customer can access self-service resources**
3. **Ensure all provided links and resources are functional**
4. **Check that customer understands any limitations or requirements**

### Documentation and Closure

1. **Update ticket with summary of resolution**
2. **Document any new processes or findings for team knowledge**
3. **Tag ticket appropriately for future reference**
4. **Close ticket with appropriate resolution code**

### Communication Requirements

1. **Follow up within 24-48 hours if no customer response**
2. **Provide clear next steps if additional actions required**
3. **Notify relevant teams of any process improvements identified**

## Best Practices and Troubleshooting Tips

### Common Pitfalls and Solutions

1. **Issue:** Customer cannot find Compliance tab
   - **Solution:** Verify enterprise account access and guide through navigation steps
   - **Tip:** Screenshots can be helpful for complex UI navigation

2. **Issue:** Customer requests documentation that requires NDA but doesn't want to sign
   - **Solution:** Explain the legal requirements and offer alternative public resources
   - **Tip:** Emphasize business benefits of the NDA process

3. **Issue:** Confusion between different compliance standards
   - **Solution:** Provide clear definitions and explain which standard applies to their use case
   - **Tip:** Use comparison tables when helpful

4. **Issue:** Customer needs compliance information urgently for audit
   - **Solution:** Prioritize self-service options and expedite NDA process if needed
   - **Tip:** Set clear expectations about processing times

### Links to Related SOPs

- Customer Security Trust FAQ: https://github.com/github/customer-security-trust/blob/main/FAQ/FAQ.md
- NDA Procedures: https://github.com/github/support-squad-compliance/blob/main/docs/misc/nda%20procedures.md
- GitHub CELA NDA Guide: https://github.com/github/CELA/blob/main/Non-Disclosure%20Agreements%20(NDA).md

### External Resources

- GitHub Trust Portal: https://ghec.github.trust.page/
- GitHub Enterprise Cloud Documentation: https://docs.github.com/en/enterprise-cloud@latest/
- Data Residency Documentation: https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/

## Revision History

| Date | Version | Changes | Author |
|------|---------|---------|---------|
| 2025-06-27 | 1.0 | Initial creation of Compliance Category SOP covering ISO 27001, RTO/RPO, BCDR, Data Residency, Regulatory Compliance, and NDA procedures | GitHub Copilot |

---

**Document Status:** Active  
**Next Review Date:** 2025-09-27  
**Document Owner:** Support Squad Compliance Team

*This document is a work in progress and should be updated as processes and resources evolve. Please contribute improvements and feedback to ensure accuracy and usefulness for all Supportocats.*