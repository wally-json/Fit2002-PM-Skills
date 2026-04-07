# Quiz Bank

Instructions for Claude: Present ONE question at a time. Wait for user answer. Then reveal correct answer with explanation. Track score.

---

## Section 1: Project Lifecycle (10 questions)

### Q1 [Lifecycle]
A project has Agreement=4 and Technology=3 on the Stacey Matrix. Which approach is most appropriate?
A) Predictive
B) Incremental
C) Agile
D) Delay and re-scope

**Answer: C**
Stacey Score = 4×3 = 12 (range 8-20 → Agile). A/B wrong: score >7. D wrong: score <21.
See: §1.6 Stacey Matrix

### Q2 [Lifecycle]
Which statement best describes the difference between iterative and incremental approaches?
A) Iterative adds new features each cycle; incremental refines existing ones
B) Iterative refines the same thing each cycle; incremental adds new pieces
C) They are the same thing with different names
D) Iterative is for software only; incremental is for hardware

**Answer: B**
Iterative = revisit and improve the SAME thing. Incremental = add NEW pieces each cycle.
See: §1.2, §1.3

### Q3 [Lifecycle]
A data centre upgrade has clear requirements and well-known technology (Agreement=1, Tech=1). Which lifecycle?
A) Agile
B) Hybrid
C) Predictive
D) Delay and re-scope

**Answer: C**
Stacey = 1×1 = 1 (range 1-7 → Predictive). Requirements clear, tech known.
See: §1.1, §1.6

### Q4 [Lifecycle]
Which Agile value states that items on the right "still have value"?
A) Only left-side items matter
B) Right-side items are deprecated
C) Items on the right still have value, but we prioritise the left
D) Right-side items are only for waterfall projects

**Answer: C**
The Manifesto explicitly states items on the right still have value. "Working Software over Comprehensive Documentation" does NOT mean no documentation.
See: §1.4

### Q5 [Lifecycle]
A project has Stacey Score of 23. What should you do?
A) Use Scrum
B) Use Waterfall with extra documentation
C) Use Hybrid
D) Delay or re-scope the project

**Answer: D**
Score 21-25 = Chaos zone. Too risky to proceed. Must re-scope or delay.
See: §1.6

### Q6 [Lifecycle]
The UniPark project scored Stacey 6 but used a hybrid approach. Why?
A) The PM didn't understand Stacey
B) Backend was stable (predictive) but UX needed iteration (agile)
C) The client demanded Agile
D) Hybrid is always better than predictive

**Answer: B**
Stacey 6 suggests predictive, but UX uncertainty justified hybrid: predictive backend, Agile frontend.
See: §1.5

### Q7 [Lifecycle]
What is an MVP in the context of incremental delivery?
A) The final complete product
B) The most valuable phase
C) The first increment — simplest version that delivers value and allows feedback
D) A prototype that is never released

**Answer: C**
MVP = Minimum Viable Product = first increment. Simplest version delivering value.
See: §1.3

### Q8 [Lifecycle]
When was the Agile Manifesto created?
A) 1995 at Toyota
B) 2001 at Snowbird, Utah
C) 2010 at a SAFe conference
D) 1930s as part of Lean thinking

**Answer: B**
2001, Snowbird, Utah, by 17 software leaders. 1995 = Scrum codified. 1930s = Toyota Way.
See: §1.4

### Q9 [Lifecycle]
In a predictive project, when does the customer typically first see a working product?
A) After each sprint
B) After each iteration
C) Late in the project, after build and test phases
D) During requirements gathering

**Answer: C**
Predictive delivers a single product at the end. Customer sees working product late.
See: §1.1

### Q10 [Lifecycle]
Which Agile principle group includes "sustainable pace"?
A) Delivery
B) People
C) Improvement
D) Planning

**Answer: B**
PEOPLE group: Motivated individuals, collaboration, face-to-face, sustainable pace.
See: §1.4

---

## Section 2: Agile Frameworks (12 questions)

