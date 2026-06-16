# Prompt Template: [Draft acceptance criteria from a user story]

**Date:** 2026-06-16
**Author:** [Jordan Quinn — Business Analyst]
**Project:** [Meridian Retail Group]
**Model:** [Claude Sonnet 4.6]
**DIAL location:** [DIAL shared link or folder path]
**Committed location:** [https://github.com/jordanq97/AI-Run---Meridian-Retail-Group-Katas]

---

## Purpose

[This prompt will parse the user story to generate structured acceptance criteria to ensure completeness and keep criteria testable and measurable. This prompt is for business analyst to write the formal draft criteria and is at the Requirements / Planning SDLC stage and is written alongside or immediately after the user story.]

---

## Variable Placeholders

| Placeholder | Description | Example value |
|---|---|---|
| `{{User Story}}` | [one-sentence description of a software feature written from the end-user's perspective] | [Acceptance Criteria, description] |
| `{{Target Audience}}` | [The people who the data will be presented to and targeted towards] | [Stakeholders] |
| `{{Language}}` | [The language spoken by the client] | [English] |

---

## Output Format Instruction

[Return a bulleted list and checklist format for acceptance criteria. Maximum 50 bullet points. No preamble.]

---

## Prompt Body

[## ROLE
You are a senior Business Analyst and QA Engineer with deep experience in Agile delivery. Your job is to produce clear, complete, and testable acceptance criteria from a user story.

---

## INSTRUCTIONS

1. Read the user story provided below carefully.
2. Identify the actor, the goal, and the intended benefit.
3. Flag any ambiguities or missing information before generating criteria.
4. Draft acceptance criteria in BOTH formats:
   a. Gherkin (Given / When / Then) — for BDD and automated testing
   b. Checklist — for business sign-off and UAT
5. Cover ALL of the following scenarios:
   - Happy path (expected successful outcome)
   - Edge cases (boundary or unusual but valid inputs)
   - Error / failure states (what happens when something goes wrong)
   - Security considerations (if applicable)
   - Accessibility considerations (if applicable)
   - Performance expectations (if applicable, be specific — e.g. "within 3 seconds")
6. Each criterion must be:
   - Testable (can be verified as pass or fail)
   - Unambiguous (only one interpretation possible)
   - Independent (each criterion stands on its own)
7. After the criteria, list any ASSUMPTIONS you have made.
8. Flag any open QUESTIONS the team should resolve before development starts.

---

## OUTPUT FORMAT

### Ambiguities noticed
[List anything unclear in the user story before proceeding]

### Acceptance criteria — Gherkin format
**Scenario 1: [Scenario name]**
- Given [precondition]
- When [action taken]
- Then [expected outcome]

(Repeat for each scenario)

### Acceptance criteria — Checklist format
- [ ] [Criterion 1]
- [ ] [Criterion 2]
(Continue for all criteria)

### Assumptions made
- [Assumption 1]
- [Assumption 2]

### Open questions for the team
- [Question 1]
- [Question 2]

---

## USER STORY

[PASTE YOUR USER STORY HERE — replace this line with the full user story, written in the format: "As a [role], I want to [goal], so that [benefit]."]]

---

## Test Run (Author)

**Input values used:**
- `{{stakeholder}}` = [Ryanair]
- `{{User story}}` = [As a budget traveler, I want to check in via the Ryanair app and access my digital boarding pass without paying for seat selection, So that I can avoid airport print fees and quickly board my flight]

**Output quality:** [Yes the output was usable as it contained all requirements and a full analysis as well as examples and followed the set format?]

---

## Peer Review

**Reviewer:** [Daniel Kane — Business Analyst]
**Date reviewed:** 2026-06-16
**Model used by reviewer:** [Claude]

**Reviewer input values used:**
- `{{stakeholder}}` = [Adidas]
- `{{User story}}` = [As an Adidas supply chain manager I want the website to automatically suggest alternative items when a specific size or color is out of stock so that I reduce cart abandonment and maintain customer happiness]

| Review question | Reviewer answer |
|---|---|
| Could you run the template without asking the author anything? | Yes — [I was able to run the template without asking for assistance as it contained everything I needed to draft acceptance criteria from a user story ] |
| Was the output format what you expected? | Yes — [It was what I was expecting as the format is laid out like you would expect from a detailed prompt ] |
| Would you use this template on your own work? | Yes — [If I was tasked with drafting acceptance criteria from a user story I would use this as it is detailed and easy to follow ] |
| One concrete improvement suggestion | [use a markdown table with columns X, Y, Z to make the results more structured and presentable] |

---

## Revision History

| Version | Date | Change | Author |
|---|---|---|---|
| 1.0 | 2026-06-16 | Initial commit | [Jordan Quinn] |
| 1.1 | 2026-06-16 | Post-review update | [Jordan Quinn] |