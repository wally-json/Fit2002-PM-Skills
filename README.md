# Project Management Revision Skill — A Guide for Students and Educators

Exam revision for IT Project Management shouldn't be passive. This skill turns a comprehensive knowledge base into an interactive study companion with quizzes, roleplay scenarios, and framework-driven Q&A.

## What Is This?

An AI-powered revision tool with three modes:

- **Quiz** — 72 multiple-choice questions across 8 topics, with instant marking and explanations
- **Roleplay** — 15 scenario-based exercises where you play PM, Scrum Master, or other roles and make decisions under pressure
- **Decision** — ask any PM question, get a structured answer using the correct framework

It covers the full PMBOK syllabus: lifecycle strategies, Agile frameworks (Scrum, Kanban, XP, SAFe), scope/cost/time/risk management, leadership, ethics, procurement, and real-world case studies.

The entire knowledge base is plain Markdown. It works with Claude Code, ChatGPT, or any AI assistant that accepts file uploads or system prompts.

## Setup

### Option A: Claude Code (recommended)

Drop the `project-management/` folder into `~/.claude/skills/`. The skill registers automatically. Type `quiz`, `roleplay`, or ask a PM question — it just works.

### Option B: ChatGPT (Custom GPT)

1. Go to [chat.openai.com](https://chat.openai.com) → Explore GPTs → Create
2. In **Instructions**, paste the full content of `SKILL.md`
3. Under **Knowledge**, upload these files:
   - `QUIZ.md` (72 MC questions)
   - `SCENARIOS.md` (15 roleplay scenarios)
   - `LIFECYCLE.md`, `AGILE.md`, `SCOPE_COST_TIME.md`, `RISK.md`
   - `LEADERSHIP_ETHICS.md`, `CASES_REFERENCE.md`
4. Name it "PM Revision" and save

Now any student with the link can use all three modes inside ChatGPT.

### Option C: Any AI (manual paste)

Copy the content of `SKILL.md` into the system prompt or first message. When a specific topic comes up, paste the relevant reference file. Works with Gemini, Copilot, or any chat-based AI.

## Quick Start

Once set up, use these trigger words:

| You type | What happens |
|---|---|
| `quiz` | Start a multiple-choice quiz |
| `roleplay` | Enter a scenario-based exercise |
| Any PM question | Get a framework-driven answer |

## Quiz Mode

Type `quiz`. Pick a topic:

1. Lifecycle (Waterfall, Agile, Stacey Matrix) — 10 questions
2. Agile Frameworks (Scrum, Kanban, XP, SAFe) — 12 questions
3. Scope & Cost (WBS, Estimation, Budget) — 10 questions
4. Risk Management — 10 questions
5. Leadership — 8 questions
6. Ethics — 10 questions
7. Procurement, PMBOK & Prioritisation — 8 questions
8. Cross-cutting (mixed) — 4 questions
9. All — full 72-question mock exam

Questions appear one at a time. After each answer, the AI reveals the correct choice, explains why the others are wrong, and cites the relevant section.

Questions follow six common exam patterns:

1. **"Which lifecycle?"** — calculate Stacey score, justify the choice
2. **"How to handle this risk?"** — classify threat/opportunity, pick strategy, assign owner
3. **"What leadership style?"** — match situation to one of six styles
4. **"Ethical dilemma"** — walk through EDMF 5 steps, check PMI values
5. **"Scrum roles/events"** — who decides WHAT (PO) vs HOW (Devs), Review vs Retro
6. **"Budget cut / scope change"** — triple constraint trade-off, MoSCoW prioritisation

**Study tip:** Start with your weakest topic. Save "All" for a timed mock exam one week before the test.

## Roleplay Mode

Type `roleplay`. Pick a role — PM, Scrum Master, Product Owner, Team Lead, Consultant, or others.

The AI drops you into a scenario. Here's an example session:

---

**AI:** You are the Project Manager on an $85,000 project. At 60% completion, costs have hit $80,000 with $15,000 of work remaining. Your boss says: "Don't tell the client. We'll sort it at the final invoice." The client asks you tomorrow: "Are we on budget?"

**Student:** I would be transparent with the client. I'd present the situation honestly and offer three options: reduce scope, extend the timeline, or approve the additional $10,000.

**AI:** Good — you've chosen disclosure, which aligns with PMI's Honesty value. But your boss just pulled you aside: "If you tell the client, I'll note it in your performance review." What do you do now?

**Student:** I'd still disclose. The EDMF framework says I need to check: would I accept responsibility for this decision? Would I make it public? Hiding costs fails both tests. I'd escalate to the project sponsor if my boss insists.

**AI:** **Debrief.** You correctly applied the EDMF 5-step framework and prioritised Honesty and Responsibility from the PMI values. You also identified the escalation path. One thing to add: present the overrun with a root cause analysis and a revised budget showing contingency reserve usage — this frames it as proactive management, not failure.

---

Each scenario runs 2-3 rounds, then debriefs with the frameworks you should have applied, what you missed, and what a stronger answer looks like.

The 15 built-in scenarios cover:

| Scenario | Topics tested |
|---|---|
| The Hidden Bug | Ethics (EDMF), Leadership |
| Velocity Crisis | Scrum, Leadership, Tuckman |
| Production Down | Directive leadership, crisis communication |
| Budget Blowout | Ethics (Honesty), Cost management |
| Methodology Selection | Stacey Matrix, Lifecycle |
| Ethical Algorithm | Utilitarianism vs Deontology, ACS Code |
| Risk Materialised | Risk response failure, Sprint replanning |
| Scope Creep | Change control, MoSCoW |
| Team Conflict | Leadership styles, Tuckman (Storming) |
| Failing Project Rescue | FBI VCF parallels, Sunk cost |
| Vendor Selection | WSM, Stakeholder management |
| The Optus Moment | Integration testing, Risk acceptance |
| Agile at Scale | SAFe, PI Planning |
| Library Analytics | Beneficence/Non-maleficence/Autonomy |
| Sprint Zero Debate | Technical spikes, PO vs SM roles |

## Decision Mode

Ask any PM question directly. The AI routes it to the right framework:

- "Agreement=4, Technology=3 — what methodology?" → Stacey Matrix (score 12 → Agile)
- "Only backend dev might get sick" → Risk response (Mitigate: pair programming + docs)
- "Two devs arguing about architecture" → Leadership (Affiliative first, then Participative)
- "Client wants to hide a bug" → EDMF 5 steps + PMI values
- "Budget cut 25%" → MoSCoW reprioritisation + stakeholder communication

This mode is useful for checking your reasoning on case study assignments or verifying framework application before submitting.

## For Educators

**In-class reinforcement.** After a lecture on risk management, have students run `quiz` on topic 4. Immediate feedback cements the concepts while they're fresh.

**Tutorial discussion starters.** Project a roleplay scenario to the class. Let students debate their approach for 10 minutes, then run the roleplay live to compare their reasoning against the framework-based debrief.

**Mock exam sessions.** Run the full 72-question quiz as a timed exercise. The score summary at the end highlights weak areas to target in the remaining revision time.

**Assignment scaffolding.** Students working on case studies can use Decision Mode to verify they're applying the correct framework before writing up their analysis.

## Customising the Content

All content is editable Markdown in the `project-management/` folder:

| File | What's inside | Size |
|---|---|---|
| `SKILL.md` | Entry point and routing logic | 100 lines |
| `QUIZ.md` | 72 MC questions with answers | 827 lines |
| `SCENARIOS.md` | 15 roleplay scenarios | 145 lines |
| `LIFECYCLE.md` | Waterfall/Agile/Hybrid/Stacey | 98 lines |
| `AGILE.md` | Scrum/Kanban/Lean/XP/SAFe | 133 lines |
| `SCOPE_COST_TIME.md` | WBS, Cost, Time management | 140 lines |
| `RISK.md` | Risk register and strategies | 100 lines |
| `LEADERSHIP_ETHICS.md` | Leadership styles + Ethics | 141 lines |
| `CASES_REFERENCE.md` | MoSCoW/Kano/PMBOK/Cases | 143 lines |

### Adding quiz questions

Follow this format in `QUIZ.md`:

```markdown
### Q73 [Topic]
Your question here?
A) Option A
B) Option B
C) Option C
D) Option D

**Answer: B**
Explanation of why B is correct and others are wrong.
See: §section reference
```

### Adding roleplay scenarios

Follow this format in `SCENARIOS.md`:

```markdown
## S16: Scenario Title [Topics]
**Role:** Role name
**Situation:** Description...
**Follow-ups:**
- Complication 1
- Complication 2
**Evaluation criteria:** Frameworks to apply
**Reference:** §section references
```

## Coverage Map

| Topic | Quiz | Roleplay |
|---|---|---|
| Lifecycle & Stacey Matrix | Q1-Q10 | S5, S10 |
| Scrum | Q11-Q17 | S2, S7, S15 |
| Kanban & Lean | Q18-Q20 | — |
| XP & SAFe | Q21-Q22 | S13 |
| Scope & WBS | Q23-Q25, Q32 | S8 |
| Cost & Estimation | Q26-Q30 | S4 |
| Time & Critical Path | Q31 | — |
| Risk Management | Q33-Q42 | S7, S12, S15 |
| Leadership | Q43-Q50 | S2, S3, S9, S13 |
| Ethics | Q51-Q60 | S1, S4, S6, S8, S14 |
| Procurement & WSM | Q63-Q64 | S11 |
| PMBOK & Prioritisation | Q61-Q62, Q65-Q66 | — |
| Case Studies | Q67-Q68 | S10, S12 |
| Cross-cutting | Q69-Q72 | — |
