# Scope, Cost & Time Management

## Scope Management

### Product Scope vs Project Scope

| | Product Scope | Project Scope |
|---|---|---|
| Definition | Features/functions of the deliverable | Work required to deliver |
| Focus | What the product does | What the team does |
| Example | "App shows real-time data, allows reservations" | "3 sprints, test with 200 users, deploy" |

### Six Core Activities

1. **Plan Scope Management** — define how scope will be defined, validated, controlled
2. **Collect Requirements** — interviews, workshops, questionnaires, prototypes
3. **Define Scope** — detailed project scope statement
4. **Create WBS** — decompose into work packages
5. **Validate Scope** — formalise acceptance (client sign-off)
6. **Control Scope** — monitor and manage changes

### Requirements Traceability Matrix (RTM)

Tracks each requirement from origin → implementation → validation.

**Fields:** ID, Type (Functional/Non-functional), Description, Category, Source, Status, Assumptions

### Project Scope Statement (6 elements)

1. Boundaries (included/excluded)
2. Business Need (why)
3. Constraints (budget, timeline, regulations)
4. Assumptions (believed true, unconfirmed)
5. Processes Impacted
6. Interfaces (systems, teams, orgs)

### Work Breakdown Structure (WBS)

| Level | Name | Description |
|---|---|---|
| 0 | Project | Entire project |
| 1 | Major Phases | High-level deliverables |
| 2 | Sub-deliverables | Components within phases |
| 3 | Work Packages | Smallest estimable/assignable unit |
| 4 | Tasks/Activities | Specific actions |

**Organisation:** By Product Deliverables (Login, Dashboard, API) or By Phase (Initiation, Planning, Execution, Closing)

Rule: Lowest level = Work Package — small enough to estimate and assign.

### User Stories & INVEST

**Format:** `AS A [persona], I WANT TO [action] SO THAT [benefit]`

| Letter | Criteria |
|---|---|
| I | Independent — any order |
| N | Negotiable — not a contract |
| V | Valuable — delivers value |
| E | Estimable — effort can be estimated |
| S | Small — fits one sprint |
| T | Testable — clear acceptance criteria |

---

## Time Management

### Critical Path

Longest sequence of dependent tasks = minimum project duration. Zero float — any delay delays the project.

### Float / Slack

Time a task can be delayed without delaying the project. Critical path tasks = zero float.

### Gantt Chart

Bar chart: schedule, dependencies, milestones. Visual timeline.

### Milestones

Significant points, zero duration. Examples: "Requirements signed off," "MVP deployed," "UAT complete."

---

## Cost Management

### Cost vs Budget vs Baseline

| Term | Definition |
|---|---|
| Cost | Monetary value of resources needed |
| Budget | Authorised financial plan (baseline + reserves) |
| Cost Baseline | Approved time-phased budget for measuring performance |
| Contingency Reserve | For known risks ("known unknowns") |
| Management Reserve | For unknown risks ("unknown unknowns") |

```
Cost Baseline + Contingency Reserve + Management Reserve = Total Project Budget
```

### Cost Classification (9 types)

| Type | Definition | Example |
|---|---|---|
| Direct | Traceable to project activity | Developer salaries |
| Indirect | Shared across projects | Office rent |
| Fixed | Don't change with volume | Annual licence fee |
| Variable | Change with volume | Cloud hosting |
| Recurring | Repeat over lifecycle | Monthly SaaS |
| Non-recurring | One-time | Server purchase |
| Tangible | Measurable objectively | Hardware |
| Intangible | Hard to measure | Brand reputation |
| Sunk | Already spent, unrecoverable | Abandoned prototype |

Overheads: typically 10-15% of direct labour costs.

### Estimation Methods

| Method | How | Accuracy | When |
|---|---|---|---|
| Analogous (Top-Down) | Compare to past project | ROM: -50% to +100% | Early, limited info |
| Parametric | Statistical model ($500/SP) | -10% to +25% | Historical data available |
| Bottom-Up | Estimate each work package, sum | -5% to +10% | Detailed WBS exists |
| Three-Point (PERT) | (O + 4M + P) / 6 | Medium-High | Uncertain durations |
| Expert Judgment | Consult experienced pros | Varies | Complex/novel projects |

**Accuracy Ranges:** ROM (Initiation) → Budgetary (Planning) → Definitive (Execution)

**PERT Example:**
```
Login page: O=3d, M=5d, P=12d
Estimate = (3 + 4×5 + 12) / 6 = 35/6 = 5.8 days
```

### Budget Structure

- **Cost Baseline:** Approved, time-phased spending plan
- **Contingency Reserve:** 5-15% for identified risks. PM owns.
- **Management Reserve:** 5-10% above contingency. Sponsor approval needed.
