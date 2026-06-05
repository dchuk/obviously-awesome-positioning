---
type: positioning-review-log
step: "ongoing"
backs_command: /obviously-awesome-positioning:review-positioning-health
status: blank
updated: 2026-06-05
---

# Positioning Review Log — Ongoing Log

> **Purpose:** An append-only record of every positioning review and market trigger, with the reposition-or-hold verdict for each — builds on the current positioning artifacts and feeds the decision to restart at Step 4.
> **Driving question:** "Has the market shifted enough that customers now judge us against a different set of alternatives?"

## Review log

Append one row each time a review is triggered. Do NOT overwrite or delete prior rows — this log is longitudinal. `Event` is one of the recognized triggers (scheduled 6-month review, competitor entered, competitor exited, you were acquired or acquired someone, new regulation, economic shift, new enabling technology, customer-attitude shift).

| Date | Event | Customer-perception check done? | Reposition? (No / Partial / Yes / TBD) |
|------|-------|---------------------------------|----------------------------------------|
| <YYYY-MM-DD> | <one trigger from the list above> | <Yes / No — evidence source or gap> | <No / Partial / Yes / TBD> |
| … | … | … | … |

**Next review date:** <YYYY-MM-DD — scheduled 6 months out, or "on next major competitive/regulatory/economic/technology event">

## Fill rules

- This file is LONGITUDINAL: it is appended over time, never regenerated. Add a new dated row per review; keep all prior rows intact.
- `Event` must be one of the recognized triggers: scheduled 6-month review, competitor entered, competitor exited, you were acquired or acquired someone, new regulation, economic shift, new enabling technology, customer-attitude shift.
- The reposition decision is driven by customer PERCEPTION, not internal opinion: mark `Reposition? = Yes` only when best-fit customers expect the event/competitor to be relevant to them or the alternatives in their minds have materially shifted.
- If no customer-perception evidence exists yet, set `Customer-perception check done? = No`, flag the gap, and set `Reposition? = TBD` until interviews or data are gathered — do not guess.
- A real landscape change (a `Yes` verdict) means restart the process at Step 4 (competitive alternatives) and work forward; record that restart as the outcome of the row.
- Always update the **Next review date** line: a concrete date six months out, or the trigger condition that should re-fire this command sooner.

---
**Backs:** `/obviously-awesome-positioning:review-positioning-health`
**Reference:** [competitive alternatives](../references/topics/competitive-alternatives.md), [positioning anti-patterns](../references/anti-patterns/positioning-anti-patterns.md), [market positioning styles](../references/patterns/market-positioning-styles.md)
