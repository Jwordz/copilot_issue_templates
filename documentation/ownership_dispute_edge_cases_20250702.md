# Standard Operating Procedure: Ownership Dispute Edge Cases

## Purpose and Scope

This Standard Operating Procedure (SOP) provides step-by-step guidance for support staff (Supportocats) handling ownership dispute edge cases and complex account ownership scenarios. This document covers user account disputes, organization account ownership transfers, account transformation scenarios, and legal review processes for both Standard Terms of Service (SToS) and Corporate Terms of Service (CToS) accounts.

**Applicable Systems:** GitHub.com, GitHub Enterprise Cloud, GitHub Enterprise Server
**Applicable Teams:** Support, Compliance Support, Legal Support
**Applicable Ticket Types:** Account ownership disputes, organization access requests, account transformation issues, deleted organization disputes

## Trigger Events

This SOP should be initiated when encountering any of the following:

- User requests access to or ownership of someone else's user account
- Contact claims ownership of an organization they cannot access
- Former employee disputes over organization account ownership
- Account transformation scenarios (user account converted to organization)
- Organization deleted during ownership dispute
- Requests for organization ownership transfer due to unreachable owners
- Corporate entity claiming ownership of organization account
- Trademark disputes related to account usernames
- Keywords in tickets: "ownership dispute", "account access", "organization transfer", "former employee", "account takeover", "trademark"

## Step-by-Step Resolution Process

### 1. Initial Assessment and Account Identification

**Identification Steps:**
1. **Determine the account in question** - Contact may provide username, organization name, or be confused about which account
2. **Clarify account type** - User account vs. Organization account
3. **Verify contact identity** - Confirm who is making the request and their relationship to the account
4. **Check Terms of Service** - Determine if organization is on SToS or CToS
5. **Review account history** - Check for any account transformations, deletions, or ownership changes

**Key Questions to Ask:**
- What is the exact username or organization name in question?
- What is your relationship to this account?
- Are you a current or former employee of the company?
- Do you have any billing information or credit card details associated with this account?

### 2. Determine Information Sharing Eligibility

