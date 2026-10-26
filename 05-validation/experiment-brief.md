[experiment-brief.md](https://github.com/user-attachments/files/33981012/experiment-brief.md)
# The Validation · FinWise

> Module 5 · Proposed experiment brief. Classroom design only: no live experiment, result, or lift is claimed. Builds on the optional collaboration bet in M1, the four-screen onboarding prototype in M2, and the unresolved activation-to-payment link in M4.

## Method

**Experiment name:** Optional Accountant Review — Week-1 Activation Test.

**Method:** Standard randomized A/B test, with persistent 50/50 assignment at the trial-workspace level before onboarding exposure.

**Justification:** This is one optional interface intervention with an observable seven-day outcome. Parallel randomized groups give a direct comparison. Workspace assignment keeps an owner and their accountant in the same variant. A bandit would add adaptive-allocation complexity; geographic and switchback designs do not match this account-level intervention. A longer holdout could later assess sustained effects. This experiment does not establish annual retention or the full collaboration growth loop.

**Target segment:** Newly created small-business trial workspaces beginning onboarding during the recruitment window, before their first valid model. Exclude test/staff accounts and prior experiment participants using rules defined before assignment. Include all eligible assigned workspaces in the primary analysis, including those that never reach the review screen or use an invitation.

**Control / current comparison experience:** The M2 four-screen flow — goal, data, input review, forecast — with the inline accountant invitation prompt omitted from input review. This defines the experimental control; the course does not document FinWise's actual production onboarding.

**Single change being tested:** In the treatment only, show an optional “Invite an accountant or teammate to review” action within the same input-review screen, before the first forecast. Independent continuation remains equally clear; no invitation, acceptance, or waiting is required. Keep the rest of the flow identical.

**Execution prerequisites:** Implement and verify the production invitation, permissions, event tracking, and assignment first; the M2 prototype only simulates invitations. Check eligibility volume and cross-workspace exposure before launch.

## Hypothesis + primary metric

**Objective:** Help more trial workspaces reach a useful first financial output within their first week, before evaluating downstream payment effects.

**Hypothesis:** IF new trial workspaces see an optional accountant-review invitation during input review, THEN week-1 activation will increase by at least 10 percentage points versus control, BECAUSE relevant help may allow owners to validate inputs and create a useful first model. Collaboration is a mechanism to test, not an established root cause.

**Primary metric:** Week-1 activation rate = eligible assigned trial workspaces that successfully import their own business data AND generate at least one valid financial model within 168 hours of assignment / all eligible assigned trial workspaces. Count each workspace once. Exclude sample-only previews from the numerator. Define valid-output and own-data events before launch.

**Success threshold:** An observed treatment-minus-control activation lift of at least +10 percentage points, with a two-sided 95% confidence interval excluding zero, acceptable data quality, and the guardrail criterion below met. Report the interval: an observed +10-point lift does not prove the true lift is at least +10 points. This is a proposed practical target, not an observed baseline or effect.

**Sample-size planning:** Target at least 800 eligible workspaces in total, approximately 400 per arm. A conservative normal approximation for a binary outcome, two-sided alpha 0.05, 80% power, and a 0.10 absolute effect gives approximately 393 per arm using the maximum Bernoulli variance. This is an initial primary-metric planning estimate. Recheck power, baseline rates, eligibility volume, and guardrail precision before execution; guardrails may require more data. The source table does not provide the operational activation baseline or workspace recruitment rate.

**Analysis:** Compare assigned groups, not voluntary inviters versus non-inviters. Report absolute percentage-point lift, relative lift, group counts, and a pre-specified two-proportion confidence interval/test. Check assignment ratios, missing events, and equal observation windows. Import completion, model completion, invitation use, and acceptance are diagnostic measures, not replacement success metrics selected after seeing results.

**Predicted outcome:** Treatment improves first-week activation because optional help reduces input uncertainty. This is an expectation to test, with no guaranteed effect on paid conversion.

**If successful:** Stage the rollout, monitor the same guardrail, and follow cohort-aligned trial-to-paid conversion and retained useful use. Preserve a suitable comparison if measuring long-term impact.

**If unsuccessful or inconclusive:** Distinguish inadequate precision from evidence against a practically useful effect. Examine the assigned-group funnel and usability evidence, then revise or retire the prompt. Do not keep extending the test until significance appears. If the guardrail deteriorates, investigate before rollout.

## Guardrail + read date

**Guardrail metric:** Day-1 onboarding abandonment, operationalized consistently with M2 as the percentage of assigned workspaces that begin onboarding but have not completed the core own-data-to-first-model path within 24 hours. It includes delay as well as exit; it is not proof of permanent abandonment.

**Guardrail threshold:** No more than +2 percentage points of treatment-minus-control deterioration. Report its 95% confidence interval. Treat a clear breach as a reason to stop or investigate; if the interval still permits deterioration beyond the margin, do not declare a clean win. Additional precision or a revised test may be needed.

**Proposed classroom schedule — Asia/Riyadh:** Launch 2 November 2026; recruit through 27 December 2026 inclusive (56 days); allow the final enrolled workspace its full seven-day follow-up. Read results on **4 January 2027**. These are proposed planning dates, not a real launch or completed test.

**Read-date rule:** Keep the pre-specified recruitment window and analysis date; record an inconclusive result if volume or precision is insufficient. If the pre-launch feasibility check fails, redesign and document the schedule before launch rather than promise an arbitrary two-week answer. Monitor data quality, operational failures, and serious guardrail harm during the test; follow pre-specified safety stopping rules.

**Connection to M4:** Monthly import usage was not a validated predictor of payment. This experiment therefore measures the joint own-data-to-first-model outcome and treats payment and retention as downstream checks. It does not assume that increasing import usage alone will fix conversion.
