# FIT2002 IT Project Management -- Knowledge Base

---

## 1. Project Lifecycle Strategies

### 1.1 Predictive (Waterfall)

A linear, sequential approach. One phase completes fully before the next begins: Requirements -> Design -> Build -> Test -> Deploy.

**When to use:** Requirements clear and stable from the start. Low technical uncertainty. Stacey score 1-7. Regulatory projects requiring mandatory documentation. Example: upgrading an existing data centre.

**Strengths:** Easy to understand and manage. Clear milestones and deliverables. Good for fixed-price contracts. Comprehensive documentation.

**Weaknesses:** Change is expensive late in the project. Customer sees working product only late. Risk of building the wrong thing. Testing happens late, bugs found late.

**Key phrase:** "Predictive works when you know WHAT you're building and HOW to build it before you start."

### 1.2 Iterative

Build the product in repeated cycles (iterations). Each iteration refines and improves the previous version. Like sculpting -- start with a rough shape, refine each pass.

**When to use:** Requirements understood at a high level but details need exploration. Feedback needed to refine the product. Example: UI/UX design where user testing reveals needed changes.

**Key distinction:** Iterative = revisit and improve the SAME thing each cycle. Incremental = add NEW pieces each cycle.

### 1.3 Incremental

Deliver the product in pieces (increments). Each increment adds new functionality. Like building a house -- foundation first, then walls, then roof.

**When to use:** Product can be divided into independent, deliverable chunks. Business wants early value delivery. Example: release a basic catalogue first, add search next, add payments next.

**MVP connection:** MVP (Minimum Viable Product) = the first increment. Simplest version that delivers value and allows feedback gathering. Subsequent increments build on the MVP based on user feedback.

### 1.4 Agile

A mindset (not a method) combining iterative AND incremental delivery with frequent feedback, self-organising teams, and embrace of change. Agile is the philosophy; Scrum, Kanban, etc. are the practices.

**When to use:** Requirements uncertain or evolving. Stacey score 8-20. Customer involvement available and desired. Team skilled and motivated. Example: new mobile app where user needs are still being discovered.

**Four Agile Values (2001 Manifesto, Snowbird, Utah):**

| Prioritise | Over |
|---|---|
| Individuals & Interactions | Processes & Tools |
| Working Software | Comprehensive Documentation |
| Customer Collaboration | Contract Negotiation |
| Responding to Change | Following a Plan |

Items on the right still have value, but we prioritise the left. "Working Software over Comprehensive Documentation" does NOT mean no documentation -- you still need user stories, DoD, API docs. It means: don't spend three months writing a 200-page requirements doc before writing any code.

**Twelve Principles (grouped):**
- DELIVERY: Deliver early and often. Welcome change. Working product is the progress measure. Simplicity.
- PEOPLE: Motivated individuals. Collaboration. Face-to-face communication. Sustainable pace.
- IMPROVEMENT: Attention to excellence. Self-organising teams. Regular reflection.

**Agile Historical Timeline:**
- 1930s: Toyota Way (influenced Lean thinking)
- 1995: Scrum codified by Ken Schwaber and Jeff Sutherland
- 2001: Agile Manifesto created by 17 software leaders
- 2010s-present: Scaled frameworks (SAFe, Spotify model) bring Agile to enterprise

### 1.5 Hybrid

Combining predictive and agile approaches within the same project. Different parts use different strategies.

**When to use:** Some parts well-understood (predictive), others uncertain (agile). Example: backend infrastructure is fixed spec (predictive), frontend UX needs iteration (agile).

**Key phrase:** "Use the right approach for the right part of the project."

**Case example (UniPark):** Stacey score 6 (Agreement=2, Tech=3) placed the project in Predictive zone, but UX uncertainty justified a hybrid: predictive for backend, Agile sprints for mobile frontend.

### 1.6 Stacey Matrix (Decision Tool)

Developed by Ralph Stacey (2002). Purpose: determine suitable project lifecycle approach.

**Score = Agreement (1-5) x Technology Complexity (1-5)**

| Score Range | Decision |
|---|---|
| 1-7 | Predictive/Incremental (requirements clear, tech known) |
| 8-20 | Iterative/Agile (uncertainty in agreement or tech) |
| 21-25 | Delay or re-scope (too chaotic, fundamentally risky) |

**Agreement Scoring:**

| Score | Meaning |
|---|---|
| 1 | Almost 100% agreement |
| 2 | ~80% agreement |
| 3 | ~50% agreement |
| 4 | ~30% agreement |
| 5 | Almost no agreement |

**Technology/Complexity Scoring:**

| Score | Meaning |
|---|---|
| 1 | Known technology, team has done this before |
| 2 | Known with few challenges |
| 3 | May require prototyping |
| 4 | Few known, many unknowns |
| 5 | Almost 100% new/unknown |

**Stacey Matrix Zones:**
- Simple (low/low): Linear approaches work well
- Complicated: Predictive works
- Complex: Adaptive approaches work well
- Chaos: Fundamentally risky -- stop, re-scope first

**Example Calculations:**

| Project | Agreement | Tech | Score | Decision |
|---|---|---|---|---|
| WiFi Upgrade (Case 1) | 1 | 1 | 1 | Predictive |
| Storage Upgrade | 1 | 2 | 2 | Predictive |
| Bank Migration (Case 3) | 1 | 3 | 3 | Hybrid |
| Cafe App (Case 2) | 4 | 3 | 12 | Agile |
| AI Chatbot (Case 4) | 5 | 5 | 25 | Delay/Re-scope |

### 1.7 SDLC Comparison Table

| Aspect | Predictive | Iterative | Incremental | Agile | Hybrid |
|---|---|---|---|---|---|
| Requirements | Fixed upfront | High-level known, details evolve | Defined per increment | Evolving continuously | Mixed |
| Delivery | Single delivery at end | Refined versions | Usable pieces | Working increments each sprint | Varies by component |
| Change response | Expensive, formal process | Moderate | Moderate | Embraced | Depends on part |
| Customer feedback | Late | Each iteration | Each increment | Every sprint | Mixed |
| Best for | Stable, well-understood | Design exploration | Phased delivery | High uncertainty | Mixed certainty |

---

## 2. Agile Frameworks

### 2.1 Scrum (Deep Dive)

Sprint-based, structured framework with defined roles, events, and artifacts. Best for evolving products with complex requirements.

