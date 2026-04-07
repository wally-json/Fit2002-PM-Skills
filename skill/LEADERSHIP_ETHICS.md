# Leadership & Ethics

## Six Leadership Styles (Margules 2011)

| Style | Core Behaviour | Best When | Danger |
|---|---|---|---|
| **Directive** | "Do this now." Clear orders. | Crisis, tight deadline, new team | Micromanagement |
| **Coaching** | "Let me help you grow." Mentoring. | Developing junior members | Too slow for urgent results |
| **Participative** | "What does everyone think?" Shared decisions. | Team has expertise, buy-in needed | Delays if no consensus |
| **Affiliative** | "People first." Harmony, trust. | Low morale, after conflict | Avoids tough conversations |
| **Pacesetting** | "Follow my example." High bar. | Expert team, tight delivery | Burnout |
| **Visionary** | "Imagine where we're going." Inspires. | Change initiatives, new projects | Needs credibility |

### Case Examples

- Production down, team panicking → **Directive**: "You check logs. You restart service. Go."
- New intern, never used Git → **Coaching**: sit with them, show basics
- Two devs had heated argument → **Affiliative**: people first, rebuild trust
- Architecture decision, everyone has opinions → **Participative**: facilitate discussion
- Company pivoting desktop to mobile → **Visionary**: paint big picture
- Sprint going badly → Combination: affiliative → coaching → directive if deadline-critical

## Servant Leadership (Greenleaf 1970)

"The servant-leader is servant first."

- "How can I help you succeed?" NOT "Did you finish the task?"
- Remove impediments, create psychological safety, listen before directing
- Aligns with Coaching + Affiliative styles
- **Default for Scrum Master**

## PM vs Scrum Master

| Aspect | Project Manager | Scrum Master |
|---|---|---|
| Focus | Scope, schedule, budget | Facilitating Scrum, empowering team |
| Authority | Budget and resources | No formal authority; influence |
| Approach | Plan-driven | Servant leader |
| Decision-making | Makes key decisions | Helps team decide |

## Tuckman's Team Development

| Stage | Description | Leader Action |
|---|---|---|
| **Forming** | Polite, uncertain, testing boundaries | Directive: clear direction, ground rules |
| **Storming** | Conflict, competing ideas, frustration | Coaching/Affiliative: mediate, clarify roles |
| **Norming** | Shared norms, trust builds | Participative: step back, encourage |
| **Performing** | High-functioning, self-organising | Servant leadership: delegate, remove obstacles |

## MBTI

| Dimension | Poles | PM Relevance |
|---|---|---|
| Energy | Introvert (I) / Extrovert (E) | Communication preferences |
| Information | Sensing (S) / iNtuitive (N) | Detail vs big-picture |
| Decision | Thinking (T) / Feeling (F) | Logic vs values |
| Lifestyle | Judging (J) / Perceiving (P) | Structured vs flexible |

---

# Ethics

## Morality vs Ethics vs Law

| Concept | Definition |
|---|---|
| **Morality** | Personal principles about right/wrong |
| **Ethics** | Philosophy examining moral principles; professional codes |
| **Law** | Formal rules, state-enforceable |

Can misalign: lawful may be immoral; unlawful may be considered moral by some.

## Helgadottir's Three Core PM Skills (2008)

PM core = intersection of **Creative thinking** + **Logical thinking** + **Ethical thinking**.

A PM must: discern ethical issues, explain own standpoint, manage the ethics of the situation.

## Ethical Concerns by Phase

| Phase | Concerns |
|---|---|
| Initiation | Falsifying estimates to win approval |
| Planning | Low-balling bids, bribery, false competence claims |
| Implementation | Hiding info, conflicts of interest, unsafe shortcuts |
| Closing | Avoiding accountability, hiding failure |

## PMI EDMF (5 Steps)

| Step | Action | Key Questions |
|---|---|---|
| 1. Assessment | Gather facts | Align with: law? PMI Code? Employer? Client? Values? |
| 2. Alternatives | List choices | Pros and cons of each? |
| 3. Analysis | Test decision | Positive impact? Look good in a year? Free from bias? |
| 4. Application | Check PMI values | **Responsibility, Respect, Fairness, Honesty** |
| 5. Action | Decide and act | Accept responsibility? Make this public? |

### Case Examples

- Client: "hide the bug from CEO" → Violates Honesty/Responsibility. Diplomatically refuse.
- Test report falsified (3→0 failed) → Assessment → Analysis → Violates Honesty. Private conversation, escalate if intentional.
- Budget $15K over, boss says don't tell client → Honesty requires disclosure. Present options.

## ACS Code of Ethics

**#1: Primacy of the Public Interest** — place public interests above personal/business interests.

## Ethical Principles

| Principle | Meaning |
|---|---|
| **Beneficence** | Do good; promote well-being |
| **Non-maleficence** | Do no harm |
| **Autonomy** | Respect individual choice and consent |

## Ethical Approaches

| Approach | Core Question | Weakness |
|---|---|---|
| **Utilitarianism** | Greatest good for greatest number? | Can justify harming minorities |
| **Deontological** | Is the action itself morally right? | Rigid rules, worse outcomes possible |

**Trolley Problem:** Utilitarian pulls lever (save 5); Deontologist doesn't (killing is wrong regardless).

## Ethics in/by/for Design

| Perspective | Question |
|---|---|
| Ethics **in** Design | What's the system's goal? Consequences? |
| Ethics **by** Design | Are the MEANS ethical? |
| Ethics **for** Designers | What motivates the designer? |

Must consider intended AND unintended consequences.

## AI & Responsibility Gap

If AI causes harm, who's responsible? Developer? Deployer? User? The AI?

- AI = tools built by humans → ultimate responsibility rests with humans
- Chain: designers → developers → deployers → operators
- Zero-risk would paralyse; must determine acceptable probability
