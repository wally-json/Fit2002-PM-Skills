# Risk Management

## Definitions

| Type | Time | Definition | Example |
|---|---|---|---|
| **Risk** | FUTURE | Uncertain event affecting objectives | "Developer might quit" |
| **Issue** | NOW | Problem already happening | "Missed last 2 deadlines" |
| **Assumption** | BELIEVED | Believed true, not confirmed | "API ready by Week 3" |

Two types: **Threats** (negative) and **Opportunities** (positive).

## Risk Management Process (6 steps)

1. **Plan** — define how risk management will be conducted
2. **Identify** — discover risks. Techniques: Brainstorming, Delphi, SWOT, Checklists
3. **Qualitative Analysis** — prioritise by impact × probability. Score = Likelihood (1-5) × Impact (1-5)
4. **Quantitative Analysis** — numerical assessment. Monte Carlo, Decision Trees
5. **Response Planning** — select strategies (see below)
6. **Monitor & Control** — track risks. Risk Audits, Reviews, Watch List. Every high/medium risk needs ONE owner.

## Risk Register

**Fields:** ID, Description, Category, Likelihood (1-5), Impact (1-5), Score, Owner, Strategy, Status, Notes

```
ID: R-1
Risk: IoT sensor data integration failure
Category: Technical
Likelihood: 3, Impact: 5, Score: 15 (High)
Owner: Lead Developer
Strategy: Mitigate — build proof-of-concept in Sprint 0
Status: Open
```

## Classification Categories

| Category | Example | Affects | Owner |
|---|---|---|---|
| Technical | API fails | Schedule, testing | Dev lead |
| Stakeholder | Client unresponsive in UAT | Approvals | PM |
| External | Policy change | Compliance, timeline | Sponsor |
| Resourcing | Key dev leaves | Velocity | SM |
| Opportunity | Tool upgrade saves time | Cost, schedule | PM |

## Qualitative Analysis

```
Score = Likelihood (1-5) × Impact (1-5)
1-5   = Low    → monitor
6-14  = Medium → plan response
15-25 = High   → act immediately
```

## Probability/Impact Matrix

```
              Impact
              Low    Medium    High
Probability
High         | Med  |  High  | High |  ← Act now
Medium       | Low  |  Med   | High |
Low          | Low  |  Low   | Med  |  ← Monitor
```

## Response Strategies

### For Threats

| Strategy | Action | Example | When |
|---|---|---|---|
| **Avoid** | Eliminate by changing plan | Remove high-risk feature | Too dangerous, can change scope |
| **Mitigate** | Reduce likelihood OR impact | Add testing, pair programming | Most common |
| **Transfer** | Pass to another party | Insurance, SLA, use Stripe for PCI | Someone else can own it |
| **Accept** | Do nothing, monitor | Low-impact cosmetic bug | Impact low, response costs more |

### For Opportunities

| Strategy | Action | Example |
|---|---|---|
| **Exploit** | Make it happen | Assign best dev to capture it |
| **Enhance** | Increase chance/value | Prepare migration guide before competitor shuts down |
| **Share** | Partner | Co-develop with another company |
| **Accept** | Welcome if it happens | Small opportunity, not worth investment |

## Case Examples

- Vendor price increase 40%: Mitigate (lock fixed-price) or Avoid (switch vendor)
- Only backend dev might get sick: Mitigate (pair programming, documentation)
- App stores credit card data: Transfer (PCI-DSS provider like Stripe)
- 5% chance blurry icon on old device: Accept (low likelihood, cosmetic)
- Competitor might shut down: Enhance (prepare migration guide NOW)

## Common Mistakes

- Confusing issues with risks
- Only listing threats (ignoring opportunities)
- Vague risks: "budget overrun" instead of "vendor invoice delays"
- Creating risk register once, never updating
- Not linking risks to schedule/cost/scope impacts
