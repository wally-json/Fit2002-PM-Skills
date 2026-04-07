# Project Lifecycle Strategies

## Predictive (Waterfall)

Linear, sequential: Requirements → Design → Build → Test → Deploy.

**When to use:** Requirements clear and stable. Low uncertainty. Stacey 1-7. Regulatory projects needing mandatory documentation.

**Strengths:** Easy to manage. Clear milestones. Good for fixed-price contracts. Comprehensive documentation.

**Weaknesses:** Change expensive late. Customer sees product late. Risk of building the wrong thing. Bugs found late.

**Key phrase:** "Predictive works when you know WHAT and HOW before you start."

## Iterative

Build in repeated cycles. Each iteration refines and improves the previous version. Like sculpting.

**When to use:** High-level requirements known, details need exploration. Feedback needed to refine.

**Key distinction:** Iterative = revisit and improve the SAME thing. Incremental = add NEW pieces.

## Incremental

Deliver in pieces. Each increment adds new functionality. Like building a house.

**When to use:** Product divisible into independent chunks. Business wants early value.

**MVP connection:** MVP = first increment. Simplest version that delivers value and allows feedback.

## Agile

A mindset (not a method) combining iterative AND incremental delivery with frequent feedback.

**When to use:** Requirements uncertain or evolving. Stacey 8-20. Customer involvement available.

**Four Values (2001 Manifesto, Snowbird, Utah):**

| Prioritise | Over |
|---|---|
| Individuals & Interactions | Processes & Tools |
| Working Software | Comprehensive Documentation |
| Customer Collaboration | Contract Negotiation |
| Responding to Change | Following a Plan |

Items on the right still have value — we prioritise the left. "Working Software over Comprehensive Documentation" does NOT mean no documentation.

**Twelve Principles (grouped):**
- DELIVERY: Deliver early and often. Welcome change. Working product = progress measure. Simplicity.
- PEOPLE: Motivated individuals. Collaboration. Face-to-face. Sustainable pace.
- IMPROVEMENT: Attention to excellence. Self-organising teams. Regular reflection.

**Timeline:** 1930s Toyota Way → 1995 Scrum codified → 2001 Agile Manifesto → 2010s+ SAFe/Spotify at enterprise.

## Hybrid

Combining predictive and agile within the same project.

**When to use:** Some parts well-understood (predictive), others uncertain (agile).

**Case (UniPark):** Stacey 6 (Agreement=2, Tech=3) → Predictive zone, but UX uncertainty justified hybrid: predictive backend, Agile sprints for mobile frontend.

## Stacey Matrix

Developed by Ralph Stacey (2002). Determines suitable lifecycle approach.

**Score = Agreement (1-5) × Technology Complexity (1-5)**

| Score | Decision |
|---|---|
| 1-7 | Predictive/Incremental |
| 8-20 | Iterative/Agile |
| 21-25 | Delay or re-scope |

**Agreement Scoring:** 1=~100% agreement, 2=~80%, 3=~50%, 4=~30%, 5=almost none

**Technology Scoring:** 1=known tech done before, 2=known few challenges, 3=may need prototyping, 4=few known many unknowns, 5=~100% new

**Zones:** Simple (low/low) → Complicated → Complex → Chaos

**Examples:**

| Project | Agree | Tech | Score | Decision |
|---|---|---|---|---|
| WiFi Upgrade | 1 | 1 | 1 | Predictive |
| Bank Migration | 1 | 3 | 3 | Hybrid |
| Cafe App | 4 | 3 | 12 | Agile |
| AI Chatbot | 5 | 5 | 25 | Delay/Re-scope |

## SDLC Comparison

| Aspect | Predictive | Iterative | Incremental | Agile | Hybrid |
|---|---|---|---|---|---|
| Requirements | Fixed upfront | High-level, details evolve | Per increment | Evolving continuously | Mixed |
| Delivery | Single at end | Refined versions | Usable pieces | Each sprint | Varies |
| Change | Expensive | Moderate | Moderate | Embraced | Depends |
| Feedback | Late | Each iteration | Each increment | Every sprint | Mixed |
| Best for | Stable | Design exploration | Phased delivery | High uncertainty | Mixed certainty |
