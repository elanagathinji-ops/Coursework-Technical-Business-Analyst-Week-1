# JTBD and Prioritisation Template

## Step 1: Group the evidence

Theme labels:

-Duplicated Work & Manual Workarounds
-Delayed or Missed Follow-ups & Inefficient Triage
-Poor Account-Status Visibility & Data Inconsistency
-Customer Friction & Disjointed Contact Journeys
-Lack of Confidence in Numbers & Financial Reporting
-Change Resistance

## Step 2: Build an evidence table

Evidence ID | Stakeholder | Quote or observation | Theme | Business impact | Confidence |
|---|---|---|---|---|---|
E01 | Christopher Richards (Collections Representative)| "The collections database does not sync with the email tracker, so representatives often re-contact customers who were already promised callbacks." | Duplicated Work & Manual Workarounds | Causes customer dissatisfaction, wastes agent handling time, and risks regulatory non-compliance | High |
E02 | Daniel Okoye (Finance & Compliance Director) | "Every status update in the old system requires manual re-keying into the spreadsheet." | Duplicated Work & Manual Workarounds | Multiplies administrative overhead across 50+ staff, introduces human data-entry errors, and slows resolution speed | High |
E03 | Thomas Wright (Operations Manager) | "I spend more time reading notes from other representatives than I spend actually calling customers." | Duplicated Work & Manual Workarounds | Drastically reduces agent contact capacity and increases average handle time per account. | High |
E04 | Dr Lynda Smith (Operations Analyst) | "The spreadsheet is now two hundred sheets thick and no one knows what half of them do." | Duplicated Work & Manual Workarounds | Severe technical debt and operational fragility; high risk of formula corruption and lost account history | High |
E05 | Catherine Frost & Lawrence Bennett (Data Analyst / Collections Representative) | "We lose at least 20% of follow-ups because they fall between shifts and no one owns the handoff." | Delayed or Missed Follow-ups & Inefficient Triage | Direct revenue leakage from expired payment promises and broken callback commitments. | High |
E06 | Lawrence Bennett (Finance Analyst) | "We have cases sitting in 'awaiting callback' status for months because the promised date was never recorded." | Delayed or Missed Follow-ups & Inefficient Triage | Debt ages into uncollectable delinquent tiers, significantly increasing provision charges | High |
E07 | Priya Nair (Operations Manager) | "Simple cases that could be resolved in minutes take days because they get stuck in the wrong queue." | Delayed or Missed Follow-ups & Inefficient Triage | Sub-optimal resource allocation and artificial operational bottlenecks across simple cases. | High |
E08 | Simon Burns & Gareth Evans (Compliance Liaison / Senior Collections Team Leader) | "We do not have a way to identify which cases are straightforward versus which require specialist handling." | Delayed or Missed Follow-ups & Inefficient Triage | Straightforward cases are delayed behind specialist work, increasing cycle time and reducing collections throughput. | High
E09 | Mr Philip Stone (Service Design Lead) | "A single customer can have five separate records in the system from different entry points." | Poor Account-Status Visibility & Data Inconsistency | Distorts portfolio account counts, leads to conflicting customer contacts, and dilutes credit risk modeling | High |
E10 | Jacqueline Norris & Sarah Mitchell (Operations Analyst / Representative) | "There is no standard definition of what each status actually means across the team." | Poor Account-Status Visibility & Data Inconsistency | Renders management reporting unreliable and prevents effective case hand-offs. | High |
E11 | Veronica Cole & Christopher Richards (Compliance Officer / Representative) | "The current system treats payment promises the same as payment confirmations, which creates confusion." | Poor Account-Status Visibility & Data Inconsistency | Inaccurate cash forecasting and premature suppression of recovery actions | High |
E12 | Robert Quinn (Process Improvement Lead) | "Customers get transferred between departments and have to repeat their entire situation each time." | Customer Friction & Disjointed Contact Journeys | High customer frustration, prolonged resolution times, and increased drop-off rates. | High |
E13 | Daniel Okoye (Finance Business Partner) | "Customers call back three times because they do not remember what they were told on the first call." | Customer Friction & Disjointed Contact Journeys | Triples inbound call volumes for preventable balance/payment clarification queries | High |
E14 | Diana White (Collections Representative) | "We are exposed to complaint risk because customers cannot track what we have told them." | Customer Friction & Disjointed Contact Journeys | Escalated regulatory complaints, Ombudsman disputes, and potential financial remediation costs. | High |
E15 | Dr Lynda Smith (Operations Analyst) | "Customers would pay more readily if they understood exactly what they owe and could see options." | Customer Friction & Disjointed Contact Journeys | Unclear balances and hidden repayment options suppress voluntary payment, lengthening recovery cycles and driving avoidable inbound queries. | Medium |
E16 | Mr Philip Stone (Service Design Lead) | "The spreadsheet workaround cost us five hundred thousand pounds in lost recovery last year." | Lack of Confidence in Numbers & Financial Reporting | Direct quantifiable financial loss (£500,000) stemming from manual operational errors | High |
E17 | Christopher Richards (Collections Representative) | "Every month the finance team has to reconcile our activity count with the database, and they never match." | Lack of Confidence in Numbers & Financial Reporting | Monthly financial reconciliation friction and severe distrust in department efficiency metrics | High |
E18 | Ms Andrea Lamb (Collections Representative) | "The data quality is so poor that we stopped running management reports altogether." | Lack of Confidence in Numbers & Financial Reporting | Complete absence of data-driven decision-making in daily debt recovery operations. | High |
E19 | Daniel Farmer (Finance Analyst) | "Reporting takes so long that by the time we see the numbers, they are already out of date." | Lack of Confidence in Numbers & Financial Reporting | Lagging metrics prevent timely operational interventions on degrading account queues | High |
E20 | Thomas Wright & Tracy Field (Operations Manager / Compliance) | "Representatives are afraid to try new things because they were burned by the last system update." | Change Resistance | Risk of low staff adoption for new portal tools without change management support. | High |
E21 | Christopher Richards-Smith (Collections Representative) | "Representatives are afraid of the portal because they think it will take away their job, not because it won't work." | Change Resistance | Employee pushback and resistance if automation is positioned purely as headcount reduction. | Medium |
E22 | Eleanor Clark & Daniel Farmer (Service Design Lead / Finance) | "We have edge cases involving hardship, vulnerability, and regulatory forbearance that need human judgment." | Change Resistance | Highlight that self-service cannot be 100%; explicit human hand-off pathways are mandatory. | High |
E23 | Gareth Evans & Ms Andrea Lamb (Senior Team Leader / Representative) | "Leadership approved the roadmap five years ago and never came back to debt recovery." | Change Resistance | Deep institutional skepticism regarding leadership's long-term commitment to tooling | High

