# Smart-Recovery Discovery Brief

## 1. Problem summary

Legacy Trust manages 100,000+ delinquent accounts through a 20-year-old collections database, spreadsheets, and email, with 50+ representatives relying on manual reconciliation and memory. The case study reports missed follow-ups, duplicate activity, inconsistent statuses, and slow, repetitive customer journeys; it does not yet quantify their frequency or establish how much each contributes to the stated ~15% revenue loss. These workarounds reduce manager visibility and consume representative capacity, while simple and complex cases share the same manual flow. Discovery should validate where work fails, identify rules-driven journeys suitable for self-service, define human escalation boundaries, and test whether a Phase 1 portal can achieve 12-month payback using sourced baselines and transparent assumptions.



## 2. Stakeholder overview

Customers are an external user group inferred from the case study; their needs and proposed measures require validation.

| Stakeholder group | What they care about | How success is measured | Main worry | Evidence they will trust |
|---|---|---|---|---|
| Operations leadership | Locate missed follow-ups, duplicate effort, and wasted handling time | Baseline those failure rates and quantify time saved by eligible automation | Simple and complex cases may be automated as if they were alike | Representative time samples, case audits, and realistic process maps |

| Team leaders and representatives | An accurate As-Is process and workable hand-offs | Consistent status updates; exceptions reach representatives with the right context | Difficult cases and messy hand-offs remain with the team without being visible | Walkthroughs of real cases, exception data, and a To-Be map with clear human ownership |

| Finance and Compliance | Measurable savings, recovery impact, compliance, and cost | A transparent 12-month value case separating hard savings from uncertain uplift | Unsupported revenue assumptions or compliance risks | Sourced baselines, explicit assumptions, sensitivity analysis, and compliance review |

| Product and delivery | Discovery outputs that can guide backlog and prototyping | Priority needs link to opportunities, workflow steps, and buildable requirements | Ambiguous scope, dependencies, or acceptance criteria | Stakeholder-validated JTBD, workflow diagrams, and a traceability matrix |

| Customers (external) | Clear next steps and less repetitive contact | Validate completion of eligible self-service journeys and repeat-contact rates | Incorrect information or unsuitable options for cases needing human help | Customer research, usability tests, and contact-journey data; needs are not yet validated |

Priya says: If the two-week window gets tight, protect analysis task 4 and discovery questions 7 and 10 first as these feed the ROI case and the eligibility rules that Daniel Okoye and Amina will use for the Phase 1 go/no-go.

## 3.1 Discovery Analysis Tasks
1. What share of activity records have duplicate_check_flag = Y (2,020 of 9,890 in a first pass), by activity_type and account_id? 
2. Using account_id, activity_date, and activity_type, how often does an account receive more than one outbound activity on the same day or within a week? 
3. What share of activity records have no next_follow_up_date (1,465 of 9,890), and what is the typical scheduled gap when one exists? 
4. What are the average and total logged minutes_spent per account and per activity type, and which activity types make up the highest volume, cross-referenced against delinquent_accounts_export.csv (3,246 accounts; product_type, delinquency_stage, days_past_due) to see which account segments carry that volume? 

## 3.2 Discovery questions

Answerable from finance_assumptions.csv, confirmed with Finance:

5. Can Finance confirm the definition and calculation behind FA-06 (14% missed-follow-up rate) so it can be checked against the next_follow_up_date rate calculated from recovery_activity_tracker.csv?

6. Can Finance confirm FA-01 (hourly cost), FA-02 (working days/month), and FA-03 (straightforward-case share) so a capacity estimate can be built from tracker minutes, and is the FA-04/FA-05 18-to-10-minute target realistic?

7. What is the source and definition of the ~15% revenue-loss estimate, and may FA-09 (monthly recovery baseline) and FA-07/FA-08 (recovery uplift) be used only as labeled low-confidence scenarios?

8. What do FA-10/FA-11 cover for Phase 1 implementation cost, and what run costs are missing from the assumptions file?

Answerable only through stakeholder conversation:

9. At each self-service escalation, what triggers the hand-off, who owns the next action, and what account context must transfer to the representative?

10. Which two or three case types look eligible for self-service given tracker volume and delinquent_accounts_export.csv segment data (product_type, delinquency_stage, days_past_due, total_balance), and what eligibility or exclusion rules make them stable enough to automate? The file's own self_service_candidate flag is inconsistently coded (Y/N/Yes/No) and should not be treated as a ready-made answer without validation. 

11. What controls or referral rules apply to disputed, vulnerable, restricted-contact, or otherwise complex accounts, and who must approve them? 



## 4. Traceability starter

This first-pass chain distinguishes reported concerns from measures that still need validation.

| Concern and source | Process area | Opportunity / JTBD to validate | Measure and evidence source | Linked deliverable |
|---|---|---|---|
| Representatives report repeated checks across spreadsheets and email (case study; quantify in discovery) | Contact-history checks, status updates, and task allocation | Help representatives see reliable contact history and next actions | Time sampled on reconciliation; duplicate-check rate; case and system audit | As-Is map, JTBD, and ranked automation opportunity |
| Follow-ups and promises to pay are difficult to track consistently (case study; baseline not supplied) | Promise tracking and follow-up scheduling | Identify eligible reminders or task prompts without automating judgement-heavy cases | Missed-follow-up and promise tracking rates; promise records and case audit | As-Is pain points, To-Be workflow, and baseline metrics |
| Human ownership at exceptions must remain clear (Gareth's stakeholder concern) | Eligibility, triage, and representative hand-off | Route exceptions with context and explicit ownership | Escalation and repeat-contact rates; walkthroughs of representative cases | To-Be workflow and linked candidate requirements |
|The 15% revenue-loss estimate needs substantiation (Daniel's concern) | Recovery outcomes and operating costs | Test operational savings separately from possible recovery uplift | Definition and source of 15% estimate; cost, volume, and recovery baselines | ROI model with assumptions, sensitivity analysis, and evidence status |

## 5. Final problem statement

Legacy Trust manages more than 100,000 delinquent accounts through spreadsheets, email, and a 20-year-old collections database, contributing to reported duplicate work, missed follow-ups, inconsistent statuses, and slow customer journeys. The frequency, cost, and contribution of these problems to the stated estimated 15% revenue loss have not yet been established. The discovery decision is whether a defined Phase 1 self-service scope, with clear eligibility and representative hand-offs, can reduce evidenced operational friction and achieve 12-month payback without weakening compliance or service for complex cases.