#### Scrum Theory & Three Pillars

Foundation: **Empiricism** -- decisions rest on evidence, not prediction. Knowledge grows from real work, not upfront documents.

| Pillar | Meaning | In Practice |
|---|---|---|
| **Transparency** | All work is visible to everyone | Kanban board visible to whole team + stakeholders |
| **Inspection** | Frequently examine progress and artifacts | Daily Scrum, Sprint Review, Retrospective |
| **Adaptation** | Adjust quickly when something isn't working | Change backlog priority after review feedback |

#### Roles (PO, SM, Developers)

| Role | What they DO | What they DON'T do |
|---|---|---|
| **Product Owner** | Define WHAT to build. Own the backlog. Maximise value. Represent the customer. Decide priority based on business value. | Tell the team HOW to build. Manage people. |
| **Scrum Master** | Ensure Scrum is followed. Remove impediments. Coach the team. Facilitate events. Servant leader. | Assign tasks. Make product decisions. Boss people around. |
| **Developers** | Build the product. Self-organise. Commit to Sprint Goal. Ensure quality (DoD). Decide HOW to build. | Wait to be told what to do. Ignore the DoD. |

#### Events (Planning, Daily, Review, Retro)

| Event | When | Duration (4-week sprint) | Purpose |
|---|---|---|---|
| **Sprint Planning** | Start of sprint | ~8 hrs | Select backlog items, define Sprint Goal, create Sprint Backlog |
| **Daily Scrum** | Every day | 15 min max | Sync progress, surface blockers. 3 questions: What did I do? What will I do? Any blockers? |
| **Sprint Review** | End of sprint | ~4 hrs | Demo working software to stakeholders. Get feedback. Update backlog. |
| **Sprint Retrospective** | After Review | ~3 hrs | Reflect on PROCESS. What went well? What to improve? Action items for next sprint. |

#### Artifacts (Product Backlog, Sprint Backlog, Increment, DoD, Burndown)

| Artifact | Description |
|---|---|
| **Product Backlog** | Ordered list of everything the product needs. Owned by PO. Always evolving. |
| **Sprint Backlog** | Subset of Product Backlog selected for this sprint + plan to deliver it. |
| **Increment** | Sum of all completed backlog items. Must meet DoD. Must be usable. |
| **Definition of Done (DoD)** | Shared quality checklist (e.g., coded, tested, reviewed, documented). Agreed by the whole Scrum team at project start. Without DoD, quality is inconsistent and velocity unreliable. |
| **Burndown Chart** | Graph showing remaining work over time. Y-axis = remaining story points. X-axis = days. |

#### Velocity & Story Points

**Story Points:** Relative measure of effort. Considers complexity + uncertainty + volume of work. Common scales: Fibonacci (1, 2, 3, 5, 8, 13, 21) or T-shirt (XS, S, M, L, XL). NOT hours. Team calibrates to their own baseline.

**Velocity:** Total story points completed in one sprint. Used to FORECAST, not to compare teams. Calculate after 3+ sprints, take the average.

**Velocity Forecasting Example:**
```
Team velocity = 25 SP/sprint
Total backlog = 150 SP
Sprints needed = 150 / 25 = 6 sprints
Sprint length = 2 weeks
Project duration = 6 x 2 = 12 weeks
```

**Velocity Analysis Example:**
```
Sprint 1: 4 stories, 10 total SP
  Story 1 (3 SP): Completed    -> counts
  Story 2 (2 SP): Rejected     -> does NOT count
  Story 3 (1 SP): Completed    -> counts
  Story 4 (4 SP): Partial      -> does NOT count
Completed SP = 3 + 1 = 4 SP (only fully done items count)
Velocity = 4 SP
Team Effectiveness = 4/10 = 40%
```

**Velocity drop investigation:** Check estimation accuracy, external blockers, team absences, technical debt. One bad sprint is not a crisis -- trend over 3-4 sprints matters more.

**Cannot compare velocity across teams** -- story points are calibrated relative to each team's own baseline.

#### Backlog Grooming

Ongoing activity to keep the backlog ready for upcoming sprints:
1. Clarify requirements
2. Prioritise tasks by business value
3. Estimate effort (story points)
4. Identify dependencies
5. Break down large stories into smaller tasks

Best practice: schedule regularly before sprint planning. Involve PO, developers, and subject matter experts.

#### Sprint Review vs Retrospective

| Aspect | Sprint Review | Sprint Retrospective |
|---|---|---|
| Focus | The PRODUCT (what we built) | The PROCESS (how we worked) |
| Who attends | Team + stakeholders | Team only |
| Output | Updated backlog based on feedback | Action items for process improvement |
| Key activity | Demo working software | Reflect on what went well/poorly |

**Sprint Review Best Practices:** Always show working software, not just slides. Rotate presenters. Involve stakeholders. Frame features as user stories / business outcomes.

**Sprint Retrospective Steps:**
1. Set the Stage -- create open environment, try icebreaker
2. Gather Data -- review backlog, goal, metrics, feedback
3. Generate Insights -- identify what went well/didn't, opportunities
4. Decide What to Do -- prioritise action items by impact and feasibility
5. Close -- summarise key takeaways, agree on next steps

#### Release Planning

```
Product Vision -> Product Roadmap -> Release Plan -> Iteration Plan
Release Plan: 3-6 months, multiple iterations/sprints
Iteration Plan: features broken into user stories, estimated in story points
```

### 2.2 Kanban

Continuous flow, visualise work, limit work-in-progress. Best for continuous delivery, support/ops teams.

**Board structure:** Backlog -> To Do -> In Progress (WIP: 3) -> Testing -> Done

| Principle | Explanation |
|---|---|
| Visualise the workflow | Every task is a card on the board |
| Limit WIP | Max number of items in each column (e.g., only 3 items "In Progress") |
| Manage flow | Track how fast items move. Identify bottlenecks. |
| Make policies explicit | Write down rules: "What does 'Done' mean?" |
| Improve collaboratively | Use data to drive improvement |

**Metrics:**
- Lead Time: request to delivery
- Cycle Time: work started to work finished
- Throughput: items completed per time period

**Case example (IT Help Desk, Case 5):** Work arrives unpredictably -- can't plan sprints. Kanban's continuous flow + WIP limits prevent overload.

### 2.3 Lean

Eliminate waste, maximise value. Originated from Toyota Production System (1930s).