### Q11 [Scrum]
Who decides WHAT to build in Scrum?
A) Scrum Master
B) Developers
C) Product Owner
D) Stakeholders

**Answer: C**
PO defines WHAT to build, owns backlog, maximises value. Developers decide HOW.
See: §2.1 Roles

### Q12 [Scrum]
What is the maximum duration of a Daily Scrum?
A) 30 minutes
B) 1 hour
C) 15 minutes
D) As long as needed

**Answer: C**
Daily Scrum = 15 minutes max. Sync progress, surface blockers.
See: §2.1 Events

### Q13 [Scrum]
Sprint velocity is used to:
A) Compare performance between teams
B) Measure individual developer productivity
C) Forecast future sprints
D) Determine developer bonuses

**Answer: C**
Velocity is for FORECASTING, not comparing teams. Teams calibrate differently.
See: §2.1 Velocity

### Q14 [Scrum]
A sprint produced 4 stories totalling 10 SP. Story 1 (3 SP) completed, Story 2 (2 SP) rejected, Story 3 (1 SP) completed, Story 4 (4 SP) partial. What is the velocity?
A) 10 SP
B) 6 SP
C) 4 SP
D) 3 SP

**Answer: C**
Only fully completed items count. 3 + 1 = 4 SP. Rejected and partial = 0.
See: §2.1 Velocity Analysis

### Q15 [Scrum]
The Sprint Review focuses on:
A) The process — how the team worked
B) The product — what was built
C) Individual performance reviews
D) Planning the next sprint

**Answer: B**
Review = PRODUCT (demo to stakeholders). Retrospective = PROCESS.
See: §2.1 Sprint Review vs Retrospective

### Q16 [Scrum]
Which Scrum artifact ensures quality consistency?
A) Product Backlog
B) Sprint Backlog
C) Definition of Done (DoD)
D) Burndown Chart

**Answer: C**
DoD = shared quality checklist agreed by the whole team. Without it, quality is inconsistent.
See: §2.1 Artifacts

### Q17 [Scrum]
The three pillars of Scrum are:
A) Plan, Execute, Review
B) Transparency, Inspection, Adaptation
C) Speed, Quality, Cost
D) Backlog, Sprint, Increment

**Answer: B**
Empiricism foundation: Transparency (visible work), Inspection (examine progress), Adaptation (adjust quickly).
See: §2.1 Theory

### Q18 [Kanban]
What does WIP limit mean in Kanban?
A) Work in Progress — maximum items in each column
B) Weekly Iteration Plan
C) Workflow Integration Process
D) Work Input Priority

**Answer: A**
WIP = Work in Progress. Limiting WIP prevents overload and helps identify bottlenecks.
See: §2.2

### Q19 [Kanban]
Which metric measures time from request to delivery?
A) Cycle Time
B) Lead Time
C) Throughput
D) Velocity

**Answer: B**
Lead Time = request to delivery. Cycle Time = work started to finished. Throughput = items/period.
See: §2.2

### Q20 [Lean]
Which of these is NOT one of the Seven Wastes in Lean (IT context)?
A) Building features nobody asked for
B) Developers waiting for approvals
C) Writing unit tests
D) Switching between too many tasks

**Answer: C**
Writing tests is quality practice, not waste. A=Overproduction, B=Waiting, D=Motion.
See: §2.3

### Q21 [XP]
Which XP practice requires writing the test BEFORE the code?
A) Pair Programming
B) Continuous Integration
C) Test-Driven Development (TDD)
D) Refactoring

**Answer: C**
TDD = write test first, then write code to pass it.
See: §2.4

### Q22 [SAFe]
SAFe's Program Increment (PI) Planning is:
A) A daily standup for large teams
B) A 2-day face-to-face event where all teams align
C) A retrospective held monthly
D) A release review with stakeholders

**Answer: B**
PI Planning = 2-day face-to-face alignment for the entire ART (50-125 people).
See: §2.5

---

## Section 3: Scope & Cost (10 questions)

