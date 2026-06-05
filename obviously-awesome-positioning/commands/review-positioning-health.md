---
description: Conduct a periodic positioning review and decide whether to reposition or hold
argument-hint: "[product name or positioning doc path]"
---

# Review Positioning Health

**Purpose:** Conduct a structured positioning review triggered by elapsed time or a market event. Use this command to determine whether your current positioning still holds or whether you need to restart at Step 4 (competitive alternatives) and work forward.

**When to use:**
- Six months have passed since your last positioning review
- A credible, established competitor has entered the market
- A competitor has been acquired and gained significant new resources or reach
- Government regulations have shifted customer priorities
- A significant economic climate change has occurred
- New technology has changed what is possible in the market
- Customer attitudes or buying patterns have noticeably shifted

---

## Steps

1. **Identify the review trigger.** Ask the user what prompted this review. Classify it as one of:
   - Scheduled (six-month cadence)
   - Competitive event (new entrant, acquisition)
   - Regulatory / economic / technology shift
   - Customer signal (sales team notices declining pitch resonance, perception has shifted)

2. **Locate current positioning artifacts.** Use Glob to search for files matching `*positioning*`, `*messaging*`, `*pitch*`, or `*sales-story*` in the repository. Use Read to load any files found. If no files exist, ask the user to paste or describe their current positioning in plain text covering: competitive alternatives, unique attributes, value themes, best-fit customers, and market frame of reference.

3. **Assess the competitive landscape change.** For each relevant trigger event identified in Step 1, ask:
   - Has a new competitor entered the market? If yes — do your best-fit customers expect that competitor to be relevant to them?
   - Has an acquisition given an existing competitor significant new resources or reach?
   - Have regulations, economic conditions, or new technology materially changed what customers can buy or expect?
   - Capture the answers in a short structured list.

4. **Evaluate customer perception shifts.** Ask the user to report any available evidence of customer perception changes:
   - Recent win/loss interview themes
   - Sales team observations about pitch resonance
   - Support or success team observations about why customers stay or churn
   - Any NPS or survey data referencing competitive alternatives or value
   - If no data exists, flag this as a gap and recommend customer interviews before deciding to reposition.

5. **Apply the reposition-or-hold decision rules.** For each competitive or market event identified, evaluate:

   **Reposition (return to Step 4) if any of the following are true:**
   - Best-fit customers expect the new competitor or event to be relevant to them
   - The event signals a change in customer expectations about price, features, or market norms
   - The competitive alternatives list in customers' minds has materially shifted

   **Hold current positioning if all of the following are true:**
   - Best-fit customers do not expect the new competitor or event to be relevant to them
   - The company's strategy targets a subsegment the new entrant is unlikely to serve better than the current leader
   - Customers do not expect market norms (price, features) to change as a result of the event

   Output a verdict — **Reposition** or **Hold** — with one sentence of rationale for each event evaluated.

6. **If verdict is Reposition — restart at Step 4.** Instruct the user to:
   - Return to Step 4: list competitive alternatives from the customer's perspective using the updated landscape (see [competitive-alternatives](../skills/obviously-awesome/references/topics/competitive-alternatives.md))
   - Work forward through Step 5 (unique attributes), Step 6 (value themes), Step 7 (best-fit customers), Step 8 (market frame of reference), and optionally Step 9 (trend layering)
   - Run the `list-competitive-alternatives.md` command to begin that process

7. **If verdict is Hold — check for messaging drift.** Even when positioning holds, drift accumulates. Use Grep to search for inconsistencies across sales decks, web copy, or README files. Look for:
   - Different descriptions of the market frame of reference across documents
   - Inconsistent value theme language
   - Missing or stale master messaging document
   - Flag any **Messaging Without a Master Document** anti-pattern signals: different pages describe the product in noticeably different ways, or no single source of truth exists for approved product messaging.

8. **Update implementation artifacts.** Based on the verdict:
   - If repositioning: after completing Steps 4–9, update the sales story, master messaging document, roadmap priorities, and pricing alignment
   - If holding: correct any messaging drift found in Step 7 and refresh the master messaging document to reflect current language
   - Schedule the next review: set a concrete date six months out, or flag that the next major competitive/regulatory/economic/technology event should re-trigger this command immediately
   - Offer the user the blank template at `../skills/obviously-awesome/templates/positioning-review-log.md` — append this review's trigger, perception check, and reposition-or-hold verdict as a new dated row, or hand it over for the user to maintain as an append-only log over time.

---

## Verify

The review is complete when you can answer **yes** to all of the following:

- [ ] Every trigger event has been classified and evaluated against the reposition-or-hold decision rules
- [ ] A clear **Reposition** or **Hold** verdict has been produced with rationale
- [ ] If repositioning: the user has been directed to restart at Step 4 with an updated competitive alternatives list
- [ ] If holding: messaging drift has been checked and a master messaging document exists or is flagged for creation
- [ ] A next review date or trigger condition has been recorded

---

## Notes

**Anti-patterns to watch for:**

- **Set-and-Forget Positioning** — treating positioning as a one-time exercise and never revisiting it even as competitors enter, regulations change, technology shifts, or customer attitudes evolve. *Why harmful:* your positioning silently drifts out of alignment with the market, and the sales team's pitch loses resonance before anyone diagnoses the cause. Fix: schedule reviews every six months and after any major market event.

- **Messaging Without a Master Document** — building campaigns and materials without a single canonical messaging document, causing each new piece to build on slightly modified previous messages. *Why harmful:* positioning drift accumulates invisibly across channels — different sales decks and web pages describe the product in noticeably different ways, and new hires can't find agreed-upon language. Fix: create and maintain a master messaging document as the accepted baseline.

See [positioning anti-patterns](../skills/obviously-awesome/references/anti-patterns/positioning-anti-patterns.md) for the full catalog.

For guidance on the three market positioning styles (Head to Head, Big Fish Small Pond, and Create a New Game) and when a repositioning event might call for switching styles, see [market-positioning-styles](../skills/obviously-awesome/references/patterns/market-positioning-styles.md).

To begin a full repositioning after a **Reposition** verdict, run [`list-competitive-alternatives.md`](list-competitive-alternatives.md) first, then proceed in step order.

---

## Related files

- [positioning anti-patterns](../skills/obviously-awesome/references/anti-patterns/positioning-anti-patterns.md)
- [market-positioning-styles](../skills/obviously-awesome/references/patterns/market-positioning-styles.md)
- [competitive-alternatives](../skills/obviously-awesome/references/topics/competitive-alternatives.md)
- [Positioning Review Log template](../skills/obviously-awesome/templates/positioning-review-log.md) — fillable blank for this command's output