**Five Lean Principles:**

| Principle | Meaning |
|---|---|
| Value | Define value from customer's perspective |
| Value Stream | Map all steps; identify waste |
| Flow | Value-creating steps flow without interruption |
| Pull | Only produce what the next step needs |
| Perfection | Continuously improve (Kaizen) |

**Seven Wastes (IT context):**

| Waste | IT Example |
|---|---|
| Overproduction | Building features nobody asked for |
| Waiting | Developers waiting for approvals |
| Transport | Unnecessary handoffs between teams |
| Over-processing | Gold-plating features beyond requirements |
| Inventory | Too many unfinished stories in progress |
| Motion | Switching between too many tasks |
| Defects | Bugs that require rework |

### 2.4 XP (Extreme Programming)

Engineering excellence through disciplined practices. Best for high-quality software delivery. Small, co-located teams (2-12 people).

| Practice | Meaning |
|---|---|
| Pair Programming | Two developers at one computer. One codes, one reviews in real-time. |
| Test-Driven Development (TDD) | Write the test FIRST, then write code to pass it. |
| Continuous Integration (CI) | Merge code to main branch frequently. Automated tests run on every merge. |
| Refactoring | Improve code structure without changing behaviour. |
| Simple Design | Build the simplest thing that works. |
| Collective Code Ownership | Anyone can modify any code. No silos. |
| 40-Hour Week | Sustainable pace. No heroics. |

**Case example (Hospital Software, Case 8):** When bugs = life-threatening, XP's TDD, pair programming, and CI catch defects early and often.

### 2.5 SAFe

Scale Agile practices to large enterprises with multiple teams. Best for 50+ people coordinating.

| Concept | Meaning |
|---|---|
| Agile Release Train (ART) | Team of Agile teams (50-125 people) that plan, commit, and execute together |
| Program Increment (PI) | Timebox (8-12 weeks) for the ART to deliver value. Like a "big sprint." |
| PI Planning | 2-day face-to-face event where all teams align on what to build |
| Portfolio Alignment | Strategic themes and budgets flow from portfolio to teams |

**Criticism:** Can feel bureaucratic. Risk of becoming "waterfall with sprints" if not implemented genuinely.

**Case example (Telco, Case 7):** 12 Scrum teams = ~60-120 people. Too many for informal coordination. SAFe provides ART and PI Planning to align all teams every 8-12 weeks.

---

## 3. Scope Management

### 3.1 Product Scope vs Project Scope

| | Product Scope | Project Scope |
|---|---|---|
| Definition | Features and functions of the deliverable | Work required to deliver the product |
| Focus | What the product does | What the team does |
| Example | "App shows real-time parking data, allows reservations, processes payments" | "Gather requirements, design architecture, develop in 3 sprints, test with 200 users, deploy to app store" |

### 3.2 Six Core Activities

1. **Plan Scope Management** -- define how scope will be defined, validated, and controlled
2. **Collect Requirements** -- determine, document, and manage stakeholder needs (techniques: interviews, workshops, questionnaires, prototypes)
3. **Define Scope** -- develop detailed project scope statement
4. **Create WBS** -- decompose deliverables into manageable work packages
5. **Validate Scope** -- formalise acceptance of completed deliverables (client sign-off)
6. **Control Scope** -- monitor scope status and manage changes (change control process)

### 3.3 Requirements Traceability Matrix (RTM)

Tracks each requirement from origin to implementation to validation. Ensures nothing is missed, nothing is built without justification, and testing covers all requirements.

**RTM Fields:**

| Field | Description |
|---|---|
| ID | Unique identifier (e.g., REQ-001) |
| Type | Functional / Non-functional |
| Description | Clear statement of the requirement |
| Category | UI, Backend, Security, Performance, etc. |
| Source | Who requested it (stakeholder, regulation, user research) |
| Status | Proposed, Approved, In Progress, Implemented, Validated |
| Assumptions | What is assumed to be true for this requirement |

### 3.4 Project Scope Statement

Six key elements:
1. **Boundaries** -- what is included and excluded
2. **Business Need** -- why the project exists
3. **Constraints** -- budget, timeline, regulations, technology limitations
4. **Assumptions** -- conditions believed true but not confirmed
5. **Processes Impacted** -- existing workflows affected by the project
6. **Interfaces** -- systems, teams, or organisations the project must interact with

### 3.5 Work Breakdown Structure (WBS)

Hierarchical decomposition of total work scope into manageable work packages. Foundation for scheduling and cost estimation.

**WBS Levels:**

| Level | Name | Description |
|---|---|---|
| Level 0 | Project | The entire project |
| Level 1 | Major Phases | High-level deliverables or phases (e.g., Planning, Development, Testing) |
| Level 2 | Sub-deliverables | Components within each phase (e.g., Frontend, Backend) |
| Level 3 | Work Packages | Smallest manageable unit of work that can be estimated and assigned |
| Level 4 | Tasks/Activities | Specific actions within a work package |

**WBS Organisation Methods:**
- **By Product Deliverables:** organise around what is being built (e.g., Login Module, Dashboard, API)
- **By Phase:** organise around project phases (e.g., Initiation, Planning, Execution, Closing)

**Example:**
```
Project (Level 0)
  +-- Phase 1: Planning (Level 1)
  |     +-- 1.1 Requirements gathering (Level 2)
  |     +-- 1.2 Architecture design
  |     +-- 1.3 Environment setup
  +-- Phase 2: Development (Level 1)
        +-- 2.1 Frontend (Level 2)
        |     +-- 2.1.1 Login page (Level 3 / Work Package)
        |     +-- 2.1.2 Dashboard
        +-- 2.2 Backend
```

Rule: Lowest level = "Work Package" -- small enough to estimate and assign.

### 3.6 User Story Format & INVEST

**User Story Format:**
```
AS A [persona], I WANT TO [action] SO THAT [benefit]
```

**INVEST Criteria** (a good user story should be):

| Letter | Criteria | Meaning |
|---|---|---|
| I | Independent | Can be developed in any order |
| N | Negotiable | Details can be discussed; not a contract |
| V | Valuable | Delivers value to user or business |
| E | Estimable | Team can estimate the effort |
| S | Small | Fits within one sprint |
| T | Testable | Has clear acceptance criteria |

---

## 4. Time Management

### 4.1 Critical Path

