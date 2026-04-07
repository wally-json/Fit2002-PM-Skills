# Roleplay Scenarios

Instructions for Claude:
1. Present the scenario and assign a role
2. Let the user respond with their decision
3. Challenge with "Why?" or introduce a complication
4. After 2-3 exchanges, debrief: frameworks used, what was missed, better alternatives
5. Reference specific knowledge base sections

---

## S1: The Hidden Bug [Ethics + Leadership]
**Role:** Project Manager
**Situation:** Your client calls you into a meeting. They say: "We found a critical bug in the payment module, but the CEO demo is tomorrow. Don't mention the bug — just demo the other features. We'll fix it after the demo."
**Follow-ups:**
- What if the CEO asks directly about the payment module?
- What if your job depends on keeping this client happy?
**Evaluation criteria:** EDMF 5 steps, PMI values (Honesty, Responsibility), leadership style choice
**Reference:** §9.4 Case 20

## S2: The Velocity Crisis [Scrum + Leadership]
**Role:** Scrum Master
**Situation:** Your team's velocity has dropped from 30 SP to 12 SP over the last two sprints. The Product Owner is frustrated and wants to add more developers. Two team members seem disengaged, and one senior developer has been arriving late consistently.
**Follow-ups:**
- The PO says "just add 3 more developers to catch up." How do you respond?
- During 1-on-1, the senior dev reveals they're job hunting. What now?
**Evaluation criteria:** Velocity analysis, leadership styles (affiliative → coaching), Tuckman stages, Brooks' Law
**Reference:** §2.1 Velocity, §8.1, §8.4

## S3: Production Down [Leadership]
**Role:** Team Lead
**Situation:** It's 2 AM. You get an alert: production is completely down. Your backend service is returning 500 errors. The on-call developer calls you panicking: "I don't know what happened! The database seems unreachable and I'm not sure what to check first."
**Follow-ups:**
- 30 minutes in, still not fixed. The CTO calls asking for an ETA. What do you say?
- The root cause was a configuration change pushed without review. How do you handle the post-mortem?
**Evaluation criteria:** Directive leadership, crisis communication, Gibbs' Reflective Cycle for post-mortem
**Reference:** §8.1 Case 15, §13.1

## S4: Budget Blowout [Ethics + Cost]
**Role:** Project Manager
**Situation:** You're managing a $85,000 project. At the 60% mark, you realise costs have already hit $80,000 with significant work remaining. Your boss says: "Don't tell the client yet. We'll absorb it and bring it up at the final invoice." The remaining work will cost approximately $15,000.
**Follow-ups:**
- The client calls asking "are we still on budget?" What do you say?
- Your boss threatens your performance review if you disclose.
**Evaluation criteria:** EDMF (Honesty), budget structure, contingency reserves, stakeholder communication
**Reference:** §9.4 Case 23, §5.5

## S5: Methodology Selection [Lifecycle]
**Role:** PM Consultant
**Situation:** A local cafe chain wants to build a mobile ordering app. The owner has strong opinions about features but keeps changing them weekly. The development team has never built a mobile app before. Agreement = 4, Technology = 3.
**Follow-ups:**
- The owner insists on Waterfall because "that's how proper projects are done." How do you convince them?
- They ask: "How long will this take and how much will it cost?" How do you estimate?
**Evaluation criteria:** Stacey Matrix (score 12 → Agile), lifecycle justification, estimation methods, managing stakeholder expectations
**Reference:** §1.6, §5.4

## S6: The Ethical Algorithm [Ethics]
**Role:** Product Owner
**Situation:** Your data science team has built a recommendation algorithm that increases sales by 30%. However, it works by exploiting psychological biases — creating urgency with false scarcity ("only 2 left!") and using dark patterns to make it harder to unsubscribe. The CEO loves the revenue numbers.
**Follow-ups:**
- A journalist contacts you asking about your "manipulative design practices." How do you respond?
- A team member raises concerns. Do you modify the algorithm? What do you keep/remove?
**Evaluation criteria:** Utilitarianism vs Deontological, Ethics in/by/for Design, ACS Code (public interest), Beneficence/Non-maleficence/Autonomy
**Reference:** §9.7 Case 22, §9.8, §9.6

## S7: Risk Materialised [Risk + Scrum]
**Role:** Scrum Master
**Situation:** Your only backend developer just called in — they'll be out for 3 weeks with a medical issue. You're mid-sprint with 4 backend stories in progress. The risk register had this listed as "Mitigate — pair programming" but pair programming was never actually implemented due to time pressure.
**Follow-ups:**
- The PO wants to bring in a contractor immediately. What are the risks of this approach?
- How do you restructure the current sprint?
**Evaluation criteria:** Risk response (mitigate failure), sprint replanning, risk register updates, honest assessment of what went wrong
**Reference:** §6.6, §2.1 Events

## S8: Scope Creep [Scope + Ethics]
**Role:** Project Manager
**Situation:** You're in Sprint 3 of 6. The client says: "I know we agreed on the original scope, but can you add real-time GPS tracking? It's essential." This feature wasn't in the scope statement, would add ~40 SP of work, and you're already using 90% of the budget. The client implies they'll give you more business in the future if you "just make it work."
**Follow-ups:**
- The client says "but your competitor said they'd include it for free." How do you respond?
- Your developer says they can hack it in but it won't be production-quality. Do you accept?
**Evaluation criteria:** Scope management (change control), MoSCoW reprioritisation, cost/schedule trade-offs, ethical boundaries (promises vs capability)
**Reference:** §3.2, §3.4, §7.1