### Q23 [Scope]
Product scope vs project scope: which focuses on "what the product does"?
A) Project scope
B) Product scope
C) Both are the same
D) Neither

**Answer: B**
Product scope = features/functions. Project scope = work required to deliver.
See: §3.1

### Q24 [WBS]
What is the lowest level of a WBS?
A) Project
B) Major Phase
C) Work Package
D) Task

**Answer: C**
Work Package = smallest estimable/assignable unit. Tasks/Activities are below but the WBS hierarchy bottoms at work packages.
See: §3.5

### Q25 [User Story]
Which INVEST criterion means "can be developed in any order"?
A) Independent
B) Negotiable
C) Valuable
D) Small

**Answer: A**
I = Independent (any order), N = Negotiable, V = Valuable, E = Estimable, S = Small, T = Testable.
See: §3.6

### Q26 [Cost]
Which cost type is "already spent and cannot be recovered"?
A) Fixed cost
B) Indirect cost
C) Sunk cost
D) Variable cost

**Answer: C**
Sunk cost = already spent, unrecoverable. Example: money spent on abandoned prototype.
See: §5.2

### Q27 [Cost]
PERT estimate formula: Optimistic=3, Most Likely=5, Pessimistic=12. What is the estimate?
A) 6.7 days
B) 5.8 days
C) 5.0 days
D) 7.5 days

**Answer: B**
(3 + 4×5 + 12) / 6 = (3+20+12)/6 = 35/6 = 5.83 ≈ 5.8 days.
See: §5.4

### Q28 [Cost]
Which estimation method has the accuracy range of -5% to +10%?
A) Analogous
B) Parametric
C) Bottom-Up
D) Three-Point

**Answer: C**
Bottom-Up = Definitive (-5% to +10%). Analogous = ROM (-50% to +100%). Parametric = -10% to +25%.
See: §5.4

### Q29 [Cost]
Contingency reserve is for:
A) Unknown unknowns
B) Known unknowns (identified risks)
C) Project profit margin
D) Team bonuses

**Answer: B**
Contingency = known risks ("known unknowns"), owned by PM. Management Reserve = unknown unknowns.
See: §5.1, §5.5

### Q30 [Cost]
Budget structure: Cost Baseline + ? + Management Reserve = Total Budget
A) Profit margin
B) Contingency Reserve
C) Overhead costs
D) Tax

**Answer: B**
Cost Baseline + Contingency Reserve + Management Reserve = Total Project Budget.
See: §5.5

### Q31 [Time]
Tasks on the critical path have:
A) Maximum float
B) Zero float
C) Negative float
D) Variable float

**Answer: B**
Critical path tasks = zero float. Any delay directly delays the project.
See: §4.1

### Q32 [Scope]
What does the Requirements Traceability Matrix (RTM) ensure?
A) Budget stays on track
B) Every requirement is tracked from origin to validation
C) Team attendance is logged
D) Risks are prioritised

**Answer: B**
RTM tracks each requirement from origin → implementation → validation. Nothing missed, nothing unjustified.
See: §3.3

---

## Section 4: Risk Management (10 questions)

### Q33 [Risk]
What is the difference between a risk and an issue?
A) Risks are bigger than issues
B) Risks are in the FUTURE; issues are happening NOW
C) Issues are more expensive
D) There is no difference

**Answer: B**
Risk = FUTURE uncertain event. Issue = current problem you're already facing.
See: §6.1

### Q34 [Risk]
Risk Score = Likelihood 4 × Impact 5 = 20. This is classified as:
A) Low — monitor
B) Medium — plan response
C) High — act immediately
D) Critical — stop project

**Answer: C**
15-25 = High → act immediately. 6-14 = Medium. 1-5 = Low.
See: §6.5

### Q35 [Risk]
Your app stores credit card data. The best risk response is:
A) Avoid — remove payment feature
B) Mitigate — encrypt the data
C) Transfer — use a PCI-DSS compliant provider like Stripe
D) Accept — monitor for breaches