The longest sequence of dependent tasks determining minimum project duration. Tasks on the critical path have zero float -- any delay directly delays the project. Identifying the critical path helps the PM know which tasks require the closest monitoring.

### 4.2 Float / Slack

The time a task can be delayed without delaying the project. Tasks on the critical path have zero float. Tasks with float can be delayed without affecting the project end date.

### 4.3 Gantt Chart

Bar chart showing schedule, dependencies, and milestones. Visual representation of what happens when, which tasks depend on others, and overall project timeline.

### 4.4 Milestones

Significant points in the project with zero duration. Mark the completion of major deliverables or phases. Examples: "Requirements signed off," "MVP deployed," "UAT complete."

---

## 5. Cost Management

### 5.1 Cost vs Budget vs Baseline

| Term | Definition |
|---|---|
| Cost | The monetary value of resources required to complete project activities |
| Budget | The authorised financial plan, including cost baseline + reserves |
| Cost Baseline | The approved time-phased budget against which performance is measured |
| Contingency Reserve | For known risks ("known unknowns") |
| Management Reserve | For unknown risks ("unknown unknowns") |

**Budget Structure:**
```
Cost Baseline (approved budget)
  + Contingency Reserve (known risks)
  + Management Reserve (unknown risks)
  = Total Project Budget
```

### 5.2 Cost Classification (9 types)

| Type | Definition | Example |
|---|---|---|
| **Direct** | Traceable to a specific project activity | Developer salaries, software licences |
| **Indirect** | Shared across projects, not directly traceable | Office rent, utilities, admin staff |
| **Fixed** | Do not change with production volume | Annual software licence fee |
| **Variable** | Change with production volume | Cloud hosting usage, overtime pay |
| **Recurring** | Repeat over the project lifecycle | Monthly SaaS subscription |
| **Non-recurring** | One-time costs | Server purchase, setup fee |
| **Tangible** | Can be measured objectively | Hardware, labour hours |
| **Intangible** | Difficult to measure objectively | Brand reputation, employee morale |
| **Sunk** | Already spent, cannot be recovered | Money spent on abandoned prototype |

**Overheads & Indirect Costs:** Typically 10-15% of direct labour costs. Some funders cap indirect costs at a fixed percentage.

### 5.3 Cost Management Process (4 steps)

1. **Plan Cost Management** -- define how costs will be estimated, budgeted, managed, monitored, and controlled
2. **Estimate Costs** -- approximate monetary resources needed for project activities
3. **Determine Budget** -- aggregate estimated costs to establish an authorised cost baseline
4. **Control Costs** -- monitor project costs and manage changes to the cost baseline

### 5.4 Estimation Methods (5 methods + accuracy ranges)

| Method | How it works | Accuracy Range | When to use |
|---|---|---|---|
| **Analogous (Top-Down)** | Compare to similar past project | ROM: -50% to +100% | Early project, limited info |
| **Parametric** | Statistical model (e.g., $500/story point) | Budgetary: -10% to +25% | Historical data available |
| **Bottom-Up** | Estimate each work package, then sum | Definitive: -5% to +10% | Detailed WBS exists |
| **Three-Point (PERT)** | (O + 4M + P) / 6 | Medium-High | Uncertain durations |
| **Expert Judgment** | Consult experienced professionals | Varies | Complex or novel projects |

**Estimate Accuracy Ranges:**

| Type | Range | Typical Phase |
|---|---|---|
| ROM (Rough Order of Magnitude) | -50% to +100% | Initiation |
| Budgetary | -10% to +25% | Planning |
| Definitive | -5% to +10% | Execution |

**Three-Point Example:**
```
Task: Build login page
Optimistic (O) = 3 days
Most Likely (M) = 5 days
Pessimistic (P) = 12 days
Estimate = (3 + 4x5 + 12) / 6 = 35/6 = 5.8 days
```

**Numerical Estimation Comparison (Workshop 4 example):**

| Method | Estimate |
|---|---|
| Analogous | $8,800 |
| Parametric | $9,900 |
| Bottom-up | $9,900 |
| PERT (Three-Point) | $9,983 |
| Expert Judgment | $10,500 |

### 5.5 Budget Structure (Baseline + Contingency + Management Reserve)

- **Cost Baseline:** Approved budget for measuring performance. Time-phased spending plan.
- **Contingency Reserve:** For identified risks (known unknowns). Typically 5-15% of baseline. Owned by PM.
- **Management Reserve:** For unidentified risks (unknown unknowns). Typically 5-10% above contingency. Requires sponsor approval to use.

**Case example (UniPark):** $80,000 total costs against $85,000 budget, leaving $5,000 contingency for known risks.

---

## 6. Risk Management

### 6.1 Definitions (Risk vs Issue vs Assumption)

| Type | Time | Definition | Example |
|---|---|---|---|
| **Risk** | FUTURE | Uncertain event that, if it occurs, affects project objectives in scope, time, cost, or quality | "The developer might quit mid-project" |
| **Issue** | NOW | Problem you are already facing | "We missed the last 2 deadlines" |
| **Assumption** | BELIEVED | Something believed true but not confirmed | "We assume the API will be ready by Week 3" |

Two types of risk: **Threats** (negative impact) and **Opportunities** (positive impact).

### 6.2 Risk Management Process (6 steps)

```
1. Plan -> 2. Identify -> 3. Qualitative Analysis -> 4. Quantitative Analysis -> 5. Respond -> 6. Monitor
```

1. **Risk Planning:** Define how risk management will be conducted. Create Risk Management Plan and Risk Register.
2. **Risk Identification:** Discover potential risks. Techniques: Brainstorming, Delphi, SWOT, Documentation Review, Checklists.
3. **Qualitative Risk Analysis:** Prioritise risks by impact and probability. Score = Likelihood (1-5) x Impact (1-5).
4. **Quantitative Risk Analysis:** Numerically assess high-priority risks. Tools: Monte Carlo Simulation, Decision Trees.
5. **Risk Response Planning:** Select strategies for threats and opportunities (see 6.6).
6. **Risk Monitoring & Control:** Track risks and response effectiveness. Risk Audits, Risk Reviews, Watch List. Every high/medium risk must have one named owner.

### 6.3 Risk Register

**Fields:** ID, Risk Description, Category, Likelihood (1-5), Impact (1-5), Score, Owner, Strategy, Status, Notes

