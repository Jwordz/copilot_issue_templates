# Standard Operating Procedure: Compliance Category Ticket Resolution

## Purpose and Scope

This Standard Operating Procedure (SOP) provides step-by-step guidance for support staff (Supportocats) handling compliance-related customer inquiries and tickets. This document covers the most common compliance topics including ISO 27001 certificates, RTO/RPO, Business Continuity and Disaster Recovery (BCDR/BCP), Data Residency, Regulatory Compliance, SOC Reports, and NDA procedures.

**Applicable Systems:** GitHub Enterprise Cloud, GitHub Enterprise Server
**Applicable Teams:** Support, Customer Success
**Applicable Ticket Types:** Compliance requests, security documentation requests, audit support

## Trigger Events

This SOP should be initiated when encountering any of the following:

- Customer requests for ISO 27001 certificates or Statement of Applicability (SoA)
- Questions about Recovery Time Objective (RTO) or Recovery Point Objective (RPO)
- Business Continuity Plan (BCP) or Disaster Recovery (DR) documentation requests
- Data residency or data location inquiries
- PCI-DSS compliance documentation requests
- SOC 1, SOC 2, or SOC 3 report requests
- Requests requiring Non-Disclosure Agreement (NDA) execution
- General compliance or audit support questions
- Keywords in tickets: "compliance", "audit", "ISO", "SOC", "PCI", "BCDR", "RTO", "RPO", "data residency"

## Step-by-Step Resolution Process

### 1. Initial Assessment
1. **Identify the compliance topic** from the customer's request
2. **Determine customer account type** (Enterprise, Standard, EMU)
3. **Check if customer has existing NDA** (if confidential documents are needed)
4. **Review customer's urgency and timeline** for the request

### 2. ISO 27001 Certificate Requests

**What it is:** ISO 27001 is an international standard for information security management systems (ISMS) that provides a framework for organizations to manage and protect their information assets.

