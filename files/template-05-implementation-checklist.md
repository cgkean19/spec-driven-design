# Implementation Checklist
## [Project Name]

**Document Owner:** Technology  
**Last Updated:** [Date]  
**Version:** [Version]  
**Audience:** Engineering, QA, Design (for validation), Product

---

## Overview

This checklist ensures every line of the Shared Specification has been implemented and tested.

---

## Phase 1: [Feature/Component Name]

### 1.1 [Endpoint/Feature Name]

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] [Requirement 1]
- [ ] [Requirement 2]
- [ ] [Requirement 3]

**Test Cases:**
- [ ] [Test 1: Input → Expected Output]
- [ ] [Test 2: Edge case]
- [ ] [Test 3: Error scenario]

---

### 1.2 [Validation/Logic]

**Implemented?** ☐  
**QA Tested?** ☐

**Rules:**
- [ ] [Rule 1]
- [ ] [Rule 2]

**Edge Cases:**
- [ ] [Edge case 1]
- [ ] [Edge case 2]

---

## Phase 2: [Response Handling]

### 2.1 Success Response (HTTP 200)

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] [Requirement 1]
- [ ] [Requirement 2]

**Validation:**
- [ ] [Validation check 1]
- [ ] [Validation check 2]

---

### 2.2 Error Response (HTTP 4xx/5xx)

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] [Error type 1]: [Requirements]
- [ ] [Error type 2]: [Requirements]

**Test Case:**
```
[Test scenario]
→ [Expected response]
```

---

## Phase 3: [State Machine / Business Logic]

### 3.1 State Transitions

**Implemented?** ☐  
**QA Tested?** ☐

**Valid Transitions:**
- [ ] [State A → State B]
- [ ] [State B → State C]

**Invalid Transitions (must NOT happen):**
- [ ] [Invalid transition 1]
- [ ] [Invalid transition 2]

---

## Phase 4: [Observability]

### 4.1 Event Emission

**Implemented?** ☐  
**QA Tested?** ☐

**Events:**
- [ ] event.name with fields: [field1, field2, field3]
- [ ] event.name_2 with fields: [field1, field2]

**Event Format:**
- [ ] Consistent schema
- [ ] Includes timestamp (ISO 8601)
- [ ] Includes request_id

---

### 4.2 Metrics Dashboards

**Implemented?** ☐  
**QA Tested?** ☐

**Business Metrics:**
- [ ] [Metric 1] - updated [frequency]
- [ ] [Metric 2] - alert if [condition]

**Operational Metrics:**
- [ ] [Metric 1] - target [value]
- [ ] [Metric 2] - alert if [condition]

---

## Phase 5: [Security]

### 5.1 Authentication

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] Requires valid credentials
- [ ] Returns 401 if invalid
- [ ] Returns 403 if unauthorised

---

### 5.2 Data Handling

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] No sensitive data in error messages
- [ ] No stack traces in responses
- [ ] No internal system details exposed

---

## Phase 6: [Cross-Touchpoint Consistency]

### 6.1 Consistency Across Channels

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] Web and Mobile get same HTTP status
- [ ] Web and API get same error codes
- [ ] All touchpoints return RFC 7807 format

**Test Case:**
- [ ] Send same request from web → Get response X
- [ ] Send same request from mobile → Get response X (identical)
- [ ] Send same request via API → Get response X (identical)

---

## Phase 7: [Rollout]

### 7.1 Canary Deployment

**Implemented?** ☐  
**QA Tested?** ☐

- [ ] Feature flags allow traffic routing
- [ ] Metrics collected for new version (distinct tags)
- [ ] Fallback to old system if new system fails
- [ ] Rollback criteria defined and automated

---

## Final Sign-Off

| Item | Owner | Status |
|------|-------|--------|
| All endpoints implemented per spec | Tech | ☐ |
| All error responses in correct format | Tech | ☐ |
| QA test cases completed | QA | ☐ |
| Design validates against spec | Design | ☐ |
| Security review completed | Security | ☐ |
| Canary deployment successful | DevOps | ☐ |

---

## Sign-Off

| Role | Name | Date | Approval |
|------|------|------|----------|
| Engineering Lead | [Name] | [Date] | ☐ |
| QA Lead | [Name] | [Date] | ☐ |
| Design Lead | [Name] | [Date] | ☐ |
| Product Lead | [Name] | [Date] | ☐ |

---

## Document Control

**Version History:**
| Version | Date | Author | Change |
|---------|------|--------|--------|
| 1.0 | [Date] | Tech | Initial implementation checklist from Shared Spec |
