# Shared Specification
## [Project Name]

**Document Owner:** Technology + Design (collaborative)  
**Last Updated:** [Date]  
**Version:** [Version]  
**Audience:** Technology, Design, Product, API Consumers

---

## Overview

This is the formal contract between frontend and backend.

---

## API Endpoints

### Endpoint 1: [HTTP METHOD] [/path]

**Purpose:** [What does this endpoint do?]  
**Access:** [Who can call it?]  
**Idempotency:** [Yes/No]

#### Request

**Method:** [GET/POST/PUT/PATCH/DELETE]  
**Path:** [/path/{id}]  
**Headers:**
```
[Header 1]: [Value]
[Header 2]: [Value]
```

**Body Schema:**
```json
{
  "field_1": {
    "type": "[type]",
    "description": "[What is this?]"
  },
  "field_2": {
    "type": "[type]",
    "description": "[What is this?]"
  }
}
```

**Validation Rules:**
- [Rule 1]
- [Rule 2]
- [Rule 3]

---

#### Response: Success (HTTP 200)

**Headers:**
```
Content-Type: application/json
```

**Body Schema:**
```json
{
  "field_1": { "type": "[type]", "description": "[What is this?]" },
  "field_2": { "type": "[type]", "description": "[What is this?]" }
}
```

---

#### Response: Accepted (HTTP 202)

[Structure for async/pending operations]

---

#### Response: Error (HTTP 4xx/5xx)

**Scenario:** [When does this happen?]  
**Headers:**
```
Content-Type: application/problem+json
```

**Body Schema (RFC 7807):**
```json
{
  "type": { "type": "string" },
  "title": { "type": "string" },
  "detail": { "type": "string" },
  "status": { "type": "integer" },
  "instance": { "type": "string" }
}
```

---

### Endpoint 2: [METHOD] [/path]

[Repeat structure above]

---

## State Machine

[ASCII diagram or description of valid state transitions]

```
[Initial State]
  |
  +-- [State A]
  |     |
  |     +-- [Terminal State 1]
  |
  +-- [State B]
        |
        +-- [Terminal State 2]
```

**State Definitions:**

| State | Meaning | User-Facing | Duration | Can Retry? |
|-------|---------|------------|----------|-----------|
| [State] | [Meaning] | [Yes/No] | [Time] | [Yes/No] |

---

## Error Response Codes Reference

| HTTP Status | Title | Reason | User Action |
|------------|-------|--------|-------------|
| [Code] | [Title] | [Reason] | [Action] |

---

## Idempotency

**Rule:** [What makes a request idempotent?]  
**Behavior:** [What happens if same key is sent twice?]  
**Use Case:** [When/why would client use this?]

---

## Observability & Metrics

**Events that must be emitted:**

```
event.name
  - field_1, field_2, field_3, timestamp

event.name_2
  - field_1, field_2, field_3, timestamp
```

---

## Design Validation Checklist

Technology implements, Design validates:

- [ ] [Item 1]
- [ ] [Item 2]
- [ ] [Item 3]

---

## Sign-Off

| Role | Name | Date | Approval |
|------|------|------|----------|
| Technology | [Name] | [Date] | ☐ |
| Design | [Name] | [Date] | ☐ |
| Product | [Name] | [Date] | ☐ |

---

## Document Control

**Version History:**
| Version | Date | Author | Change |
|---------|------|--------|--------|
| 1.0 | [Date] | Tech + Design | Initial shared specification |
