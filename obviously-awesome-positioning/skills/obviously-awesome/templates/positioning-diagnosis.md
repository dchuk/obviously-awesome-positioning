---
type: positioning-diagnosis
step: "diagnostic"
backs_command: /obviously-awesome-positioning:diagnose-positioning
status: blank
updated: 2026-06-05
---

# Positioning Diagnosis — Diagnostic

> **Purpose:** Capture the symptom checklist, the customer-vs-prospect description gap, and a verdict — the entry point that decides whether to begin the positioning process and which command to run next.
> **Driving question:** "Do you have a positioning problem?"

## Symptom checklist

Mark each symptom Present only with concrete evidence from the product description, happy-customer language, and prospect language collected upfront.

| Symptom | Present? | Evidence from user input |
|---------|----------|--------------------------|
| Prospects can't quickly explain what the product does | … | … |
| Sales team spends more time explaining than closing | … | … |
| Long sales cycles / low close rates / competitor losses | … | … |
| Late-stage drop-outs after serious evaluation | … | … |
| High churn shortly after purchase | … | … |
| New customers request features with no delivery plan | … | … |
| Persistent price-too-high complaints | … | … |
| Disconnect between happy-customer descriptions and prospect descriptions | … | … |

## Description gap: customers vs. prospects

How happy, best-fit CUSTOMERS describe the product vs. how new PROSPECTS describe it. Name the specific words, frames, or value claims that appear in one column but not the other.

| How happy customers describe it | How prospects describe it | Words / frames present in one, missing in the other |
|---------------------------------|---------------------------|-----------------------------------------------------|
| <customer quote or paraphrase> | <prospect quote, objection, or confused question> | <specific word, frame, or value claim that differs> |
| … | … | … |

**Gap summary:** <one line naming the clearest divergence between the two columns>

## Root-cause anti-pattern(s)

For each symptom marked Present, name the anti-pattern(s) it matches, or explicitly rule them out with a reason.

- **Throwing Budget at Weak Positioning:** <present / ruled out — reason>
- **Letting the Market Position You by Default:** <present / ruled out — reason>
- **Building Features for Churned/Misfit Customers:** <present / ruled out — reason>

## Verdict

**Verdict:** <confirmed | likely | no problem> — <one line citing the symptom count and the customer-vs-prospect gap that drove it>

## Next-step commands

Prioritized commands to run next, driven by the verdict.

1. <command> — <why this is the first step given the verdict>
2. <command> — <why this follows>

## Fill rules

- Evidence is REQUIRED for every symptom marked Present — a Present mark with an empty evidence cell is invalid. Cite specific words or facts from the user's input, not generic observations.
- Mark all eight symptom rows; leave none blank (Present or not-present, each with a note).
- The description gap must name specific words or frames from the two columns — not a generic "they describe it differently."
- The Verdict is driven by the customer-vs-prospect gap and the symptom count, NOT by internal opinion or product quality: confirmed if 3+ symptoms present OR a clear description gap exists; likely if 1–2 symptoms and a partial gap; no problem if prospects understand the product fast, best-fit customers buy quickly, price objections are rare, and churn is low.
- Name at least one root-cause anti-pattern as present or explicitly rule the three out with reasons.
- Recommend at least one concrete next-step command.
- Keep this sheet comparable across re-diagnoses over time: keep the same symptom rows and columns, and date each run via the frontmatter `updated` field so gaps can be tracked against prior diagnoses.

---
**Backs:** `/obviously-awesome-positioning:diagnose-positioning`
**Reference:** [positioning foundations](../references/core/positioning-foundations.md), [positioning anti-patterns](../references/anti-patterns/positioning-anti-patterns.md), [best-fit customers](../references/core/best-fit-customers.md)