**Answer: C**
Transfer the risk to a specialist (Stripe) who handles PCI compliance.
See: §6.6

### Q36 [Risk]
A vendor might increase prices by 40%. Which response?
A) Accept — nothing you can do
B) Avoid — cancel the project
C) Mitigate — lock in a fixed-price contract
D) Transfer — buy insurance

**Answer: C**
Mitigate by locking in a fixed-price contract (reduces impact). Could also Avoid by switching vendor.
See: §6.6

### Q37 [Risk]
A competitor might shut down, creating an opportunity. Which strategy?
A) Avoid
B) Accept
C) Enhance — prepare a migration guide NOW
D) Mitigate

**Answer: C**
This is an OPPORTUNITY. Enhance = increase the chance/value by preparing in advance.
See: §6.6

### Q38 [Risk]
Which is NOT a common risk management mistake?
A) Confusing issues with risks
B) Only listing negative risks
C) Updating the risk register regularly
D) Using vague risk descriptions

**Answer: C**
Updating regularly is CORRECT practice. All others are common mistakes.
See: §6.8

### Q39 [Risk]
Every high/medium risk must have:
A) A Gantt chart entry
B) One named owner
C) A budget line item
D) A separate project plan

**Answer: B**
Every high/medium risk needs ONE named owner responsible for monitoring and response.
See: §6.8

### Q40 [Risk]
5% chance of a blurry icon on an old device. Best response?
A) Avoid
B) Mitigate
C) Transfer
D) Accept

**Answer: D**
Low likelihood, cosmetic only. Cost of response exceeds the risk. Accept and monitor.
See: §6.6

### Q41 [Risk]
Monte Carlo simulation is used in which type of risk analysis?
A) Qualitative
B) Quantitative
C) Risk identification
D) Risk planning

**Answer: B**
Quantitative analysis uses Monte Carlo (probability distribution) and Decision Trees.
See: §6.5

### Q42 [Risk]
The only backend developer might get sick. Best response?
A) Avoid — hire a second backend dev
B) Accept — hope they stay healthy
C) Mitigate — pair programming and documentation
D) Transfer — outsource backend

**Answer: C**
Mitigate by knowledge sharing (pair programming) and documentation to reduce impact.
See: §6.6

---

## Section 5: Leadership (8 questions)

### Q43 [Leadership]
Production is down and the team is panicking. Which leadership style?
A) Participative
B) Affiliative
C) Directive
D) Coaching

**Answer: C**
Crisis → Directive. "You check logs. You restart service. Go." Clear orders, immediate action.
See: §8.1

### Q44 [Leadership]
A new intern has never used Git. Which style?
A) Directive
B) Pacesetting
C) Coaching
D) Visionary

**Answer: C**
Teaching/mentoring moment → Coaching. Sit with them, show basics, focus on growth.
See: §8.1

### Q45 [Leadership]
Two developers had a heated argument. Which style first?
A) Directive
B) Affiliative
C) Pacesetting
D) Participative

**Answer: B**
After conflict → Affiliative. People first, rebuild trust, create harmony.
See: §8.1

### Q46 [Leadership]
Tuckman's "Storming" stage is characterised by:
A) Polite introductions
B) High-functioning delivery
C) Conflict and competing ideas
D) Established shared norms

**Answer: C**
Storming = conflict, competing ideas, power struggles. Leader should mediate/clarify roles.
See: §8.4

### Q47 [Leadership]
The Scrum Master's default leadership approach is:
A) Directive
B) Pacesetting
C) Servant Leadership
D) Visionary

**Answer: C**
SM = servant leader. "How can I help you succeed?" Remove impediments, no formal authority.
See: §8.2, §8.3

### Q48 [Leadership]
Which Tuckman stage matches Participative leadership?
A) Forming
B) Storming
C) Norming
D) Performing

**Answer: C**
Norming = shared norms, trust builds. Leader steps back, encourages collaboration → Participative.
See: §8.4

