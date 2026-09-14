# Error Experience Matrix
## [Project Name]

**Document Owner:** Design  
**Last Updated:** [Date]  
**Version:** [Version]  
**Audience:** Design, Technology, Product, Content

---

## Overview

This matrix maps every possible outcome (success and failure) to:
1. **UI State:** Which state the user experiences
2. **User Message:** What they see
3. **Recovery Action:** What they can do next
4. **HTTP Status & Error Code:** What the API returns
5. **Design Notes:** Tone, emphasis, when to show support

---

## The 5 UI States

| State | Meaning | Duration | User Sees |
|-------|---------|----------|-----------|
| **1. Idle / Pre-Action** | System ready, user reviewing | N/A | [Form/interface ready] |
| **2. Processing** | Action in flight | [Duration] | [Loading state, spinner] |
| **3. Success (2xx)** | Happy path | Permanent | [Success message, next steps] |
| **4. User Recovery (4xx)** | User can fix (bad input, limit) | Permanent until fixed | [Specific error + guidance] |
| **5. System Refusal (5xx/Blocked)** | User cannot fix | Permanent until support | [Empathetic message + support] |

---

## Success Path

### Outcome: [Success Scenario]

| Attribute | Value |
|-----------|-------|
| **Scenario** | [When does this happen?] |
| **UI State** | State [#]: [Name] |
| **HTTP Status** | [200/202/etc] |
| **Duration** | [How long?] |
| **User Sees** | [Icon + message] |
| **Primary Message** | [Main text] |
| **Supporting Details** | [Additional info] |
| **Next Step** | [Primary CTA] / [Secondary CTA] |
| **Tone** | [Warm/professional/casual] |
| **Design Notes** | [Visual guidance] |
| **Copy Emphasis** | [What to highlight?] |
| **Accessibility** | [Screen reader guidance] |

---

## Failure Paths

### Failure Category 1: User Recovery (State 4)

---

#### Outcome: [Failure Type 1]

| Attribute | Value |
|-----------|-------|
| **Scenario** | [When/why does this happen?] |
| **UI State** | State 4: User Recovery |
| **HTTP Status** | [Code] |
| **Duration** | [Temporary/permanent] |
| **User Sees** | [Icon + message] |
| **Primary Message** | [Main text] |
| **Supporting Details** | [Additional info] |
| **Recovery Options** | [Option 1], [Option 2] |
| **Tone** | [Helpful/non-judgmental] |
| **Design Notes** | [Visual guidance] |
| **Copy Emphasis** | [What to clarify] |
| **Accessibility** | [Screen reader guidance] |
| **Support Link?** | [Yes/No] |

#### Outcome: [Failure Type 2]
[Repeat above structure]

---

### Failure Category 2: System Refusal (State 5)

---

#### Outcome: [Failure Type 1]

| Attribute | Value |
|-----------|-------|
| **Scenario** | [When/why does this happen?] |
| **UI State** | State 5: System Refusal |
| **HTTP Status** | [Code] |
| **Duration** | [Temporary/permanent] |
| **User Sees** | [Icon + message] |
| **Primary Message** | [Main text] |
| **Supporting Details** | [Additional info] |
| **Recovery Option** | [What can they do?] / [Support link] |
| **Tone** | [Apologetic/firm] |
| **Design Notes** | [Visual guidance] |
| **Copy Emphasis** | [What to clarify] |
| **Accessibility** | [Screen reader guidance] |
| **Support Link?** | Yes |

---

## Cross-Touchpoint Consistency

| Touchpoint | Failure Type 1 | Failure Type 2 | Failure Type 3 |
|------------|----------------|----------------|----------------|
| **Web** | [Response] | [Response] | [Response] |
| **Mobile App** | [Response] | [Response] | [Response] |
| **Mobile Web** | [Response] | [Response] | [Response] |
| **API** | [Response] | [Response] | [Response] |
| **[Other]** | [Response] | [Response] | [Response] |

**Consistency Rule:** [State what must be identical across all touchpoints]

---

## Copy Guidelines by Category

### Success Messages
- **Tone:** [Describe]
- **Avoid:** [What not to do]
- **Do:** [What to do]
- **Example:** "[Example message]"

### User Recovery Messages
- **Tone:** [Describe]
- **Avoid:** [What not to do]
- **Do:** [What to do]
- **Example:** "[Example message]"

### System Refusal Messages
- **Tone:** [Describe]
- **Avoid:** [What not to do]
- **Do:** [What to do]
- **Example:** "[Example message]"

---

## Accessibility Checklist

- [ ] Every error has both icon AND text (not icon alone)
- [ ] Form field errors use aria-describedby
- [ ] Status messages are announced (aria-live)
- [ ] Links and buttons are keyboard-navigable
- [ ] Color is never the only indicator
- [ ] [Custom item]
- [ ] [Custom item]

---

## Sign-Off

| Role | Name | Date | Approval |
|------|------|------|----------|
| Design | [Name] | [Date] | ☐ |
| Product | [Name] | [Date] | ☐ |
| Technology | [Name] | [Date] | ☐ |

---

## Document Control

**Version History:**
| Version | Date | Author | Change |
|---------|------|--------|--------|
| 1.0 | [Date] | Design | Initial error matrix from Product Requirements |
