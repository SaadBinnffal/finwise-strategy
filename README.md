# FinWise strategy

**Saad Binnffal**  
Product Analytics & Experimentation · Individual final project

This project proposes a 12-month growth and experimentation strategy for the fictional FinWise Co. The company has reached product-market fit with $10M ARR, approximately 2% trial-to-paid conversion, and 40% one-year paid retention.

**Growth thesis:** Help trial workspaces create a useful forecast from their own financial data, keep that forecast useful through meaningful reviews, and validate whether collaboration leads to sustained paid use and qualified introductions to another business.

The designs, growth loop, experiment targets, and pricing recommendations are hypotheses. No live experiment, customer interview, conversion lift, or retention improvement is claimed.

## Presentation

- [Open the HTML presentation](pitch.html) after downloading it or serving the repository.
- [Read the PDF presentation](pitch.pdf).
- [Read the speaker notes](pitch-notes.md).

The HTML is self-contained and uses embedded evidence images. Use Previous/Next or the arrow keys, Home/End, N for notes, and the Print/PDF button. Click a prototype or wireframe image to enlarge it. The presentation follows the course order: context and roadmap first, then M1-M6 on slides 5-10 and reflection on slide 11.

## Deliverables

| Module | Deliverable | Supporting evidence |
| --- | --- | --- |
| 1 · The Bet | [Growth hypothesis and bet](01-bet/growth-bet.md) | [Proposed collaboration loop](01-bet/FinWise_Collaboration_Loop.png) |
| 2 · The Solution | [Activation solution](02-solution/activation-solution.md) | [Local prototype](02-solution/finwise-onboarding.html) and four screen images |
| 3 · The Mechanic | [Engagement mechanic](03-mechanic/engagement-mechanic.md) | [Weekly review wireframe](03-mechanic/mechanic-wireframe.png) |
| 4 · The Signals | [Data signals](04-signals/data-signals.md) | [Dashboard](04-signals/finwise-metrics-dashboard.png), [correlation view](04-signals/import-vs-conversion.png), and [source values](04-signals/finwise-monthly-data.json) |
| 5 · The Validation | [Experiment brief](05-validation/experiment-brief.md) | Proposed workspace-level A/B design, success target, guardrail and read date |
| 6 · The Model | [Pricing memo](06-model/pricing-model.md) | Conditional packaging bet and the M4 model-completion signal |

## The Story

### Growth thesis

FinWise needs more useful first experiences and more sustained value from its existing trial inflow. My first bet is optional accountant or teammate review during onboarding. The proposed loop requires useful collaboration and repeat use before some collaborators might introduce another business. That last link remains unvalidated.

### One friction

I treated a required invitation or waiting step as a design risk: it could delay an owner who is ready to build a first forecast. I kept collaboration optional and allowed independent completion. This is a friction avoided in the prototype, not a finding from a live FinWise usability study.

### One Aha

The prototype's fictional Nook Studio example ends with $8,400, yet cash reaches a $7,000 low point below the owner's $8,000 buffer. The useful realization is about the timing of pressure, not just the ending balance. Whether this moment predicts retention still needs validation.

### What changed my thinking

I initially expected import usage to help explain payment conversion. Across the supplied 13 monthly aggregates, its Pearson correlation with the same-month trial-to-paid ratio is approximately -0.05. I revised the claim that this was a validated payment predictor and shifted attention to the linked path from import to first useful output, repeat use, and payment. Aggregate correlation does not establish user-level effects.

### Takeaways

- Separate observations from explanations. A low conversion rate does not establish a pricing or onboarding cause.
- Use meaningful behavior as the experiment outcome. An invitation or sample preview alone is not activation.
- Keep a commercial follow-up. Activation can improve without improving sustained paid use.
- Define the decision before the experiment starts. The M5 target, sample plan, guardrail, and read date are proposed rather than observed results.
- Retain pricing when evidence is insufficient. FinWise already uses a reverse trial. Audit entitlements and costs before changing the free/paid boundary.