**Resolution Steps:**
1. Direct customer to self-serve options:
   - **Trust Portal:** [https://ghec.github.trust.page/](https://ghec.github.trust.page/)
   - **Enterprise Compliance Tab:** 
     - Profile photo → Your enterprise → Compliance → Resources section → ISO/IEC 27001:2013 certification
2. For Slack users, mention `.rem iso 27001` command for latest version link
3. Use prepared response: "Please find your latest ISO/IEC 27001 certification via your organisation settings, under the `Security` heading then choose `Compliance` or via our Trust Center found [here](https://ghec.github.trust.page/resources?s=3xojj6ga78m9tnarwcgzs6&name=iso/iec-27001-:-2022-certificate)."

### 3. RTO & RPO Inquiries

**What they are:**
- **RTO (Recovery Time Objective):** Maximum acceptable downtime before system must be restored
- **RPO (Recovery Point Objective):** Maximum acceptable data loss measured in time

**Resolution Steps:**
1. **For standard requests:** Use prepared response covering:
   - GitHub doesn't share specific RTO/RPO guarantees
   - Monthly availability reports published first Wednesday of each month
   - Enterprise Plan Uptime SLA reference
   - Customer backup options
2. **For detailed requests:** Provide additional technical details about:
   - Redundant production network edges (Ashburn, VA and Seattle, WA)
   - Real-time Git data replication between data centers
   - Backup procedures (archived backups, encrypted AWS backups, delayed replicas)
3. **Reference materials:**
   - [GitHub Availability Report](https://github.blog/tag/github-availability-report/)
   - [Enterprise Cloud uptime SLA](https://help.github.com/articles/github-enterprise-cloud-addendum/#enterprise-cloud-uptime-sla)
   - [Backing up a Repository](https://docs.github.com/en/repositories/archiving-a-github-repository/backing-up-a-repository/)

### 4. Business Continuity and Disaster Recovery (BCDR/BCP)

**Definitions:**
- **Business Continuity Plan (BCP):** Comprehensive plan ensuring entire organization can continue critical operations during/after disruption
- **Disaster Recovery (DR):** Subset of BCP focused on restoring IT systems, data, and infrastructure after disruption

**Resolution Steps:**
1. Direct customer to [Customer Security Trust FAQ](https://github.com/github/customer-security-trust/blob/main/FAQ/FAQ.md#business-continuity-and-disaster-recovery---bcdr-or-bcp)
2. **For customers on correct terms:** Share [GitHub.com Services Continuity and Incident Management Plan](https://github.com/github/customer-security-trust/blob/main/BCDR%20Plans/GitHub.com%20Services%20Continuity%20and%20Incident%20Management%20Plan%20(2).pdf)
3. Verify customer's terms allow document sharing before providing confidential materials

### 5. Data Residency Requests

**What it is:** Data residency refers to the physical or geographic location where an organization's data is stored or processed.

**Resolution Steps:**
1. **Standard response:** Use canned response about compliance reports complexity
2. **For specific regional requirements:** Inform about GitHub Enterprise Cloud with data residency (separate product)
3. **Key points to cover:**
   - Review [compliance reports for your enterprise](https://docs.github.com/en/enterprise-cloud@latest/admin/overview/accessing-compliance-reports-for-your-enterprise)
   - Data residency guarantee requires [GitHub Enterprise Cloud with data residency](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/about-github-enterprise-cloud-with-data-residency)
   - Reference [Getting started with data residency](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/getting-started-with-data-residency-for-github-enterprise-cloud)

**Note:** This doesn't apply to Proxima/GHEC-DR customers with geographically specific instances.

### 6. Regulatory Compliance (PCI-DSS)

**What it is:** Payment Card Industry Data Security Standard - security standard to protect credit card data.

**Resolution Steps:**
1. **For customers under NDA:** Share PCI-DSS AOC (Attestation of Compliance) from Customer Security Trust repo
2. **Slack command:** `.rem pci-dss` for latest version link
3. **For SRM requests:** Use `.rem pci-srm` for shared responsibility matrix
4. **Verify NDA status** before sharing confidential documents

### 7. SOC Reports

**Report Types:**
- **SOC 1:** Internal controls over financial reporting (ICFR)
- **SOC 2:** Security, availability, confidentiality, processing integrity, privacy controls
- **SOC 3:** Public summary of SOC 2 report

**Resolution Steps:**
1. **SOC 3 (Public):** Direct to [Trust Centre](https://ghec.github.trust.page/resources)
2. **SOC 1 & 2 (Confidential):**
   - **For EMU customers:** Organization owners can download from `Compliance` tab in organization settings
   - **For other customers:** Verify NDA status before sharing
3. **Slack commands:** `.rem SOC1`, `.rem SOC2`, `.rem SOC3`

### 8. NDA Procedures

**When NDA is required:** Before sharing non-public/confidential GitHub compliance documents.

**Resolution Steps:**
1. **Check existing NDA:** Use Microsoft's Contract Experience site
2. **For new NDA (Standard accounts):** Request customer information:
   - Name, title, and email of signatory
   - Company name and legal address
3. **For Enterprise customers:** Check if existing enterprise agreement covers compliance document sharing
4. **Reference materials:**
   - [NDA procedures](https://github.com/github/support-squad-compliance/blob/main/docs/misc/nda%20procedures.md)
   - [Guide on NDAs at GitHub](https://github.com/github/CELA/blob/main/Non-Disclosure%20Agreements%20(NDA).md)

## Escalation and Handoff

### Escalation Criteria
- Customer requires compliance documents not covered in this SOP
- Unusual or complex compliance requirements
- Legal questions about NDA terms or document sharing permissions
- Requests involving custom compliance frameworks not documented
- Time-sensitive audit deadlines requiring expedited processing

### Escalation Contacts
- **Primary:** Support Squad Compliance team
- **Legal questions:** GitHub CELA team via Slack
- **NDA processing:** Microsoft Global Contracting Office
- **Complex technical compliance:** Enterprise Engineering team

### Required Information for Escalation
- Customer organization and account type
- Specific compliance requirement or standard
- Requested documents or information
- Customer timeline/deadline
- Any existing NDAs or agreements
- Previous ticket history related to compliance

## Post-Resolution Actions

### Verification Steps
1. **Confirm document delivery** (if applicable)
2. **Verify customer can access** self-serve resources
3. **Check document completeness** against customer requirements
4. **Ensure NDA execution** (if confidential documents shared)

### Documentation Requirements
1. **Update ticket with resolution details**
2. **Note any new compliance questions** for knowledge base updates
3. **Document any process improvements** discovered during resolution
4. **Record customer feedback** on document usefulness

### Communication Requirements
1. **Send follow-up message** confirming resolution
2. **Provide additional resource links** if helpful
3. **Set expectation for future compliance requests**
4. **Notify customer of regular availability report schedule** (if applicable)

## Best Practices and Troubleshooting Tips

### Common Pitfalls and Solutions

**Pitfall:** Sharing confidential documents without NDA verification
**Solution:** Always verify NDA status before sharing SOC 1/2, PCI-DSS AOC, or internal compliance documents

**Pitfall:** Providing specific RTO/RPO guarantees
**Solution:** Use prepared responses that reference SLAs and availability reports without specific guarantees

**Pitfall:** Confusion between BCP and DR
**Solution:** Use clear definitions and explain the relationship between business continuity and disaster recovery

**Pitfall:** Promising data residency without understanding product limitations
**Solution:** Clearly distinguish between standard GitHub Enterprise Cloud and data residency product

### Troubleshooting Tips

1. **Customer can't find compliance documents:**
   - Verify their account type and permissions
   - Check if they're looking in the correct enterprise/organization
   - Provide step-by-step navigation instructions

2. **Customer disputes compliance information:**
   - Reference official documentation and FAQ
   - Escalate to compliance team for verification
   - Avoid making commitments outside documented capabilities

3. **Urgent audit deadlines:**
   - Prioritize ticket appropriately
   - Identify fastest resolution path (self-serve vs. document sharing)
   - Escalate if expedited NDA processing needed

### Related Resources
- [Customer Security Trust FAQ](https://github.com/github/customer-security-trust/blob/main/FAQ/FAQ.md)
- [GitHub Trust Portal](https://ghec.github.trust.page/)
- [Enterprise compliance documentation](https://docs.github.com/en/enterprise-cloud@latest/admin/overview/accessing-compliance-reports-for-your-enterprise)
- Monthly GitHub Availability Reports
- GitHub Online Services SLA

## Prepared Customer Responses

### ISO Request
```
Please find your latest ISO/IEC 27001 certification via your organisation settings, under the `Security` heading then choose `Compliance` or via our Trust Center found [here](https://ghec.github.trust.page/resources?s=3xojj6ga78m9tnarwcgzs6&name=iso/iec-27001-:-2022-certificate).

Please let me know if you have any other questions.
```

### RTO/RPO (Standard)
```
While we are not at a place where we share or guarantee specific RTO, RPO, we do publish monthly availability reports. On the first Wednesday of each month, we publish a report describing GitHub's availability, including a description of any incidents that may have occurred for the previous month and update you on how we are evolving our engineering systems and practices in response. You should expect these updates to include a summary of what happened, as well as a technical explanation for incidents where we believe the occurrence was novel and contains information that helps engineers around the world learn how to improve product operations at scale. These reports can be found [Github Availability Report](https://github.blog/tag/github-availability-report/). Additionally, GitHub's Enterprise Plan provides an Uptime SLA which can be reviewed here: [Enterprise Cloud uptime SLA](https://help.github.com/articles/github-enterprise-cloud-addendum/#enterprise-cloud-uptime-sla).

If RTO and RPO are concerns you can also create backups of your own data. GitHub provides information on how customers may backup their own data as a safeguard. See the below GitHub Help article for further context and instructions [Backing up a Repository](https://docs.github.com/en/repositories/archiving-a-github-repository/backing-up-a-repository/).

Please let me know if you have any further questions.
```

### Data Residency
```
Details about how our data is stored and compliance for audit reports are complex (because they involve multiple sites and partners) and subject to change, so my recommendation is to review the [compliance reports for your enterprise](https://docs.github.com/en/enterprise-cloud@latest/admin/overview/accessing-compliance-reports-for-your-enterprise) which cover the details you need for many common audits.

If you need to guarantee data residency in a specific region, we do offer [GitHub Enterprise Cloud with data residency](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/about-github-enterprise-cloud-with-data-residency) which is a separate product and something that you would need to migrate to. If you're interested in this, you can find more information in "[Getting started with data residency for GitHub Enterprise Cloud](https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/getting-started-with-data-residency-for-github-enterprise-cloud)" and let me know if you have any questions.
```

### NDA Request (Standard Account)
```
We will need additional information to process the NDA, please provide the following:

1. Name, title, and email address of the individual at your company who will be the signatory of any NDA.
2. Company's name and legal address.

If we receive that information we can begin the process to generate an NDA for your signature.
```

### SOC 1 or 2 Request (EMU)
```
Any organization owner can download our most recent SOC 1 & SOC 2 reports from the `Compliance` tab in their organization settings.
```

## Revision History

| Date | Version | Changes | Author |
|------|---------|---------|---------|
| 2025-06-27 | 1.0 | Initial creation of Compliance Category SOP covering ISO 27001, RTO/RPO, BCDR/BCP, Data Residency, Regulatory Compliance, SOC Reports, and NDA procedures | Support Documentation Team |