**Example Entry:**
```
ID: R-1
Risk: IoT sensor data integration failure
Category: Technical
Likelihood: 3, Impact: 5, Score: 15 (High)
Owner: Lead Developer
Strategy: Mitigate -- build proof-of-concept in Sprint 0
Status: Open
```

### 6.4 Risk Classification Categories

| Category | Example | Typically Affects | Who Owns |
|---|---|---|---|
| Technical | Backend API fails | Schedule, testing | Dev lead |
| Stakeholder | Client unresponsive during UAT | Approvals, handover | PM |
| External | Policy change delays data approval | Compliance, timeline | Sponsor/Legal |
| Resourcing | Key developer leaves | Velocity, task ownership | Scrum Master |
| Opportunity | Tool upgrade reduces testing time | Cost, schedule | PM |

### 6.5 Qualitative & Quantitative Analysis

**Qualitative:**
```
Risk Score = Likelihood (1-5) x Impact (1-5)
1-5   = Low    -> monitor
6-14  = Medium -> plan response
15-25 = High   -> act immediately
```

**Quantitative (advanced):**
- Monte Carlo Simulation: run thousands of scenarios to get probability distribution
- Decision Trees: map choices and outcomes with probabilities and values

### 6.6 Risk Response Strategies (Threats & Opportunities)

**For Threats:**

| Strategy | What you do | Example | When to use |
|---|---|---|---|
| **Avoid** | Eliminate the risk entirely by changing the plan | Remove high-risk feature from scope | Risk is too dangerous AND you can change scope |
| **Mitigate** | Reduce likelihood OR impact | Add testing, training, pair programming | Most common -- practical steps to reduce risk |
| **Transfer** | Pass risk to another party | Insurance, SLA, use Stripe for PCI compliance | You don't control the risk; someone else can |
| **Accept** | Do nothing, just monitor | Low-impact cosmetic bug on old device | Impact low AND cost of response exceeds risk |

**For Opportunities:**

| Strategy | What you do | Example |
|---|---|---|
| **Exploit** | Make it happen | Assign best developer to capture the opportunity |
| **Enhance** | Increase the chance or value | Prepare migration guide before competitor shuts down |
| **Share** | Partner with someone | Co-develop a feature with another company |
| **Accept** | Don't actively pursue, but welcome if it happens | Small opportunity, not worth additional investment |

**Case examples:**
- Vendor might increase prices 40% (Case 9): Mitigate (lock in fixed-price contract) or Avoid (switch vendor)
- Only backend dev might get sick (Case 10): Mitigate (pair programming, documentation)
- App stores credit card data (Case 12): Transfer (use PCI-DSS compliant provider like Stripe)
- 5% chance of blurry icon on old device (Case 13): Accept (low likelihood, cosmetic only)
- Competitor might shut down (Case 14): Enhance (prepare migration guide NOW)

### 6.7 Probability/Impact Matrix

```
              Impact
              Low    Medium    High
Probability
High         | Med  |  High   | High |  <- Act immediately
Medium       | Low  |  Med    | High |
Low          | Low  |  Low    | Med  |  <- Monitor
```

Upper-right = highest priority, act now. Lower-left = lowest priority, monitor.

### 6.8 Risk Monitoring & Ownership

- Track risks and response effectiveness continuously
- Risk Audits, Risk Reviews, Watch List
- Every high/medium risk must have ONE named owner
- Update risk register regularly -- not a one-time document
- Link risks to schedule, cost, or scope impacts

**Common Mistakes:**
- Confusing issues with risks
- Only listing negative risks (ignoring opportunities)
- Using vague risks: "budget overrun" instead of "vendor invoice delays"
- Creating a risk register once but never updating it
- Not linking risks to schedule, cost, or scope impacts

---

## 7. Prioritisation

### 7.1 MoSCoW

| Priority | Meaning | Effort Rule |
|---|---|---|
| **Must have** | Non-negotiable. Project fails without these. | ~60% of effort |
| **Should have** | Important but not critical for launch. | ~20% of effort |
| **Could have** | Nice to have. Include if time/budget allows. | ~20% of effort |
| **Won't have (this time)** | Agreed to NOT include in this release. | Documented for future |

Use for: Sprint planning, scope negotiation, budget cuts. Case example (FreshBox): when budget cut 25%, use MoSCoW to identify Could/Won't features to cut.

### 7.2 INVEST Criteria

See Section 3.6.

### 7.3 Kano Model

Classifies features by customer satisfaction:

| Type | Description | Example |
|---|---|---|
| **Basic (Must-be)** | Expected. Absence causes dissatisfaction, presence doesn't excite. | Login works |
| **Performance** | More is better. Linear relationship with satisfaction. | Faster load time = happier users |
| **Excitement (Delighter)** | Unexpected. Absence doesn't cause dissatisfaction, presence delights. | AI-powered recommendations |

---

## 8. Leadership

### 8.1 Six Leadership Styles (Margules 2011)

| Style | Core Behaviour | Best When | Danger |
|---|---|---|---|
| **Directive** | "Do this now." Clear orders. | Crisis, tight deadline, new team | Micromanagement, disempowerment |
| **Coaching** | "Let me help you grow." Mentoring. | Developing junior team members | Too slow when immediate results needed |
| **Participative** | "What does everyone think?" Shared decisions. | Team has expertise, buy-in needed | Delays if no consensus |
| **Affiliative** | "People first." Harmony, trust. | Team morale is low, after conflict | Avoids tough conversations |
| **Pacesetting** | "Follow my example." High bar. | Expert team, tight delivery | Burnout, frustration |
| **Visionary** | "Imagine where we're going." Inspires. | Change initiatives, new projects | Not effective without credibility |

**Case examples:**
- Production down, team panicking (Case 15): Directive -- "You check logs. You restart service. Go."
- New intern, never used Git (Case 16): Coaching -- sit with them, show basics, focus on growth
- Two devs had heated argument (Case 17): Affiliative -- people first, rebuild trust
- Architecture decision, everyone has opinions (Case 18): Participative -- facilitate discussion, build consensus
- Company pivoting desktop to mobile (Case 19): Visionary -- paint the big picture, connect to concrete steps
- Sprint going badly, team losing motivation: Combination -- affiliative first (rebuild trust), then coaching (1-on-1), then directive if deadline-critical

### 8.2 Servant Leadership (Greenleaf 1970)

Robert K. Greenleaf (1970): "The servant-leader is servant first."

