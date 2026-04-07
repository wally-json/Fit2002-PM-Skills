---
name: project-management
description: >
  IT Project Management knowledge engine with three modes: Decision (apply frameworks like Stacey Matrix,
  risk strategies, cost estimation, leadership styles to real problems), Quiz (multiple-choice exam revision
  with answers and explanations), and Roleplay (scenario-based PM decision-making practice). Covers PMBOK,
  Agile (Scrum/Kanban/XP/SAFe), Waterfall, Hybrid, risk/cost/scope/time management, leadership, ethics
  (EDMF/ACS), and procurement. Use when choosing project methodology, managing risks, estimating costs,
  selecting leadership approach, resolving ethical dilemmas, revising for PM exams, or practising PM scenarios.
  Triggers on: "project management", "Scrum", "Agile", "risk register", "Stacey", "WBS", "MoSCoW", "EDMF",
  "quiz", "revision", "roleplay", "scenario".
---

# IT Project Management

## Three Modes

### 1. Decision Mode (default)
User asks a PM question → route to the right framework → structured answer.

**Routing table:**

| Question type | Framework | Reference |
|---|---|---|
| Which lifecycle/methodology? | Stacey Matrix | [LIFECYCLE.md](LIFECYCLE.md) |
| Which Agile framework? | Scrum/Kanban/XP/SAFe comparison | [AGILE.md](AGILE.md) |
| How to estimate cost? | Analogous/Parametric/Bottom-up/PERT | [SCOPE_COST_TIME.md](SCOPE_COST_TIME.md) |
| How to handle a risk? | Avoid/Mitigate/Transfer/Accept | [RISK.md](RISK.md) |
| What leadership style? | 6 styles + Tuckman + Servant Leadership | [LEADERSHIP_ETHICS.md](LEADERSHIP_ETHICS.md) |
| Ethical dilemma? | EDMF 5 steps + ACS + Util/Deontology | [LEADERSHIP_ETHICS.md](LEADERSHIP_ETHICS.md) |
| Prioritise features? | MoSCoW / Kano / INVEST | [CASES_REFERENCE.md](CASES_REFERENCE.md) |
| Vendor selection? | WSM | [CASES_REFERENCE.md](CASES_REFERENCE.md) |

### 2. Quiz Mode
Trigger: user says "quiz", "revision", "MC", "multiple choice"

Workflow:
1. Ask: which topic? (or "all")
2. Read [QUIZ.md](QUIZ.md) → select questions for that topic
3. Present ONE question at a time (A/B/C/D)
4. Wait for user answer
5. Reveal: correct answer + why correct + why others wrong + section reference
6. Ask: next question or stop?
7. At end: show score summary (correct / total, weak areas)

### 3. Roleplay Mode
Trigger: user says "roleplay", "scenario"

Workflow:
1. Ask: which role? (PM / Scrum Master / Product Owner / Team Lead)
2. Read [SCENARIOS.md](SCENARIOS.md) → select a scenario
3. Present situation — set the scene, give constraints
4. User makes a decision
5. Challenge: "Why?" / introduce a complication
6. User responds again
7. Debrief: which frameworks applied, what was missed, better alternatives
8. Reference specific sections from knowledge base

## Decision Trees (Quick Reference)

```
"How certain are we?"
   Very certain        → Predictive     (Stacey 1-7)
   Somewhat uncertain  → Hybrid
   Very uncertain      → Agile          (Stacey 8-20)
   Total chaos         → Stop, re-scope (Stacey 21-25)

"What Agile method?"
   Structure + sprints       → Scrum
   Unpredictable flow        → Kanban
   Max code quality          → XP
   Many teams (50+ people)   → SAFe

"How to handle this risk?"
   Eliminate it?             → Avoid
   Reduce it?               → Mitigate
   Someone else can own it?  → Transfer
   Too small to care?        → Accept
   It's a GOOD thing?        → Exploit / Enhance / Share

"What leadership style?"
   Crisis                   → Directive
   Teaching moment          → Coaching
   Need buy-in              → Participative
   Low morale               → Affiliative
   High-performers          → Pacesetting
   Big change               → Visionary
   Scrum Master default     → Servant Leadership
```

## Key Formulas

| Formula | Calculation |
|---|---|
| Stacey Score | Agreement (1-5) × Technology (1-5) |
| Risk Score | Likelihood (1-5) × Impact (1-5) |
| PERT Estimate | (O + 4M + P) / 6 |
| Velocity | Completed SP per sprint |
| Sprints Needed | Total Backlog SP / Avg Velocity |
| WSM Score | Σ (Weight × Rating) |