### Q49 [Leadership]
A PM assigns tasks, controls budget, and manages scope. A SM:
A) Does the same but in Agile
B) Has no formal authority and serves the team
C) Reports to the PM
D) Only handles technical decisions

**Answer: B**
SM has no formal authority. Influences through coaching. Serves the team, doesn't manage it.
See: §8.3

### Q50 [Leadership]
Which leadership style risks burnout?
A) Affiliative
B) Coaching
C) Pacesetting
D) Participative

**Answer: C**
Pacesetting sets a high bar. Risk: burnout and frustration if team can't keep up.
See: §8.1

---

## Section 6: Ethics (10 questions)

### Q51 [Ethics]
A client says "hide this bug from the CEO." Using EDMF, this violates:
A) Only Fairness
B) Honesty and Responsibility
C) Only Respect
D) No PMI values — it's a business decision

**Answer: B**
Hiding a bug violates Honesty (concealment) and Responsibility (duty to stakeholders).
See: §9.4

### Q52 [Ethics]
The ACS Code's #1 principle is:
A) Maximise profit
B) Protect company reputation
C) Primacy of the Public Interest
D) Follow management instructions

**Answer: C**
ACS #1: Place interests of the public above personal, business, or sectional interests.
See: §9.5

### Q53 [Ethics]
A test report was falsified from "3 failed" to "0 failed." First action?
A) Report to the police
B) Fire the person immediately
C) Private conversation to understand facts
D) Ignore it — tests aren't important

**Answer: C**
EDMF Step 1: Assessment — gather facts first. Have a private conversation. Escalate if intentional.
See: §9.4

### Q54 [Ethics]
The Trolley Problem: a utilitarian would:
A) Not pull the lever — killing is wrong
B) Pull the lever — save 5, sacrifice 1
C) Walk away — it's not their problem
D) Ask for consensus first

**Answer: B**
Utilitarian: greatest good for greatest number. Save 5 > sacrifice 1 = net positive.
See: §9.7

### Q55 [Ethics]
An algorithm increases sales 30% by exploiting psychological weaknesses. A deontologist would:
A) Approve — it increases revenue
B) Reject — exploiting users treats them as means, violating autonomy
C) Approve if revenue exceeds lawsuits
D) Ask shareholders to vote

**Answer: B**
Deontological: the action itself must be morally right. Exploiting people violates autonomy.
See: §9.7

### Q56 [Ethics]
"Ethics BY Design" asks:
A) What is the system's goal?
B) Are the MEANS of achieving the goal ethical?
C) What motivates the designer?
D) Is the system profitable?

**Answer: B**
Ethics IN design = goal/consequences. Ethics BY design = means. Ethics FOR designers = motivation.
See: §9.8

### Q57 [Ethics]
Budget is $15K over. Boss says don't tell the client. The ethical action is:
A) Agree — boss knows best
B) Disclose to client with options (cut scope, extend timeline, approve cost)
C) Quietly cut features to stay on budget
D) Resign from the project

**Answer: B**
Honesty requires disclosure. Present options so client can make informed choices.
See: §9.4

### Q58 [Ethics]
Helgadottir's three core PM skills are:
A) Technical, managerial, leadership
B) Creative, logical, ethical thinking
C) Planning, executing, monitoring
D) Communication, negotiation, conflict resolution

**Answer: B**
PM core = intersection of Creative + Logical + Ethical thinking.
See: §9.2

### Q59 [Ethics]
The "Responsibility Gap" in AI refers to:
A) Budget shortfalls in AI projects
B) Unclear who is responsible when AI causes harm
C) Skill gaps in AI teams
D) Time gaps between AI updates

**Answer: B**
When AI makes harmful decisions, traditional frameworks struggle to assign human responsibility.
See: §9.9

### Q60 [Ethics]
Non-maleficence means:
A) Do good
B) Do no harm
C) Respect autonomy
D) Maximise profit

**Answer: B**
Beneficence = do good. Non-maleficence = do no harm. Autonomy = respect choice.
See: §9.6

---

## Section 7: Procurement, PMBOK & Prioritisation (8 questions)

