# Model Selection Note

**Date:** 2026-06-15
**Author:** [Jordan Quinn — Business Analyst]
**Project:** [Meridian Retail Group]
**Task:** [Generating alerts to engineering teams automatically detecting and flagging anomalies or failures in the unified commerce platform’s system logs.]
**Committed location:** [https://github.com/jordanq97/AI-Run---Meridian-Retail-Group-Katas]

---

## Evaluation Criteria

| # | Criterion | Why it matters for this task |
|---|-----------|------------------------------|
| 1 | [Output accuracy] | [because false positives can overwhelm engineering teams with unnecessary alerts, while false negatives may allow real outages or performance issues to go undetected, risking business continuity.] |
| 2 | [Completeness] | [missing or incomplete anomaly detection could result in undetected system failures or performance degradations, preventing timely intervention and potentially disrupting sales and customer experience.] |
| 3 | [Context window fit] | [Context window fit matters for this task because the AI model needs to analyze long sequences of log entries together to accurately detect patterns and anomalies that may span multiple events] |
---
## Prompt Used
[Generate sample alerts to engineering teams automatically detecting and flagging anomalies or failures in the unified commerce platform’s system logs for Meridian Retail Group using the attached onboarding.md doc]
---
## Output Comparison
### Model A: [DIal ChatHub GPT-4.1]
> [Representative excerpt — Here are sample alert templates for engineering teams at Meridian Retail Group, designed to automatically detect and flag anomalies or failures in the unified commerce platform’s system logs. These alerts are tailored to the platform’s architecture and operational context, as described in your onboarding documentation:]

### Model B: [Claude Sonnet 4.6]
> [Representative excerpt — Now I have a clear picture of the onboarding doc and design guidance. Let me build an AI-powered alert dashboard that generates realistic, context-aware anomaly alerts for Meridian Retail Group's commerce platform.]

---

## Scorecard                                                                                                                                | Criterion | Model A score (1–3) | Model A evidence | Model B score (1–3) | Model B evidence |
|-----------|---------------------|------------------|---------------------|------------------|
| [Output accuracy] | Model A score (2) | The model provide 6 example alerts which contain adequate bullet point description of each section of an alert e.g alert, details, impact, action and compliance notes but does not provide a visual example | Model B score (3) | The model provided live alerts dashboard which contains 5 alerts which go into detail about example alerts and provides a fully accurate representation of a live alert.  |
| [Completeness] | Model A score (2) | The model only provided alert types and a list of sections and a description it did not provide a complete alert including level of severity and visual dashboard  | Model B score (3) | The model provided a full detailed breakdown of the example alert including a severity score, runbook, page squad, root cause and SLAs  |
| [Context window fit] | Model A score (1) | The model did not provide any example context data to allow it to formulate a complete sample alert | Model B score (3) | The model provided example context data using the attached onboarding.md doc which enabled it to provide realistic, context-aware anomaly alerts  |
| **Total** | Model A score | (2) | Model B score | (3) |

---

## Decision

**Selected model:** [Claude Sonnet 4.6]

**Rationale:** [Model B won as it was able to not only provide an example alert but was also able to generate a live monitoring dashboard which included a severity level and example alert data as well as root cause, Runbook and Page squad links. The main shortcoming for this task for model A was that it only provided sample alerts from a definition level and did not provide any sample alerts using sample data or create any additional tools such as an AI-powered alert dashboard that generates realistic, context-aware anomaly alerts  ]

---

## Active Constraint

**What could change this decision within 30 days:**
[I would introduce a token budget cap to ensure the team is within budget as well as a developer tool approval to ensure that the team as satisfied with the live dashboard and that it can be used for the business.]

---

## Revision history

| Version | Date | Change |
|---------|------|--------|
| 1.0 | YYYY-MM-DD | Initial commit |