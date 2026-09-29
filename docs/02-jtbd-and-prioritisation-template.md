# JTBD and Prioritisation Template

## Step 1: Group the evidence

Theme labels:

-Duplicated Work & Manual Workarounds
-Delayed or Missed Follow-ups & Inefficient Triage
-Poor Account-Status Visibility & Data Inconsistency
-Customer Friction & Disjointed Contact Journeys
-Lack of Confidence in Numbers & Financial Reporting
-Change Resistance, Technical Debt & Governance Distrust

## Step 2: Build an evidence table

| Stakeholder | Quote or observation | Theme | Business impact | Confidence |
|---|---|---|---|---|
| Christopher Richards (Collections Representative)| "The collections database does not sync with the email tracker, so representatives often re-contact customers who were already promised callbacks." | Duplicated Work & Manual Workarounds | Causes customer dissatisfaction, wastes agent handling time, and risks regulatory non-compliance | High |
| Daniel Okoye (Finance & Compliance Director) | "Every status update in the old system requires manual re-keying into the spreadsheet." | Duplicated Work & Manual Workarounds | Multiplies administrative overhead across 50+ staff, introduces human data-entry errors, and slows resolution speed | High |
| Thomas Wright (Operations Manager) | "I spend more time reading notes from other representatives than I spend actually calling customers." | Duplicated Work & Manual Workarounds | Drastically reduces agent contact capacity and increases average handle time per account. | High |
| Dr Lynda Smith (Operations Analyst) | "The spreadsheet is now two hundred sheets thick and no one knows what half of them do." | Duplicated Work & Manual Workarounds | Severe technical debt and operational fragility; high risk of formula corruption and lost account history | High |
| Catherine Frost & Lawrence Bennett (Data Analyst / Collections Representative) | "We lose at least 20% of follow-ups because they fall between shifts and no one owns the handoff." | Delayed or Missed Follow-ups & Inefficient Triage | Direct revenue leakage from expired payment promises and broken callback commitments. | High |
| Lawrence Bennett (Finance Analyst) | "We have cases sitting in 'awaiting callback' status for months because the promised date was never recorded." | Delayed or Missed Follow-ups & Inefficient Triage | Debt ages into uncollectable delinquent tiers, significantly increasing provision charges | High |
| Priya Nair (Operations Manager) | "Simple cases that could be resolved in minutes take days because they get stuck in the wrong queue." | Delayed or Missed Follow-ups & Inefficient Triage | Sub-optimal resource allocation and artificial operational bottlenecks across simple cases. | High |
| Mr Philip Stone (Service Design Lead) | "A single customer can have five separate records in the system from different entry points." | Poor Account-Status Visibility & Data Inconsistency | Distorts portfolio account counts, leads to conflicting customer contacts, and dilutes credit risk modeling | High |
| Jacqueline Norris & Sarah Mitchell (Operations Analyst / Representative) | "There is no standard definition of what each status actually means across the team." | Poor Account-Status Visibility & Data Inconsistency | Renders management reporting unreliable and prevents effective case hand-offs. | High |
| Veronica Cole & Christopher Richards (Compliance Officer / Representative) | "The current system treats payment promises the same as payment confirmations, which creates confusion." | Poor Account-Status Visibility & Data Inconsistency | Inaccurate cash forecasting and premature suppression of recovery actions | High |
| Robert Quinn (Process Improvement Lead) | "Customers get transferred between departments and have to repeat their entire situation each time." | Customer Friction & Disjointed Contact Journeys | High customer frustration, prolonged resolution times, and increased drop-off rates. | High |
| Daniel Okoye (Finance Business Partner) | "Customers call back three times because they do not remember what they were told on the first call." | Customer Friction & Disjointed Contact Journeys | Triples inbound call volumes for preventable balance/payment clarification queries | High |
| Diana White (Collections Representative) | "We are exposed to complaint risk because customers cannot track what we have told them." | Customer Friction & Disjointed Contact Journeys | Escalated regulatory complaints, Ombudsman disputes, and potential financial remediation costs. | High |
| Mr Philip Stone (Service Design Lead) | "The spreadsheet workaround cost us five hundred thousand pounds in lost recovery last year." | Lack of Confidence in Numbers & Financial Reporting | Direct quantifiable financial loss (£500,000) stemming from manual operational errors | High |
| Christopher Richards (Collections Representative) | "Every month the finance team has to reconcile our activity count with the database, and they never match." | Lack of Confidence in Numbers & Financial Reporting | Monthly financial reconciliation friction and severe distrust in department efficiency metrics | High |
| Ms Andrea Lamb (Collections Representative) | "The data quality is so poor that we stopped running management reports altogether." | Lack of Confidence in Numbers & Financial Reporting | Complete absence of data-driven decision-making in daily debt recovery operations. | High |
| Daniel Farmer (Finance Analyst) | "Reporting takes so long that by the time we see the numbers, they are already out of date." | Lack of Confidence in Numbers & Financial Reporting | Lagging metrics prevent timely operational interventions on degrading account queues | High |


