# Agile Frameworks

## Scrum (Deep Dive)

Sprint-based framework with defined roles, events, and artifacts.

### Theory — Three Pillars

Foundation: **Empiricism** — decisions rest on evidence, not prediction.

| Pillar | Meaning | In Practice |
|---|---|---|
| Transparency | All work visible | Kanban board visible to team + stakeholders |
| Inspection | Frequently examine progress | Daily Scrum, Sprint Review, Retrospective |
| Adaptation | Adjust quickly | Change backlog priority after review feedback |

### Roles

| Role | DO | DON'T |
|---|---|---|
| **Product Owner** | Define WHAT to build. Own backlog. Maximise value. Represent customer. Decide priority. | Tell team HOW. Manage people. |
| **Scrum Master** | Ensure Scrum followed. Remove impediments. Coach. Facilitate. Servant leader. | Assign tasks. Make product decisions. |
| **Developers** | Build product. Self-organise. Commit to Sprint Goal. Ensure quality (DoD). Decide HOW. | Wait to be told. Ignore DoD. |

### Events

| Event | When | Duration (4-wk) | Purpose |
|---|---|---|---|
| Sprint Planning | Start | ~8 hrs | Select backlog items, define Sprint Goal |
| Daily Scrum | Every day | 15 min | Sync progress, surface blockers |
| Sprint Review | End | ~4 hrs | Demo to stakeholders, get feedback |
| Sprint Retrospective | After Review | ~3 hrs | Reflect on PROCESS, action items |

### Artifacts

| Artifact | Description |
|---|---|
| Product Backlog | Ordered list of everything needed. Owned by PO. Always evolving. |
| Sprint Backlog | Subset selected for this sprint + plan to deliver. |
| Increment | Sum of completed items. Must meet DoD. Must be usable. |
| Definition of Done (DoD) | Shared quality checklist. Agreed at project start. |
| Burndown Chart | Remaining work (SP) over time (days). |

### Velocity & Story Points

**Story Points:** Relative effort measure. Considers complexity + uncertainty + volume. Fibonacci (1,2,3,5,8,13,21) or T-shirt. NOT hours.

**Velocity:** Total SP completed per sprint. For FORECASTING, not comparing teams. Average after 3+ sprints.

```
Velocity = 25 SP/sprint, Backlog = 150 SP
Sprints = 150/25 = 6, Sprint = 2 weeks → 12 weeks total
```

**Velocity analysis:** Only fully completed items count. Partial/rejected stories = 0 SP.

**Velocity drop:** Check estimation accuracy, external blockers, absences, tech debt. Trend over 3-4 sprints matters.

### Backlog Grooming

1. Clarify requirements  2. Prioritise by value  3. Estimate (SP)  4. Identify dependencies  5. Break down large stories

### Sprint Review vs Retrospective

| | Review | Retrospective |
|---|---|---|
| Focus | PRODUCT (what we built) | PROCESS (how we worked) |
| Attendees | Team + stakeholders | Team only |
| Output | Updated backlog | Action items for improvement |
| Activity | Demo working software | Reflect well/poorly |

### Release Planning

Product Vision → Product Roadmap → Release Plan (3-6 months) → Iteration Plan (stories, SP)

---

## Kanban

Continuous flow, visualise work, limit WIP. Best for continuous delivery, support/ops.

**Board:** Backlog → To Do → In Progress (WIP: 3) → Testing → Done

| Principle | Explanation |
|---|---|
| Visualise workflow | Every task is a card |
| Limit WIP | Max items per column |
| Manage flow | Track speed, find bottlenecks |
| Make policies explicit | Write down rules |
| Improve collaboratively | Data-driven improvement |

**Metrics:** Lead Time (request → delivery), Cycle Time (start → finish), Throughput (items/period)

---

## Lean

Eliminate waste, maximise value. From Toyota Production System (1930s).

**Five Principles:** Value (customer perspective) → Value Stream (map steps, find waste) → Flow (no interruption) → Pull (produce on demand) → Perfection (Kaizen)

**Seven Wastes (IT):** Overproduction (unwanted features), Waiting (approvals), Transport (unnecessary handoffs), Over-processing (gold-plating), Inventory (too many WIP), Motion (task-switching), Defects (bugs/rework)

---

## XP (Extreme Programming)

Engineering excellence. Small co-located teams (2-12).

| Practice | Meaning |
|---|---|
| Pair Programming | Two devs, one computer |
| TDD | Write test FIRST |
| CI | Merge frequently, auto-test |
| Refactoring | Improve structure, keep behaviour |
| Simple Design | Simplest thing that works |
| Collective Ownership | Anyone can modify any code |
| 40-Hour Week | Sustainable pace |

---

## SAFe

Scale Agile to large enterprises (50+ people).

| Concept | Meaning |
|---|---|
| Agile Release Train (ART) | Team of teams (50-125 people) |
| Program Increment (PI) | Timebox 8-12 weeks |
| PI Planning | 2-day face-to-face alignment |
| Portfolio Alignment | Strategic themes → teams |

**Criticism:** Can feel bureaucratic. Risk of "waterfall with sprints."