Core idea: Lead by serving others -- focus on THEIR growth, well-being, performance.

Key behaviours:
- "How can I help you succeed?" NOT "Did you finish the task?"
- Remove impediments
- Create psychological safety
- Listen before directing

Most closely aligns with Coaching + Affiliative styles.

### 8.3 PM vs Scrum Master

| Aspect | Project Manager | Scrum Master |
|---|---|---|
| Focus | Planning, scope, schedule, budget, stakeholder alignment | Facilitating Scrum, empowering team, removing impediments |
| Authority | Often has authority over budget and resources | No formal authority; influence through coaching |
| Approach | Plan-driven, controls execution | Servant leader, enables self-organisation |
| Relationship to team | Manages the team | Serves the team |
| Decision-making | Makes key project decisions | Helps team make their own decisions |

### 8.4 Team Development (Tuckman)

Tuckman's stages of group development:

| Stage | Description | Leader Action |
|---|---|---|
| **Forming** | Team comes together. Polite, uncertain, testing boundaries. | Provide clear direction, establish ground rules. Directive style. |
| **Storming** | Conflict emerges. Competing ideas, power struggles, frustration. | Mediate conflicts, clarify roles. Coaching/Affiliative style. |
| **Norming** | Team establishes shared norms. Trust builds, roles clarify. | Step back, encourage collaboration. Participative style. |
| **Performing** | High-functioning team. Self-organising, delivering effectively. | Delegate, remove obstacles. Servant leadership. |

### 8.5 MBTI

Myers-Briggs Type Indicator -- personality framework useful for understanding team dynamics:

| Dimension | Poles | Relevance to PM |
|---|---|---|
| Energy source | Introvert (I) / Extrovert (E) | How team members recharge and communicate preferences |
| Information gathering | Sensing (S) / iNtuitive (N) | Detail-oriented vs big-picture thinkers |
| Decision-making | Thinking (T) / Feeling (F) | Logic-driven vs values-driven decisions |
| Lifestyle | Judging (J) / Perceiving (P) | Structured planners vs flexible adapters |

Understanding MBTI helps PMs adapt communication style, assign roles effectively, and manage team dynamics.

---

## 9. Ethics

### 9.1 Morality vs Ethics vs Law

| Concept | Definition | Example of Misalignment |
|---|---|---|
| **Morality** | Personal principles and values about right/wrong | Whistleblowing may feel morally right |
| **Ethics** | Branch of philosophy examining moral principles to establish standards; also professional codes of conduct | Professional codes may conflict with personal morality |
| **Law** | Formal rules governing society, enforceable by the state | Something lawful may be immoral; something unlawful may be considered moral by some |

Morality and law can misalign: what is lawful may be immoral; what is unlawful may be considered moral by some.

### 9.2 Helgadottir's Three Core PM Skills

Helgadottir (2008): Core PM skills = intersection of three types of thinking:
- **Creative thinking** -- generating innovative solutions
- **Logical thinking** -- systematic analysis and reasoning
- **Ethical thinking** -- moral reasoning and judgment

The intersection of all three = PM core competency. A PM must: discern and debate ethical issues; explain own ethical standpoint; manage the ethics of the situation.

### 9.3 Ethical Concerns by Project Phase

| Phase | Ethical Concerns |
|---|---|
| **Initiation & Feasibility** | Falsifying estimates (cost, time, ROI) to win approval |
| **Planning & Organisation** | Low-balling bids, bribery, false claims of competence, discrimination |
| **Implementation** | Hiding info, conflicts of interest, expense padding, unsafe shortcuts |
| **Closing** | Avoiding accountability, hiding project failure, breaking commitments |

### 9.4 PMI EDMF (5 steps)

PMI's Ethical Decision-Making Framework:

| Step | Action | Key Questions |
|---|---|---|
| 1. Assessment | Gather all facts | Align with: law? PMI Code? Employer's code? Client's code? Your values? Culture? |
| 2. Alternatives | List possible choices | What are the pros and cons of each? |
| 3. Analysis | Test candidate decision | Positive impact or prevent harm? Will it seem good in a year? Am I free from bias? |
| 4. Application | Check against PMI values | Consistent with: **Responsibility, Respect, Fairness, Honesty**? |
| 5. Action | Decide and act | Can you accept responsibility? Would you make this public? |

**Case examples using EDMF:**
- Client says "hide the bug from CEO" (Case 20): Violates Honesty, Responsibility, Fairness. Diplomatically refuse; frame the bug fix as good PM.
- Test report falsified from "3 failed" to "0 failed" (Case 21): Assessment (verify facts), Analysis (falsifying harms client/users), Application (violates Honesty/Responsibility). Private conversation first, escalate if intentional.
- Budget $15K over, boss says don't tell client (Case 23): Honesty requires disclosure. Present options to client (cut scope, extend timeline, approve additional cost). Telling after the fact removes their ability to choose.

### 9.5 ACS Code of Ethics

**#1: The Primacy of the Public Interest** -- place interests of the public above personal, business, or sectional interests.

"Professionals are expected to promote good while working within ethical constraints."

### 9.6 Ethical Principles (Beneficence, Non-maleficence, Autonomy)

| Principle | Meaning |
|---|---|
| **Beneficence** | Do good; promote well-being |
| **Non-maleficence** | Do no harm |
| **Autonomy** | Respect individual choice and consent |

**Alice Library Analytics Case Study:** Library analytics system identifies usage patterns among female tech students. Tests:
- Beneficence: Does the system promote well-being? Could targeted services help?
- Non-maleficence: Could profiling cause harm? Stigmatisation? Privacy violation?
- Autonomy: Do users know their data is being analysed? Can they opt out?

### 9.7 Ethical Approaches (Utilitarianism vs Deontological)

| Approach | Core Question | Answer | Weakness |
|---|---|---|---|
| **Utilitarianism** | What produces the greatest good for the greatest number? | Choose action with best overall outcome | Can justify harming minorities for majority benefit |
| **Deontological** | Is the action itself morally right, regardless of outcome? | Follow moral rules/duties (e.g., never lie, never use people as means) | Rigid rules may lead to worse outcomes |

**Trolley Problem Application:**
- Utilitarian: pull the lever (save 5, sacrifice 1 = net positive)
- Deontologist: don't pull (deliberately killing is wrong regardless of outcome)