## Step 3: Write JTBD statements

Use the structure:

**When** ...  
**I want to** ...  
**So that** ...

Minimum coverage:
- customer
- representative
- operations manager
- finance partner

## JTBD table

| JTBD ID | Actor | Statement | Evidence link | Portal relevance | Priority |
|---|---|---|---|---|---|
| JTBD-01 | Representative | When I'm about to contact a customer, I want to see a single, up-to-date record of promised callbacks across every channel, so that I don't waste calls re-contacting someone who's already been handled and risk breaching a promise made through another channel. | Christopher Richards (Collections Representative): "The collections database does not sync with the email tracker, so representatives often re-contact customers who were already promised callbacks." | High — a unified promise/contact view is a core self-service and representative-workflow requirement for Phase 1. | TODO |
| JTBD-02 | Operations Manager | When I pick up a case worked by another representative, I want to quickly understand its current status and history without reading through unstructured notes, so that I can spend my time actually contacting customers instead of reconstructing context. | Thomas Wright (Operations Manager): "I spend more time reading notes from other representatives than I spend actually calling customers." | High — structured, at-a-glance case history is a prerequisite for reliable hand-offs and representative capacity gains. | TODO |
| JTBD-03 | Customer | When I've been given information or a decision on my account, I want a reliable way to recall or confirm what I was told, so that I don't have to call back repeatedly to get the same answer. | Daniel Okoye (Finance Business Partner): "Customers call back three times because they do not remember what they were told on the first call." | High — a self-service record of prior contact outcomes directly reduces repeat-call volume the portal is meant to prevent. | TODO |
| JTBD-04 | Finance Analyst | When I'm assessing recovery performance, I want current, near-real-time operational numbers instead of a delayed reporting cycle, so that I can intervene on degrading accounts while there's still time to act, rather than reacting to stale data. | Daniel Farmer (Finance Analyst): "Reporting takes so long that by the time we see the numbers, they are already out of date." | High — timely operational data is a prerequisite for the ROI case and ongoing performance monitoring. | TODO |
| JTBD-05 | Finance & Compliance Director | When a case status changes in the collections system, I want that update to flow through to the spreadsheet/reporting record without manual re-entry, so that I can trust reconciled figures and avoid administrative overhead and data-entry error across 50+ staff. | Daniel Okoye (Finance & Compliance Director): "Every status update in the old system requires manual re-keying into the spreadsheet." | High — automated status propagation removes a core duplicated-work pain point and underpins reliable reconciliation. | TODO |
| JTBD-06 | Compliance Officer | When I check an account's payment state, I want promised payments and confirmed payments to be visibly and structurally distinct, so that I can forecast cash and decide on next recovery action based on what has actually happened, not what was merely said. | Veronica Cole & Christopher Richards (Compliance Officer / Representative): "The current system treats payment promises the same as payment confirmations, which creates confusion." | High — distinguishing promise from confirmation is a compliance and cash-forecasting requirement, and likely an eligibility rule for self-service. | TODO |

## Step 4: Top 3 justification

For each of your top 3 JTBDs, write:
- why it matters now
- which evidence supports it
- how it should influence Phase 1


## Quality check

Ask yourself:
- Does this describe a need instead of a feature?
- Would the job still exist if the screen or tool changed?
- Can I point to real evidence behind the priority?
