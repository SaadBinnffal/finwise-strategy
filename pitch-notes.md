# FinWise presentation notes

## 1. FinWise growth strategy

This is an individual classroom strategy for a fictional company. No customer experiment has run.
The scenario supplies $10M ARR, about 2% trial conversion, and 40% one-year paid retention.
The 12-month plan tests first value, useful recurrence, and a conditional packaging change before scaling a product-driven acquisition loop.

Source: Saad Binnffal · Product Analytics & Experimentation

## 2. The growth problem

FinWise has reached product-market fit. The immediate strategy priority is the trial experience and repeated value, not a claim that the company is pre-PMF.
The scenario describes paid acquisition as the main growth dependency and says that more acquisition spending is no longer producing meaningful growth.
The existing data do not establish price, onboarding, or collaboration as the root cause.

Source: Source: course scenario. These are givens, not measured project results.

## 3. Trial-to-paid has the largest relative loss

The table totals are 94,558 visits, 6,424 trials, and 128 paid conversions. Trial-to-paid is 1.9925%.
This puts the largest observed relative drop at Revenue, not a proven substep inside activation.
Acquisition has the larger absolute loss (88,134 visits do not appear as trials).
Paid and Trials may not be cohort-aligned. These ratios describe same-month table totals, not verified user-level conversion journeys.

Source: Source: 04-signals/data-signals.md and supplied monthly table.

## 4. A 12-month plan with evidence gates

Months 1-2: verify event definitions and eligible workspace recruitment. Run M5 only after checking the sample plan. The proposed M5 read date is 4 January 2027.
Months 3-5: evaluate first-value results and test the M3 weekly-review progress bar after a first own-data forecast. Follow paid cohorts and retained useful use.
Months 6-8: audit packaging and unit costs. Run M6 only if a real pre-value payment barrier exists and the experiment is feasible.
Months 9-12: investigate whether collaborators bring another business. Count qualified referred workspaces and their activation, payment, retention, and cost. Reallocate acquisition budget only after a durable commercial signal.
No revenue forecast is invented because ARPA, unit costs, CAC and linked cohorts are unavailable.

Source: Proposed sequence: November 2026 to October 2027. Timing depends on feasibility.

## 5. The Bet

The original bet is optional accountant or teammate collaboration during onboarding.
The loop requires useful shared value before repeat use, and cross-business introductions before it can create new trials.
Expansion within one workspace is not itself acquisition of a new business.
The source loop image is available in the repository. This slide restates it as editable text and connectors.
First test: does offering collaboration improve week-1 activation? Paid and retained use are downstream checks.

Source: Source: 01-bet/growth-bet.md. All loop links remain hypotheses.

## 6. The Solution

Candidate Aha: I can see when the business may run short of cash before it happens, even if its ending balance looks healthy.
The four screens are goal, data, review inputs, and forecast. Each has one primary job.
The optional invitation lives in input review. No invitation or waiting is required to continue.
The sample's ending cash is $8,400, but the low point is $7,000, below the chosen $8,000 buffer.
Production activation requires own-business data plus a first valid model within seven days. A sample-only preview does not count.
The local HTML prototype simulates invitations and does not send messages.

Source: Source: 02-solution/activation-solution.md. Screen uses fictional USD sample data.

## 7. The Mechanic

The proposed mechanic is a progress bar for one meaningful weekly cash review.
Trigger: the owner's chosen planning moment, optionally supported by a reminder.
Action: confirm or update data, review the lowest cash point and buffer, and save a decision or no-changes-needed note.
Reward: current financial clarity and a visibly completed review.
Investment: updated inputs and a dated note help the next review.
A weekly cadence is a hypothesis. No streak penalty is used, history stays available, and 100% review completion does not mean healthy finances.
Validation compares the same review function with versus without progress framing. Primary: days 8-14 meaningful review after first forecast. Check week-4 use and paid retention later.

Source: Source: 03-mechanic/engagement-mechanic.md. Static concept, not a tested retention result.

## 8. The Signals

North Star: number of trial users importing their own data and reaching first modeling output. Proposed window: seven days.
Leading 1: own-data import completion among trial starters.
Leading 2: first-model completion among importers in the same trial cohort by day 7. The reported Modeling percentage is not this conditional rate.
Lagging: cohort-aligned paid conversion and paid retention.
The selected Import-versus-conversion Pearson r is about -0.05, a descriptive result. It does not validate import usage as a payment predictor and does not prove import improvements ineffective.
The scatter's conversion axis is zoomed. Definitions, timing, and cohort alignment remain unresolved. Monthly counts are small and consistent with rounded 2% of trials.
Keep user-level North Star counts distinct from workspace assignment and business-account payment outcomes.

Source: Source: 04-signals/data-signals.md. 13 monthly aggregates. Conversion axis zoomed.

## 9. The Validation

This is an account-level invitation experiment, not a pricing test.
Assign eligible new trial workspaces 50/50 before onboarding exposure. Keep owners and collaborators in the same variant.
Control: M2 flow without inline invitation. Treatment: same flow with an optional invitation in input review.
Primary: workspace imports own data and generates a valid model within 168 hours.
Success target: observed lift at least 10 percentage points, 95% confidence interval excluding zero, and acceptable guardrail.
Guardrail: day-1 noncompletion deterioration no greater than 2 percentage points. This captures delay as well as exit.
About 400 per arm is a conservative primary-metric planning estimate for a 10-point effect, 80% power, two-sided alpha 0.05. The guardrail may require more observations.
Proposed recruitment: 2 November-27 December 2026. Complete seven-day follow-up, then read on 4 January 2027. Validate feasibility before launch. An insufficient sample remains inconclusive.
Monitor serious harm and data quality throughout. No lift has been measured.

Source: Source: 05-validation/experiment-brief.md. Targets and dates are proposed.

## 10. The Model

Prioritize Stage 1 value creation for the trial experience despite PMF and $10M ARR.
Keep base prices and billing terms. Retain the existing reverse-trial freemium approach with paid workspace subscriptions for recurring cash planning.
Candidate packaging boundary: own-data import, one editable 30-day forecast, and optional accountant review available without payment. Preserve manual weekly review. Paid capacity could cover extra forecast scenarios.
Audit entitlements, actual payment exposure, and servicing cost first. If the first-value path is already free, preserve it and prioritize M5 instead of a redundant packaging change.
M4 Leading 2 is diagnostic alongside activation in all assigned workspaces. Do not claim a day-7 effect from a change exposed only after trial expiry.
A separate later comparison measures 90-day revenue after discounts and refunds per originally assigned workspace, paid conversion, retained useful use, and costs.

Source: Source: 06-model/pricing-model.md. Packaging and willingness to pay remain unvalidated.

## 11. The Story

Growth thesis: useful first forecasts, repeat reviews, and conditional collaboration may create a path to sustained paid use.
One friction: forcing an invitation could delay first value. The proposed prototype lets owners continue without inviting or waiting. This is a design concern, not a verified production finding.
One Aha: ending cash of $8,400 can hide an earlier $7,000 low point below an $8,000 buffer.
Takeaway: I revised the assumption that import usage was a validated payment predictor after seeing monthly r near zero.
The next decision is to verify events and execute a feasible M5 test. Broader acquisition investment follows evidence of retained revenue and acceptable cost.
The README contains the full reflection and 12-month decision gates.

Source: Author reflection based on this coursework. No live customer experiment or interview is claimed.