**Case example (Addictive Algorithm, Case 22):** Algorithm increases sales 30% by exploiting psychological weaknesses.
- Utilitarian: might approve (more revenue, jobs)
- Deontologist: reject (exploiting users treats them as means, violating autonomy)
- ACS: Public interest first; addictive patterns harm well-being
- Best exam answer: acknowledge both perspectives, argue non-maleficence and autonomy should prevail. Propose: keep algorithm but add transparency and opt-out controls.

### 9.8 Ethics in/by/for Design

| Perspective | Question | Focus |
|---|---|---|
| **Ethics in Design** | What is the system's goal? What are its likely consequences? | Purpose and impact of the technology |
| **Ethics by Design** | Even if the goal is good, are the MEANS ethical? | How the system achieves its goal |
| **Ethics for Designers** | What motivates the designer? Why this approach? | Intent and motivation of the builders |

**Intended vs Unintended Consequences:** Ethics in/by/for Design must consider both. A system designed with good intent (beneficence) may have unintended negative consequences (non-maleficence failure). Ethical review should anticipate both.

### 9.9 AI & Responsibility Gap

If an AI system makes a decision that causes harm, who is responsible? The developer? The deployer? The user? The AI itself?

This is the **Responsibility Gap** -- traditional ethical frameworks assign responsibility to human agents, but AI decisions may not have a clear human decision-maker.

**Key considerations:**
- AI systems are tools built by humans -- ultimate responsibility rests with humans
- The chain of responsibility includes: designers, developers, deployers, operators
- Risk management approaches (Francis & Armstrong 2003): ethical culture starts from top, supported by policies
- Permitting risky behaviour (Altham 1983): zero-risk would paralyse; must determine acceptable probability

---

## 10. Procurement

### 10.1 SOW / RFP / RFQ

| Document | Full Name | Purpose |
|---|---|---|
| **SOW** | Statement of Work | Describes the work to be performed -- deliverables, timelines, requirements, performance standards |
| **RFP** | Request for Proposal | Sent to potential vendors asking them to propose a solution and pricing for the defined scope |
| **RFQ** | Request for Quotation | Sent to vendors asking for a price quote for specific, well-defined goods or services |

**Bidders' Conference:** A meeting where prospective vendors can ask questions about the SOW/RFP to ensure they understand requirements before submitting proposals.

### 10.2 Vendor Selection (WSM)

**Weighted Scoring Model (WSM):**

Score = Sum of (Weight x Rating) for each criterion

Steps:
1. Define evaluation criteria (e.g., cost, experience, technical fit, timeline)
2. Assign weights to each criterion (must total 100%)
3. Rate each vendor on each criterion (e.g., 1-10 scale)
4. Calculate weighted score for each vendor
5. Select vendor with highest total score

**Example:**

| Criterion | Weight | Vendor A Rating | Vendor A Score | Vendor B Rating | Vendor B Score |
|---|---|---|---|---|---|
| Cost | 30% | 8 | 2.4 | 6 | 1.8 |
| Experience | 25% | 7 | 1.75 | 9 | 2.25 |
| Technical Fit | 25% | 6 | 1.5 | 8 | 2.0 |
| Timeline | 20% | 9 | 1.8 | 7 | 1.4 |
| **Total** | 100% | | **7.45** | | **7.45** |

---

## 11. PMBOK 7 Performance Domains

### 11.1 Eight Domains Overview

| Domain | Focus |
|---|---|
| **Stakeholder** | Identify, engage, and manage stakeholder expectations |
| **Team** | Build, develop, and lead the project team |
| **Development Approach & Life Cycle** | Select the right approach (predictive, agile, hybrid) |
| **Planning** | Establish scope, schedule, cost, quality, resources, communications, risk plans |
| **Project Work** | Execute and manage the work to deliver value |
| **Delivery** | Deliver the intended value and outcomes |
| **Measurement** | Monitor and control performance against plans |
| **Uncertainty** | Manage risks, ambiguity, and complexity |

### 11.2 Planning Process Group

Purpose: Establish scope, define objectives, develop action plan.

Sub-processes (2A-2I):
- 2A: Develop Project Management Plan
- 2B: Plan Scope Management
- 2C: Collect Requirements
- 2D: Define Scope
- 2E: Create WBS
- 2F: Plan Schedule Management
- 2G: Plan Cost Management
- 2H: Plan Quality Management
- 2I: Plan Resource Management

### 11.3 Executing Process Group

Purpose: Complete work per plan, coordinate resources, manage stakeholder expectations.

Key activities:
- Direct and manage project work
- Manage project knowledge
- Manage quality assurance
- Acquire and develop project team
- Manage communications
- Conduct procurements
- Manage stakeholder engagement

### 11.4 Integration Across Domains

| Domain | What to Include |
|---|---|
| Risk (Uncertainty) | Register + responses |
| Time (Schedule) | Milestones, critical path, schedule variance measures |
| Cost | Budget estimates, cost variance measures, contingency linked to risks |
| Scope (Delivery) | Deliverables in WBS, linked to risk of scope creep |
| Quality | Quality objectives, defect measures, linked KPIs |
| Resources (Team) | Resource availability risks, workload measures |
| Stakeholders | Stakeholder risks, engagement measures, communication KPIs |

---

## 12. Case Studies

### 12.1 FBI Virtual Case File ($170M failure)

**Background:** FBI's attempt to modernise its case management system after 9/11.

**Key Facts:**
- Cost: $170 million
- Duration: 4 years
- Outcome: Completely abandoned

**What went wrong:**
- Used Waterfall methodology for requirements that were rapidly evolving post-9/11
- Requirements changed continuously as new security needs emerged
- No iterative feedback loops -- built the entire system before testing with users
- By the time the system was complete, requirements had fundamentally changed
- Classic case of using the wrong lifecycle approach for a high-uncertainty project

**Lesson:** Waterfall fails when requirements are volatile. A Stacey analysis would have shown high uncertainty on both agreement (post-9/11 changing priorities) and technology axes, indicating Agile or at minimum Hybrid was needed.

### 12.2 Optus Outage (Nov 2023)

**Background:** Nationwide telecommunications outage on November 8, 2023.

**Key Facts:**
- Cause: Software update gone wrong
- No integration testing was performed before deployment
- No failover mechanisms activated
- Nationwide impact -- millions of customers affected
- Critical services (emergency calls, banking) disrupted