## S9: Team Conflict [Leadership + Tuckman]
**Role:** Scrum Master
**Situation:** During Sprint Planning, two senior developers get into a heated argument about architecture. One wants microservices, the other wants a monolith. The argument becomes personal: "You always overcomplicate things!" "And you always take shortcuts!" The rest of the team has gone silent.
**Follow-ups:**
- After the meeting, both developers come to you separately to "explain their side." How do you handle this?
- At the next Daily Scrum, the tension is still visible. Team morale is dropping.
**Evaluation criteria:** Leadership style progression (affiliative → participative), Tuckman (storming), servant leadership
**Reference:** §8.1 Case 17, §8.4

## S10: The Failing Project [Lifecycle + Cost + Risk]
**Role:** PM Consultant (brought in to rescue)
**Situation:** A government agency hired a vendor 2 years ago to build a case management system using Waterfall. They're $2M over budget, 18 months behind schedule, and the delivered prototype doesn't match current requirements (which changed significantly since project start). The agency is considering abandoning the project.
**Follow-ups:**
- The vendor claims they followed the original spec exactly. Who's at fault?
- You recommend switching to Agile for the remaining work. The agency says "we need a fixed price and fixed date." How do you reconcile?
**Evaluation criteria:** FBI VCF parallels, Stacey analysis, sunk cost fallacy, hybrid approach, risk register
**Reference:** §12.1, §1.6, §5.2 (sunk costs)

## S11: Vendor Selection [Procurement]
**Role:** Project Manager
**Situation:** You're selecting a vendor for your cloud infrastructure. Three vendors submitted proposals. Vendor A is cheapest but has no experience with your tech stack. Vendor B is most experienced but 40% more expensive. Vendor C is mid-price with decent experience but their timeline is 2 months longer. Your boss wants the cheapest option.
**Follow-ups:**
- How do you structure the WSM to justify your recommendation?
- Vendor A wins the contract (boss overrides you). 3 months in, they're struggling. What now?
**Evaluation criteria:** WSM setup, criteria weighting, stakeholder management, risk mitigation
**Reference:** §10.2, §6.6

## S12: The Optus Moment [Risk + Ethics]
**Role:** Release Manager
**Situation:** It's Friday afternoon. Your team wants to push a major network configuration change to production. The change hasn't gone through integration testing because "the test environment is down and won't be fixed until Monday." Your team lead says: "It's a simple change, we've done similar ones before. Let's push it and monitor over the weekend."
**Follow-ups:**
- You push the change. At 3 AM, services start failing nationwide. What's your immediate action plan?
- In the post-mortem, management asks "how did this happen?" What systemic failures do you identify?
**Evaluation criteria:** Risk analysis (mitigate vs accept), Optus parallels, integration testing necessity, failover planning
**Reference:** §12.2, §6.6

## S13: Agile at Scale [SAFe + Leadership]
**Role:** Agile Coach
**Situation:** A telco company with 12 Scrum teams (about 80 developers) is struggling with coordination. Teams are stepping on each other's code, sprint reviews are chaotic, and there's no alignment on priorities. Management asks you to "fix Agile" or they'll go back to Waterfall.
**Follow-ups:**
- Some teams resist SAFe, calling it "Waterfall in disguise." How do you address their concerns?
- PI Planning is scheduled. Two teams refuse to attend, saying it's a waste of time. What do you do?
**Evaluation criteria:** SAFe (ART, PI Planning), scaling justification, leadership (visionary + participative), change management
**Reference:** §2.5, §8.1

## S14: Library Analytics [Ethics]
**Role:** Data Analyst
**Situation:** You've built an analytics dashboard for your university library. The data reveals a distinct pattern: female students in technology courses visit the library 40% more than the average. Your manager wants to create a targeted marketing campaign specifically for this demographic. You notice the campaign mockup uses language that could feel patronising.
**Follow-ups:**
- A student group files a complaint about "being profiled." How do you respond?
- How would you redesign the analytics to respect autonomy while still providing value?
**Evaluation criteria:** Beneficence/Non-maleficence/Autonomy, Ethics in/by/for Design, intended vs unintended consequences
**Reference:** §12.3, §9.6, §9.8

## S15: Sprint Zero [Scrum + Risk]
**Role:** Scrum Master
**Situation:** Your team is starting a new IoT project. The tech stack is unfamiliar (new sensor hardware, new cloud platform). The PO wants to jump straight into Sprint 1 with user-facing features. You believe a Sprint 0 for technical spikes and proof-of-concept is necessary, but the PO argues "Sprint 0 delivers no business value."
**Follow-ups:**
- The CEO asks why no features were delivered in the first 2 weeks. How do you explain Sprint 0's value?
- During Sprint 0, the proof-of-concept fails. The sensor data integration doesn't work as expected. What now?
**Evaluation criteria:** Risk mitigation (technical spikes), Stacey analysis, PO vs SM responsibilities, sprint backlog negotiation
**Reference:** §6.6, §2.1 Roles, §1.6