### Q61 [MoSCoW]
In MoSCoW, "Must have" features should consume approximately:
A) 100% of effort
B) 80% of effort
C) 60% of effort
D) 40% of effort

**Answer: C**
Must ~60%, Should ~20%, Could ~20%, Won't = documented for future.
See: §7.1

### Q62 [Kano]
A feature that users expect (absence causes dissatisfaction, presence doesn't excite) is:
A) Performance feature
B) Excitement feature
C) Basic (Must-be) feature
D) Luxury feature

**Answer: C**
Basic/Must-be: expected. Absence = dissatisfaction. Presence is neutral. Example: login works.
See: §7.3

### Q63 [Procurement]
An RFP is:
A) A request for vendors to quote a price for specific items
B) A request for vendors to propose a solution and pricing
C) A statement of work to be performed
D) A vendor evaluation scorecard

**Answer: B**
RFP = Request for Proposal (propose solution + pricing). RFQ = price quote. SOW = work description.
See: §10.1

### Q64 [Procurement]
In WSM vendor selection, if Cost (30%) rates Vendor A at 8, the weighted score is:
A) 8.0
B) 3.0
C) 2.4
D) 0.3

**Answer: C**
30% × 8 = 2.4. Weighted score = weight × rating.
See: §10.2

### Q65 [PMBOK]
Which PMBOK 7 domain focuses on managing risks and ambiguity?
A) Planning
B) Delivery
C) Uncertainty
D) Measurement

**Answer: C**
Uncertainty domain = manage risks, ambiguity, and complexity.
See: §11.1

### Q66 [Prioritisation]
When a 25% budget cut hits, which framework helps identify features to cut?
A) Kano Model
B) MoSCoW
C) INVEST
D) Stacey Matrix

**Answer: B**
MoSCoW: cut Could/Won't features first. Must haves are non-negotiable.
See: §7.1

### Q67 [Case Study]
The FBI Virtual Case File project failed primarily because:
A) The budget was too small
B) They used Waterfall for rapidly evolving requirements
C) The team was too large
D) They used too many Agile sprints

**Answer: B**
$170M, 4 years, abandoned. Used Waterfall when requirements were volatile post-9/11.
See: §12.1

### Q68 [Case Study]
The Optus outage (2023) was caused by:
A) A cyberattack
B) Hardware failure
C) A software update with no integration testing
D) A natural disaster

**Answer: C**
Software update gone wrong. No integration testing. No failover. No rollback plan.
See: §12.2

---

## Section 8: Reflective Writing & Cross-cutting (4 questions)

### Q69 [Gibbs]
In Gibbs' Reflective Cycle, which step asks "What will you do differently next time?"
A) Evaluation
B) Analysis
C) Conclusion
D) Action Plan

**Answer: D**
Action Plan = what will you do differently. Conclusion = what else could you have done.
See: §13.1

### Q70 [Cross-cutting]
Team velocity = 25 SP/sprint, total backlog = 150 SP, sprint length = 2 weeks. Project duration?
A) 6 weeks
B) 10 weeks
C) 12 weeks
D) 15 weeks

**Answer: C**
150/25 = 6 sprints × 2 weeks = 12 weeks.
See: §2.1 Velocity

### Q71 [Cross-cutting]
A PM notices sprint velocity dropping. Which is the WORST response?
A) Investigate estimation accuracy
B) Check for external blockers
C) Compare velocity to another team
D) Review for technical debt

**Answer: C**
Cannot compare velocity across teams — SP are calibrated per team. All others are valid investigations.
See: §2.1 Velocity

### Q72 [Cross-cutting]
Which combination of lifecycle approach and Agile method would suit a hospital software project where bugs could be life-threatening?
A) Predictive + Waterfall
B) Agile + Kanban
C) Agile + XP (TDD, pair programming, CI)
D) Hybrid + SAFe

**Answer: C**
When bugs = life-threatening, XP's TDD, pair programming, and CI catch defects early.
See: §2.4