**Risk Management Failures:**
- No adequate testing strategy (Mitigate failure)
- No rollback plan (Accept without contingency)
- No failover/redundancy (Avoid failure -- risk was not eliminated through redundancy)
- Single point of failure in network architecture

**Connections to course:**
- Risk analysis has ontological (state of the world) and epistemological (knowledge) components -- Optus failed on both
- Risk management is normative: what OUGHT to be done -- Optus knew but didn't do
- Demonstrates why integration testing and failover are not optional for critical infrastructure

### 12.3 Alice Library Analytics (Ethics)

**Scenario:** A university library deploys an analytics system that identifies a behavioural pattern among female students studying technology courses.

**Ethical Analysis:**

| Principle | Test |
|---|---|
| **Beneficence** | Could targeted services benefit these students? Yes, potentially. |
| **Non-maleficence** | Could profiling cause harm? Stigmatisation? Privacy violation? Yes, potentially. |
| **Autonomy** | Do users know their data is analysed? Can they opt out? Critical question. |

**Ethics in/by/for Design Application:**
- Ethics in Design: Is the analytics system's goal (understanding usage patterns) ethical?
- Ethics by Design: Even if the goal is good, does profiling by gender cross ethical lines?
- Ethics for Designers: What motivates the library -- genuine student welfare or institutional metrics?

**Key takeaway:** The system may have good intentions but could produce unintended consequences. Ethical review must consider both intended and unintended impacts.

---

## 13. Reflective Writing

### 13.1 Gibbs' Reflective Cycle

Used for lessons learned and reflective writing assignments:

| Step | Question |
|---|---|
| 1. Description | What happened? |
| 2. Feelings | What were you thinking/feeling? |
| 3. Evaluation | What was good/bad about the experience? |
| 4. Analysis | Why did things go that way? What sense can you make of the situation? |
| 5. Conclusion | What else could you have done? What have you learned? |
| 6. Action Plan | What will you do differently next time? |

---

## 14. Quick Reference

### 14.1 Key Formulas

| Formula | Calculation |
|---|---|
| Stacey Score | Agreement (1-5) x Technology (1-5) |
| Risk Score | Likelihood (1-5) x Impact (1-5) |
| Three-Point Estimate (PERT) | (Optimistic + 4 x Most Likely + Pessimistic) / 6 |
| Velocity | Total Story Points completed in one sprint |
| Sprints Needed | Total Backlog SP / Average Velocity |
| Project Duration | Sprints Needed x Sprint Length |
| Team Effectiveness | Completed SP / Planned SP |
| WSM Vendor Score | Sum of (Weight x Rating) per criterion |

### 14.2 Strategy Selection Cheat Sheet

| Decision | Use This |
|---|---|
| How to run the project? | Stacey Matrix -> Predictive / Agile / Hybrid |
| Which Agile method? | Scrum (structured sprints) / Kanban (flow) / XP (quality) / SAFe (scale) |
| How to estimate cost? | Analogous -> Parametric -> Bottom-up (increasing accuracy) |
| How to prioritise features? | MoSCoW (scope) / Kano (satisfaction) / INVEST (story quality) |
| How to handle a risk? | Avoid / Mitigate / Transfer / Accept (threats) + Exploit / Enhance / Share (opportunities) |
| What leadership to use? | Match style to situation (6 styles + servant leadership) |
| How to solve ethical dilemma? | EDMF 5 steps + ACS Code + Utilitarianism vs Deontology |
| How to reflect on experience? | Gibbs' Reflective Cycle |
| How to decompose scope? | WBS (by deliverable or by phase) |
| How to forecast timeline? | Velocity + Story Points |
| How to select a vendor? | Weighted Scoring Model (WSM) |

### 14.3 Exam Q&A Patterns

**Pattern 1: "Which lifecycle?"**
- Assess Agreement and Tech on 1-5 scale -> calculate Stacey -> justify choice
- Always explain WHY, not just WHAT

**Pattern 2: "How would you handle this risk?"**
- State whether it's a threat or opportunity
- Choose strategy (Avoid/Mitigate/Transfer/Accept or Exploit/Enhance/Share)
- Give concrete action, not just the strategy name
- Assign an owner

**Pattern 3: "What leadership style?"**
- Match to situation (crisis -> directive, growth -> coaching, morale -> affiliative)
- Note that styles can be combined or shifted over time
- Default for Scrum Master = servant leadership

**Pattern 4: "Ethical dilemma"**
- Walk through EDMF 5 steps explicitly
- Check against: Responsibility, Respect, Fairness, Honesty
- Reference ACS Code (public interest first)
- Consider both Utilitarian and Deontological perspectives
- Recommend a course of action

**Pattern 5: "Scrum roles/events"**
- Know who decides WHAT (PO) vs HOW (Developers) vs removes blockers (SM)
- Know Review (product) vs Retrospective (process)
- Know that velocity is for forecasting, not comparing teams

**Pattern 6: "Budget cut / scope change"**
- Frame as triple constraint trade-off (scope vs cost vs time)
- Present options to client (reduce scope via MoSCoW, extend timeline, or reduce quality -- recommend against quality reduction)
- Be transparent with stakeholders

**Quick Decision Tree:**
```
"How certain are we?"
   Very certain        -> Predictive
   Somewhat uncertain  -> Hybrid
   Very uncertain      -> Agile
   Total chaos         -> Stop, re-scope first

"What Agile method?"
   Need structure + sprints    -> Scrum
   Unpredictable work flow     -> Kanban
   Need max code quality       -> XP
   Many teams (50+ people)     -> SAFe

"How to handle this risk?"
   Can we eliminate it?        -> Avoid
   Can we reduce it?           -> Mitigate
   Can someone else own it?    -> Transfer
   Is it too small to care?    -> Accept
   Is it a GOOD thing?         -> Exploit / Enhance / Share

"What leadership style now?"
   Crisis / emergency          -> Directive
   Teaching moment             -> Coaching
   Need team buy-in            -> Participative
   Morale is low               -> Affiliative
   High-performers, deadline   -> Pacesetting
   Big change, need vision     -> Visionary
   Scrum Master default        -> Servant Leadership

"Ethical dilemma?"
   -> EDMF: Assess -> Alternatives -> Analyse -> Apply -> Act
   -> Check: Responsibility, Respect, Fairness, Honesty
   -> ACS: Public interest first
```