**Information Sharing Rules:**
- Follow [Requirements for sharing information](https://thehub.github.com/support/compliance/general/what-can-i-share/) guidelines
- When in doubt, consult with fellow Supportocats
- Some grey areas exist regarding benefit of the doubt

**Shareable Information (when requirements are met):**
- Organization owner usernames
- Organization name confirmation
- General account status (active/deleted)

**Non-Shareable Information:**
- Email addresses on accounts
- Personal account details
- Specific account activity

### 3. User Account Disputes

**Important Note:** This differs from Account Takeovers where someone claims their own account was compromised.

**Resolution Approach:**
1. **Default Response:** We attribute ownership to the individual on the account rather than the company
2. **Standard Resolution:** Direct contact to reach out to the original account owner directly
3. **No Direct Access:** Do not help contacts gain access to someone else's user account, even with work email addresses

**Canned Response for User Account Disputes:**
```
As this is a user account, we attribute ownership to the individual on that account rather than to the company they are (or have been) a part of. In this instance, the best method to gain control of that account would be to identify and reach out to the original account owner and ask them to reach out about converting their account to an organization account so they can add you, to release the username or to ask them to transfer any repositories your way.

Should there be any trouble with their own access to the account, if they could reach out to us themselves, we could then assist them with the steps needed to recover access. For privacy reasons, we are not able to share any details about the account or the email address on the account.
```

#### 3.1 Trademark Dispute Option (Occasional)

**When Applicable:**
- User account appears to use an organization name as username
- Contact represents that organization
- Likelihood of other methods working is low
- Request is for username (not account content)

**Canned Response Inclusion:**
```
In case it helps, it's worth mentioning that we have a trademark policy that could allow you to obtain a username that's already been claimed. If the username you're interested in is a trademark you hold, I'd recommend taking a look at that policy for more information about potentially filing a violation report:

https://docs.github.com/en/github/site-policy/github-trademark-policy
```

#### 3.2 Message Relay (Rare)

**Criteria for Message Relay:**
- Clear indication that account holder works/worked for the company
- Contact unable to identify or reach account holder
- Account should probably have been set up as organization (username = company name, generic company email)
- Use as second-to-last resort

**Canned Response for Message Relay Offer:**
```
If you'd like to send a polite message to the owner of the `USERNAME` account asking them to rename the account so you could have the username, or to convert the account to an organization account and transfer ownership to you, we would be happy to send it on your behalf just this one time. They might be willing to assist or they might not and they're under no obligation to even respond to the request.

If that sounds good, please reply with the exact message you'd like us to pass along. Please be sure to identify yourself in a way they'll be able to recognise and to provide your preferred contact details for us to share.
```

#### 3.3 Legal Review (Even Rarer)

**When Required:** If above options fail and contact persists in claiming ownership
**Requirement:** Court order regarding account ownership
**Process:** Review by @github/legal-support

### 4. Organization Account Disputes

#### 4.1 Organizations on Standard Terms of Service (SToS)

**Key Principle:** Organization accounts on SToS belong to the owner(s), not the company they work for.

**Available Resolution Avenues:**
1. **Provide Owner Usernames** (Conditional)
2. **Relay Message** (Primary approach)
3. **Legal Review** (Rare - requires evidence that org should have been on CToS)

##### 4.1.1 Providing Owner Usernames

**When Allowed:** If [requirements for sharing information](https://thehub.github.com/support/compliance/general/what-can-i-share/) are met

**Canned Response Inclusion:**
```
Currently, the `ORGNAME` has the following owner(s) who can add you:

```
Owner username - Profile name
Owner username - Profile name
```
```

##### 4.1.2 Message Relay Process

**Canned Response for Offering Message Relay:**
```
Only one of the current owners of the `ORGNAME` organization account would be able to transfer ownership or add new owners to the organization, even if they have since left the company. I'm afraid we're not able to change organization ownership or access on your behalf.

If you're unable to identify or contact any of the owners directly, we can relay a message on your behalf. If that sounds good, please reply with the exact message you'd like us to pass along. Please be sure to identify yourself in a way they'll be able to recognise and to provide your preferred contact details for us to share.
```

**Macro:** `CannedReplies::support delivery::Compliance::takeovers and disputes::org account dispute relay message`

#### 4.2 Organizations on Corporate Terms of Service (CToS)

**Key Principle:** Organization accounts on CToS belong to the business/institution, not individual owners.

**Available Resolution Avenues:**
1. **Provide Owner Usernames** (Conditional)
2. **Relay Message** (Primary approach)
3. **Legal Review Supported Transfer** (Secondary option)

##### 4.2.1 Legal Review Supported Transfer

**Eligibility:** Authorized Representative of the company can prove their status
**Process:** Legal team assistance required

**Required Documentation:**
- Current corporate registration or licensing documentation:
  - Articles of Organization (LLC)
  - Articles of Incorporation (Inc.)
- Licensed attorney clearly representing the company
- Link to company website showing position details
- Internal documentation or public registration demonstrating authorized representative status

**Canned Response for Documentation Request:**
```
We would need someone from the corporate exec team, founders, general counsel, or anyone that can provide the documentation listed below to reach out to us:

- Current corporate registration or licensing documentation:
  - Articles of Organization (LLC)
  - Articles of Incorporation (Inc.)

- A licensed attorney who has clearly stated that they are representing the company

- A link to the company's website where we can find details about their position at the company

- Internal documentation or a public registration (e.g. business license), which demonstrates that they are an authorized representative of the company.

If you are unable to provide such documentation, you could either CC the appropriate person into this ticket so they can reply here, or they can simply create their own ticket just as you did, and get them to mention this ticket number (#TICKETNUMBER):

https://support.github.com/contact/account
```

##### 4.2.2 Bug - Incorrect Terms of Service Display

**Issue:** Organizations created during a period where CToS was not properly displayed
**Identification:** Shows "Standard Terms of Service through <COMPANY/ENTITY NAME>"
**Treatment:** Consider as CToS organization due to bug

### 5. Message Relay Process

#### 5.1 Executing Message Relay

**Process:**
1. **Forward message** to ALL verified email addresses on ALL owner accounts
2. **Use judgment** for excessive number of emails (set reasonable limit)
3. **Use macro:** `CannedReplies::support delivery::Compliance::takeovers and disputes::org account dispute relay message`

#### 5.2 Post Relay Confirmation

**Canned Response:**
```
Hi there,

Thanks for sending that through. 

I have just forwarded that message to the owners of the `ORGNAME` organization. Hopefully, they will reach out to you about this.

If they reply to our email, I will be sure to pass on any relevant updates.
```

### 6. Legal Review Process

#### 6.1 Initiating Legal Review

**Process:**
1. **Use macro:** `Request Legal-Support Review (Accounts Support)`
2. **Status update:** Ticket will be updated to `On-Hold`

**Confirmation Response:**
```
Thanks for sending that through.

I have now sent this off for review by our legal team. From here they will verify the information and let us know how to proceed.

We will be in touch again as soon as we hear back from them. Unfortunately, I am not able to provide a timeframe but rest assured that you'll hear from me when they get back with anything at all.
```

#### 6.2 Successful Legal Review

**Requirements:**
1. **Form completion:** [GitHub Corporate ToS admin transfer form](https://github.com/github/support-squad-compliance/blob/main/docs/account-ownership/GitHub-Corporate-ToS-admin-transfer.pdf)
2. **Reference:** [Form cheat sheet](https://github.com/github/support-squad-compliance/blob/main/docs/account-ownership/CToS%20transfer%20form%20CHEAT%20SHEET.png)

**Canned Response for Successful Review:**
```
Our legal team have finished their review and I'm happy to say we can now move forward with the ownership transfer. To do this, there are two steps we will need from you:

- Firstly, we'll need you to designate (or create) an account to be made the new owner. If you intend to use the existing `USERNAME` account that is already linked with this email address, we'll just need you to let us know.

- We'll also need you to fill out our Corporate Terms of Service transfer form which I've attached to this reply.

Once we have that form returned, and the correct account nominated, we can assign ownership of the `ORGNAME` organization to the designated account. That account will then have full administrative access to make any necessary changes.

Please let us know, and do ask any other questions you may still have on this.
```

### 7. Edge Case Scenarios

#### 7.1 Organization Username Request Disguised as Ownership Dispute

**Scenario:** User claims to have set up or own an organization with no actual connection
**Resolution:** Treat as username request rather than ownership dispute
**Assessment:** Review account history to determine actual relationship

#### 7.2 Dispute of Deleted Organization

**Immediate Action:** Place legal hold on deleted organization to preserve data

**Investigation Steps:**
1. **Search audit log** for `org.update_terms_of_service` events
2. **Check `terms_of_service_type` attribute** in most recent occurrence
3. **Determine original ToS type** (Standard vs Corporate)
4. **Proceed based on original ToS type**

**Example Audit Log Values:**
```
new_value: Corporate
old_value: Standard
```

#### 7.3 Account Transformation Edge Case

**Scenario:** Personal user account transformed to organization, original user loses access

**Events Leading to Issue:**
1. Personal user account transformed to organization
2. Different user made organization owner
3. Organization owner deletes organization
4. Original user cannot access account (404 error)
5. Email address becomes available for reuse

**Resolution Approach:**
1. **Explain the events** that led to current situation
2. **Identify required actions:**
   - Organization owner must request restoration
   - Organization owner must transfer ownership back
3. **Privacy constraints:** Cannot name current organization owner
4. **Offer message relay** if direct contact not possible

**Canned Response for Account Transformation Cases:**
```
[Detail events that led to this] followed by:

Only one of the current owners of the `[org name]` organization account would be able to request restoration of the org and then transfer ownership or add new owners to the organization. I'm afraid we're not able to change organization ownership or access on your behalf.

If you are able to reach out to them and should there be any trouble with their own access to the account, they should reach out to us themselves and we could then assist them with the steps needed to recover access, if possible.

For privacy reasons, we are unable to share the details of the current owners. 

However, if you're unable to identify or contact the owners directly, we can relay a message on your behalf. If that sounds good, please reply with the exact message you'd like us to pass along. Please be sure to identify yourself in a way they'll be able to recognise and to provide your preferred contact details for us to share.
```

## Escalation and Handoff

### Escalation Criteria

- Complex legal questions requiring specialized review
- Court orders or legal documentation requiring verification
- Cross-jurisdictional disputes involving international entities
- Cases involving potential trademark infringement
- Disputes requiring expedited processing due to business impact
- Technical account issues during transformation or recovery
- Situations requiring data preservation or legal holds

### Escalation Contacts

- **Primary:** Support Squad Compliance team
- **Legal questions:** @github/legal-support
- **Complex account technical issues:** Enterprise Engineering team
- **Trademark disputes:** GitHub CELA team
- **International legal matters:** Microsoft Global Legal team

### Required Information for Escalation

- Complete account and organization details
- Chronological summary of events leading to dispute
- All documentation provided by requestor
- Previous related tickets or interactions
- Current account status and ownership details
- Business impact and urgency assessment
- Any legal documents or court orders involved

## Post-Resolution Actions

### Verification Steps

1. **Confirm resolution method** implemented successfully
2. **Verify new ownership** has appropriate access
3. **Check account functionality** post-transfer
4. **Ensure proper documentation** of resolution in ticket
5. **Validate no secondary issues** created by resolution

### Documentation Requirements

1. **Complete ticket documentation** with full resolution details
2. **Update internal knowledge base** with new edge cases
3. **Document any process improvements** discovered
4. **Record legal review outcomes** for future reference
5. **Note any policy clarifications** needed

### Communication Requirements

1. **Final confirmation** to all involved parties
2. **Summary of resolution** and next steps
3. **Contact information** for future issues
4. **Documentation links** for self-service options
5. **Follow-up schedule** if monitoring required

## Best Practices and Troubleshooting Tips

### Common Pitfalls and Solutions

**Pitfall:** Sharing account information without proper verification
**Solution:** Always follow information sharing guidelines and verify requirements are met

**Pitfall:** Promising account transfers without legal review
**Solution:** Clearly explain the process and requirements upfront

**Pitfall:** Confusing SToS and CToS resolution paths
**Solution:** Always verify Terms of Service type before offering resolution options

**Pitfall:** Providing access to accounts without proper authorization
**Solution:** Maintain strict verification requirements regardless of urgency

**Pitfall:** Overlooking account transformation scenarios
**Solution:** Always check audit logs for account history and transformations

### Troubleshooting Tips

1. **Contact claims ownership but has no proof:**
   - Guide through available verification methods
   - Explain documentation requirements clearly
   - Offer alternative resolution paths

2. **Organization owners are unresponsive:**
   - Attempt message relay process
   - Consider escalation for business-critical cases
   - Document all contact attempts

3. **Legal documentation is incomplete:**
   - Provide specific requirements checklist
   - Offer examples of acceptable documentation
   - Connect with legal team for clarification

4. **Urgent business deadlines:**
   - Assess true urgency and business impact
   - Escalate appropriately while maintaining security
   - Provide clear timeline expectations

5. **Complex account transformation history:**
   - Use audit logs to trace account evolution
   - Involve technical teams for complex scenarios
   - Document findings for future reference

### Related Resources

- [Requirements for sharing information](https://thehub.github.com/support/compliance/general/what-can-i-share/)
- [Supporting account takeover tickets](https://thehub.github.com/support/compliance/account-takeovers/supporting-account-takeover-tickets/)
- [GitHub Trademark Policy](https://docs.github.com/en/github/site-policy/github-trademark-policy)
- [Message Relay Process](https://thehub.github.com/support/compliance/general/message-relay-process/)
- [GitHub Corporate ToS admin transfer form](https://github.com/github/support-squad-compliance/blob/main/docs/account-ownership/GitHub-Corporate-ToS-admin-transfer.pdf)
- [NDA procedures](https://github.com/github/support-squad-compliance/blob/main/docs/misc/nda%20procedures.md)

## Revision History

| Date | Version | Changes | Author |
|------|---------|---------|------------|
| 2025-07-02 | 1.0 | Initial creation of Ownership Dispute Edge Cases SOP covering user account disputes, organization ownership transfers, account transformations, legal review processes, and complex edge cases | Support Documentation Team |