## Step 3: Write JTBD statements


## JTBD table

| JTBD ID | Actor | Statement | Evidence link | Portal relevance | Priority |
|---|---|---|---|---|---|
| JTBD-01 | Representative | When I'm about to contact a customer, I want to see a single, up-to-date record of promised callbacks across every channel, so that I don't waste calls re-contacting someone who's already been handled and risk breaching a promise made through another channel. | E01 | High — a unified promise/contact view is a core self-service and representative-workflow requirement for Phase 1. | High |
| JTBD-02 | Customer | When I'm trying to deal with my debt, I want to see exactly what I owe and what repayment options are available to me, so that I can confidently choose an arrangement I can afford and start paying without needing to call. | E15 | High — clear balance and option visibility is the core self-service value proposition of the portal and a direct driver of voluntary payment. | High |
| JTBD-03 | Finance Analyst | When I'm assessing recovery performance, I want current, near-real-time operational numbers instead of a delayed reporting cycle, so that I can intervene on degrading accounts while there's still time to act, rather than reacting to stale data. | E17 | High — timely operational data is a prerequisite for the ROI case and ongoing performance monitoring. | Medium |
| JTBD-04 | Finance & Compliance Director | When a case status changes in the collections system, I want that update to flow through to the spreadsheet/reporting record without manual re-entry, so that I can trust reconciled figures and avoid administrative overhead and data-entry error across 50+ staff. | E02 | High — automated status propagation removes a core duplicated-work pain point and underpins reliable reconciliation. | High |
| JTBD-05 | Senior Collections Team Leader | When a new case enters recovery, I want to quickly distinguish straightforward cases from those needing specialist handling, so that simple work is fast-tracked while complex or regulated scenarios are routed to the right experts without delay. | E08 | High — eligibility triage is foundational to safe self-service and prevents specialist queues from blocking recoverable low-complexity cases. | Critical |
| JTBD-06 | Customer | When my account is passed to another team or department, I want the person I speak to next to already understand my situation, so that I don't have to repeat my whole story and can reach a resolution faster. | E12 | High — a shared case context that moves with the customer underpins portal-to-representative hand-offs and reduces repeat explanations. | High |
## Step 4: Top 3 justification

For each of your top 3 JTBDs, write:
- why it matters now
- which evidence supports it
- how it should influence Phase 1

**JTBD-05** (Triage straightforward vs specialist cases) matters now because simple cases get queued behind complex ones with no priority logic, artificially extending resolution time and wasting representative capacity on routing work instead of collection work. Evidence: E08 directly states this problem; additionally E07 notes simple cases take days when they should take minutes. **Phase 1 implication:** Design an intake questionnaire or rules engine that classifies cases as self-service eligible, representative-led, or specialist-only at entry. This unblocks the rest of the portal value.

**JTBD-04** (Automated status propagation) matters now because every status update in the legacy database requires manual re-keying into the spreadsheet, multiplying overhead across 50+ staff and introducing reconciliation failures every month. Evidence: E02 identifies the root cause; E17 shows the downstream impact on reporting timeliness. **Phase 1 implication:** Build a direct integration between the new portal/system and the existing reporting layer so status changes flow automatically. This removes duplicated work and restores trust in numbers.

**JTBD-02** (Customer sees balance and options) matters now because customers don't understand what they owe or that they can pay online, causing them to call back repeatedly for the same clarification. Evidence: E13 shows customers call three times for clarification; E15 confirms that visibility drives voluntary payment. **Phase 1 implication:** The portal's first screen must show a clear, current balance and all available payment arrangements in plain language, with no hidden complexity. This is the primary reason a customer would use self-service. 



## Quality check

Ask yourself:
- Does this describe a need instead of a feature?
- Would the job still exist if the screen or tool changed?
- Can I point to real evidence behind the priority?
