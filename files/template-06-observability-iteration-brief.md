# Observability & Iteration Brief
## [Project Name]

**Document Owner:** Product + Technology  
**Last Updated:** [Date]  
**Version:** [Version]  
**Audience:** Business, Product, Design, Technology, Finance

---

## Overview

This defines:
1. **What we measure** (metrics that matter to each role)
2. **How we measure it** (queries, dashboards, frequency)
3. **When we act** (thresholds that trigger investigation or change)
4. **How we iterate** (data-driven process for improving)

---

## Tier 1: Business Metrics (Business + Product Own)

### 1.1 [Key Metric Name]

**What It Means:** [Plain English explanation]

**Why It Matters:** [Business impact]

**How to Measure:**
```sql
[Sample query]
```

**Dashboard:**
- [Visual type]: [What it shows]
- [Update frequency]

**Frequency:** [Daily/Weekly/Real-time]

**Alert Triggers:**
- [Condition 1] → Do [action]
- [Condition 2] → Do [action]

**Who Investigates:** [Role]

**What We Do:** [Iteration steps]

---

### 1.2 [Metric 2]

[Repeat structure above]

---

## Tier 2: Operational Metrics (Tech + Product Own)

### 2.1 [Metric Name]

**What It Means:** [Explanation]

**Why It Matters:** [Why care]

**How to Measure:**
```sql
[Query]
```

**Dashboard:**
- [Visualization]
- [Target/alert lines]

**Frequency:** [Update cadence]

**Alert Triggers:**
- [Condition] → Investigate [what]

**Who Investigates:** [Role]

---

### 2.2 [Metric 2]

[Repeat]

---

## Tier 3: Design Metrics (Design + Product Own)

### 3.1 [Metric Name: e.g., "Error Recovery Rate"]

**What It Means:** [Explanation]

**Why It Matters:** [Impact]

**How to Measure:**
```sql
[Query]
```

**Dashboard:**
- [Visualization by error type]
- [Recovery targets]

**Frequency:** [Daily/Weekly]

**Alert Triggers:**
- [Recovery rate drops by X%] → Investigate UX

---

## Iteration Framework

### Phase 1: Weekly Standup (Frequency)

**Attendees:** [Roles]  
**Duration:** [Time]

**Agenda:**
1. Review Tier 1 metrics (trends? Issues?)
2. Review Tier 2 operational health
3. Any alerts from last week?
4. Themes emerging?

**Outcome:**
- Decide if action needed
- Assign owners for follow-up

---

### Phase 2: Bi-Weekly Deep Dive (Frequency)

**Attendees:** [Roles]  
**Focus:** One emerging issue

**Process:**
1. Define the problem (data)
2. Investigate root cause (by role)
3. Identify solution
4. Plan rollout
5. Set monitoring

---

### Phase 3: Monthly Policy Review (Frequency)

**Attendees:** [Roles]  
**Agenda:**
1. Key metric trending vs. target?
2. Any new patterns?
3. Are policies still working?
4. Do we need to change anything?

**Decisions Made:**
- Policy/rule adjustments
- Staffing/capacity changes
- Feature prioritisation

---

## Dashboard Topology

### View 1: [Audience] Scorecard

**Metrics:**
- [Metric 1]
- [Metric 2]
- [Metric 3]

**Update:** [Frequency]  
**Audience:** [Roles]

---

### View 2: [Audience] Operations

**Metrics:**
- [Metric 1]
- [Metric 2]
- [Metric 3]

**Update:** [Frequency]  
**Audience:** [Roles]

---

## When to Escalate

### Severity 1 (Immediate Action)
- [Condition 1: e.g., "Service down"]
- [Condition 2: e.g., "Error rate > X%"]

**Response:** [What to do]

### Severity 2 (Same Day)
- [Condition 1]
- [Condition 2]

**Response:** [What to do]

### Severity 3 (This Week)
- [Condition 1]
- [Condition 2]

**Response:** [What to do]

---

## Example: Data-Driven Iteration

**Week 1 Observation:**
- [Metric 1]: Status
- [Metric 2]: Status
- [Metric 3]: Status
- → [Decision/action]

**Week 2 Observation:**
- [Change observed]
- → [Investigation]

**Week 3 Observation:**
- [Result of intervention]
- → [Next iteration]

---

## Sign-Off

| Role | Name | Date | Approval |
|------|------|------|----------|
| Business | [Name] | [Date] | ☐ |
| Product | [Name] | [Date] | ☐ |
| Design | [Name] | [Date] | ☐ |
| Technology | [Name] | [Date] | ☐ |

---

## Document Control

**Version History:**
| Version | Date | Author | Change |
|---------|------|--------|--------|
| 1.0 | [Date] | Product + Tech | Initial observability & iteration framework |