## Metrics and evidence

The supplied table totals 94,558 visits, 6,424 trials, and 128 paid conversions. The table-total trial-to-paid ratio is 1.99%, and the monthly ratios stay between 1.87% and 2.08%. Trial-to-paid has the greatest proportional loss. Acquisition has the greater absolute loss.

The course North Star is the number of trial users who import financial data and reach their first modeling output. My proposed operational window is seven days using own-business data. For the collaboration experiment, randomize and analyze at workspace level. Map users to workspaces rather than mixing user-level and account-level denominators.

M4 Leading 1 is own-data import completion among trial starters. Leading 2 is first-model completion among successful importers by trial day 7 in the same cohort. These are candidate signals, not validated payment predictors. The reported Import and Modeling percentages have unspecified denominators and cannot reconstruct the joint North Star or the conditional second indicator.

Additional limitations:

- Paid counts may not belong to the same month's trial starters. Cohort-aligned payment events are needed.
- The annual churn column has an unspecified cohort. The scenario's 40% retention is a separate given.
- Revenue equals Paid times 78,125 in every supplied row. It is not an independent growth signal or a verified ARR series.
- Session duration alone does not establish value. The final drop in reported modeling usage needs a data-quality and cohort investigation.
- The invitation prototype simulates the action. A live experiment requires production permissions, events, and reliable assignment.

## Twelve-month execution plan

Proposed planning horizon: **November 2026 to October 2027**. No revenue projection is invented without unit economics and linked cohorts.

| Window | Work | Evidence required before expanding |
| --- | --- | --- |
| Months 1-2 · Nov-Dec | Verify event definitions, payment cohorts, costs and eligible recruitment. Implement the production invitation and run M5 if feasible. | Reliable assignment and own-data model events. The M5 plan proposes recruitment through 27 Dec and a 4 Jan 2027 read after full follow-up. |
| Months 3-5 · Jan-Mar | Read M5. Test the M3 progress bar after first forecast, with the same review functionality in both variants. Follow useful recurrence and paid cohorts. | Credible activation or review improvement, acceptable guardrails, and sufficient precision. No automatic rollout from an inconclusive result. |
| Months 6-8 · Apr-Jun | Audit entitlements and willingness to pay. Test the M6 boundary only if a verified first-value payment barrier exists. Keep invitation exposure equal across pricing variants. | Cohort revenue after discounts/refunds, servicing cost, conversion, and retained useful use. Keep base prices if the proposed path is already available. |
| Months 9-12 · Jul-Oct | Investigate cross-business collaboration introductions, then test a distribution loop if the earlier value and commercial links hold. | Qualified new-business trials, activation, retained paid outcomes, and cost per retained account. Reallocate acquisition spending only with durable evidence. |

## Decision rules

M5 proposes a +10 percentage-point activation target with credible statistical evidence, and a day-1 noncompletion deterioration margin of at most +2 points. Its initial 800-workspace sample estimate addresses the primary metric; the guardrail may require more precision. Confirm feasible recruitment and baselines before launch.

The pricing recommendation preserves the existing reverse trial and base prices. One editable forecast, optional review, and paid additional scenarios are proposed entitlements, not confirmed current features. If the path is already free, prioritize activation rather than a redundant pricing change. A post-expiry packaging change cannot explain a day-7 outcome before exposure.

Treat a guardrail breach or unresolved material harm as a reason to investigate. Record insufficient evidence as inconclusive. Follow trial-to-paid conversion and later paid retention before claiming sustainable revenue growth.

## Submission

Commit the six module folders, this README, and pitch.html to the course repository. Submit the repository URL plus the HTML/PDF presentation on the Learning Platform. Keep the repository private and grant the instructor access as directed by the course.

The course brief sets the written-feedback deadline at seven days after the cohort ends. This package does not claim a GitHub commit, publishing action, instructor-access change, or Learning Platform submission.
