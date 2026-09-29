---
description: "Turn a stakeholder quote into a Jobs-to-be-Done (JTBD) statement, separating the requested feature from the underlying job"
agent: "agent"
argument-hint: "Paste a stakeholder quote (and who said it, if known)"
---
## Jobs-to-be-Done

A discovery framework for understanding what people are trying to achieve, not just what features they ask for. Legacy Trust stakeholders describe symptoms — duplicated work, missed follow-ups, poor visibility, distrust of new tools — and this prompt turns those complaints into structured needs that can drive process design and scope decisions.

Key concepts:
- Focus on outcomes, not requested features
- Separate customer, representative, manager, and finance perspectives
- Use the pattern: "When..., I want to..., so that..."
- Prioritise jobs by business impact and evidence strength

## Task

Given a stakeholder quote (and, if known, who said it and their role), produce a JTBD statement.

1. **Identify the surface ask.** Quote or paraphrase the literal thing requested (e.g., "a dashboard," "a report," "an alert").
2. **Ask why, twice.** Infer the situation triggering the ask (the "when"), the outcome they're actually trying to achieve (the "want to"), and the deeper motivation or consequence they care about (the "so that"). Do not stop at the first restatement of the tool.
3. **Write the JTBD statement** in the pattern: "When [situation/trigger], I want to [underlying capability/outcome], so that [deeper motivation or consequence]." The middle clause must describe a capability or outcome, not a named tool or artefact.
4. **Attribute perspective.** Note which stakeholder lens this job belongs to (customer, representative, manager/operations, or finance/compliance), since the same surface complaint can hide different jobs depending on who says it.
5. **Flag evidence strength.** State whether the job is directly supported by the quote, or whether it's an inference that should be validated with the stakeholder before being treated as confirmed.
6. **Show your work briefly.** Include a one-line "surface ask → underlying job" note so the leap from feature request to JTBD is auditable, not just asserted.

## Output format

```
**Surface ask:** <what they literally asked for>
**Stakeholder / perspective:** <name/role — customer | representative | manager/operations | finance/compliance>
**JTBD statement:** When <situation>, I want to <outcome/capability>, so that <motivation/consequence>.
**Evidence strength:** Direct from quote | Inferred — validate with stakeholder
**Why:** <one line connecting the surface ask to the underlying job>
```

## Example

Input quote: "I need a dashboard so I can see what's going on with cases."

```
**Surface ask:** A dashboard.
**Stakeholder / perspective:** Manager/operations.
**JTBD statement:** When I review workload, I want reliable visibility of self-serve and representative-routed cases, so that I can manage the team accurately.
**Evidence strength:** Inferred — validate with stakeholder whether "what's going on" means case status, workload distribution, or exceptions.
**Why:** "Dashboard" is the requested tool; the underlying job is reliable visibility to support accurate team management, not the UI itself.
```

If the quote is ambiguous or could map to more than one job, produce multiple candidate JTBD statements rather than guessing a single one, and flag which stakeholder conversation would resolve the ambiguity.
