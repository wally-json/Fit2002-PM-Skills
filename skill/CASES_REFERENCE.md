# Prioritisation, Procurement, PMBOK, Cases & Reference

## Prioritisation

### MoSCoW

| Priority | Meaning | Effort |
|---|---|---|
| **Must have** | Non-negotiable. Project fails without. | ~60% |
| **Should have** | Important but not critical for launch. | ~20% |
| **Could have** | Nice to have. If time/budget allows. | ~20% |
| **Won't have** | Agreed NOT to include this release. | Documented |

Use for: sprint planning, scope negotiation, budget cuts.

### Kano Model

| Type | Description | Example |
|---|---|---|
| **Basic (Must-be)** | Expected. Absence = dissatisfaction. | Login works |
| **Performance** | More is better. Linear satisfaction. | Faster load time |
| **Excitement** | Unexpected delight. | AI recommendations |

---

## Procurement

### SOW / RFP / RFQ

| Document | Purpose |
|---|---|
| **SOW** | Describes work: deliverables, timelines, requirements, standards |
| **RFP** | Ask vendors to propose solution + pricing |
| **RFQ** | Ask vendors for price quote on specific items |

**Bidders' Conference:** Meeting where vendors ask questions about SOW/RFP.

### Vendor Selection — Weighted Scoring Model (WSM)

Score = Sum of (Weight x Rating) per criterion.

1. Define criteria (cost, experience, technical fit, timeline)
2. Assign weights (total 100%)
3. Rate each vendor (1-10)
4. Calculate weighted scores
5. Select highest total

---

## PMBOK 7 Performance Domains

| Domain | Focus |
|---|---|
| Stakeholder | Identify, engage, manage expectations |
| Team | Build, develop, lead |
| Development Approach | Select right approach (predictive/agile/hybrid) |
| Planning | Scope, schedule, cost, quality, resources, risk |
| Project Work | Execute and manage work |
| Delivery | Deliver intended value |
| Measurement | Monitor and control performance |
| Uncertainty | Manage risks, ambiguity, complexity |

### Integration Across Domains

| Domain | Include |
|---|---|
| Risk | Register + responses |
| Time | Milestones, critical path, schedule variance |
| Cost | Budget, cost variance, contingency linked to risks |
| Scope | Deliverables in WBS, scope creep risk |
| Quality | Objectives, defect measures, KPIs |
| Resources | Availability risks, workload measures |
| Stakeholders | Risks, engagement measures, communication KPIs |

---

## Case Studies

### FBI Virtual Case File ($170M failure)

- Cost: $170M, Duration: 4 years, Outcome: abandoned
- Used Waterfall for rapidly evolving post-9/11 requirements
- No iterative feedback loops
- **Lesson:** Waterfall fails with volatile requirements. Stacey analysis would have indicated Agile/Hybrid.

### Optus Outage (Nov 2023)

- Software update gone wrong, no integration testing
- No failover, no rollback plan
- Nationwide impact, millions affected
- **Failures:** No testing strategy (Mitigate failure), no rollback (Accept without contingency), no redundancy (Avoid failure)
- **Lesson:** Integration testing and failover are NOT optional for critical infrastructure.

### Alice Library Analytics (Ethics)

- University library analytics identifies pattern among female tech students
- Beneficence: targeted services could help
- Non-maleficence: profiling could stigmatise
- Autonomy: do users know? Can they opt out?
- **Lesson:** Good intentions can produce unintended consequences. Review both.

---

## Reflective Writing — Gibbs' Cycle

| Step | Question |
|---|---|
| 1. Description | What happened? |
| 2. Feelings | What were you thinking/feeling? |
| 3. Evaluation | What was good/bad? |
| 4. Analysis | Why did things go that way? |
| 5. Conclusion | What else could you have done? |
| 6. Action Plan | What will you do differently? |

---

## Key Formulas

| Formula | Calculation |
|---|---|
| Stacey Score | Agreement (1-5) x Technology (1-5) |
| Risk Score | Likelihood (1-5) x Impact (1-5) |
| PERT | (O + 4M + P) / 6 |
| Velocity | Completed SP per sprint |
| Sprints Needed | Total SP / Average Velocity |
| Project Duration | Sprints x Sprint Length |
| Team Effectiveness | Completed SP / Planned SP |
| WSM Score | Sum (Weight x Rating) |

## Strategy Selection Cheat Sheet

| Decision | Use |
|---|---|
| How to run project? | Stacey → Predictive/Agile/Hybrid |
| Which Agile method? | Scrum/Kanban/XP/SAFe |
| How to estimate cost? | Analogous → Parametric → Bottom-up |
| How to prioritise? | MoSCoW / Kano / INVEST |
| How to handle risk? | Avoid/Mitigate/Transfer/Accept |
| What leadership? | Match style to situation |
| Ethical dilemma? | EDMF + ACS + Util/Deontology |
| How to reflect? | Gibbs' Cycle |
| How to decompose scope? | WBS |
| How to select vendor? | WSM |
