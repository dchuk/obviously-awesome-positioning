---
description: Diagnose whether your product has a positioning problem using the book's symptom checklist
argument-hint: "[product name or description]"
---

# Diagnose Positioning

**Purpose:** Run a structured diagnostic to determine whether your product has a positioning problem. Use this command when marketing or sales results feel inexplicably weak, or when you suspect that unclear messaging — not product quality — is the root cause.

## When to Use

Invoke this command when any of the following are true:

- Current customers love your product but new prospects can't figure out what you're selling
- Your sales team spends more time explaining *what you do* than closing deals
- You have long sales cycles, low close rates, or late-stage drop-offs
- Customer churn is high shortly after purchase
- New customers constantly request features you have no plan to deliver
- Prospects complain your prices are too high despite strong customer satisfaction
- There is a disconnect between how happy customers describe the product and how prospects describe it

## Steps

1. **Collect the product description.** Ask the user: "Provide a one-paragraph description of your product — what it does, who it's for, and how you currently position it. If you have website copy or a pitch deck excerpt, paste it here."

2. **Collect happy-customer language.** Ask the user: "How do your happiest, best-fit customers describe your product to others? Paste 2–4 real quotes or paraphrases if you have them."

3. **Collect prospect language.** Ask the user: "How do new prospects describe your product after a first demo or first visit to your site? Paste 2–4 real quotes or paraphrases if you have them. If you don't have these, describe what objections or confused questions prospects most commonly raise."

4. **Run the symptom checklist.** Evaluate the user's inputs against all eight symptoms from the decision rule `ch01.decision.do-you-have-positioning-problem`. Output a checklist table:

   | Symptom | Present? | Evidence from user input |
   |---------|----------|--------------------------|
   | Prospects can't quickly explain what the product does | ✅ / ❌ | … |
   | Sales team spends more time explaining than closing | ✅ / ❌ | … |
   | Long sales cycles / low close rates / competitor losses | ✅ / ❌ | … |
   | Late-stage drop-outs after serious evaluation | ✅ / ❌ | … |
   | High churn shortly after purchase | ✅ / ❌ | … |
   | New customers request features with no delivery plan | ✅ / ❌ | … |
   | Persistent price-too-high complaints | ✅ / ❌ | … |
   | Disconnect between happy-customer descriptions and prospect descriptions | ✅ / ❌ | … |

5. **Identify the description gap.** Compare the happy-customer language (Step 2) against the prospect language (Step 3). Flag the specific words, frames, or value claims that appear in one set but not the other. A significant gap is the clearest single indicator of a positioning problem.

6. **Check for the three root-cause anti-patterns.** For each symptom flagged ✅, identify whether it matches one or more of the canonical anti-patterns:
   - **Throwing Budget at Weak Positioning** — increasing spend without fixing the message; signals: ads run but close rates don't improve
   - **Letting the Market Position You by Default** — no deliberate frame of reference was ever chosen; signals: positioning was assumed at launch and never revisited
   - **Building Features for Churned/Misfit Customers** — roadmap driven by disappointed customers attracted by bad positioning; signals: churn + relentless feature requests from customers who leave anyway

7. **Render a verdict.** Using the decision rule logic:
   - **Positioning problem confirmed** if 3 or more symptoms are present, OR if a clear description gap exists between happy customers and prospects.
   - **Positioning problem likely** if 1–2 symptoms are present and the description gap is partial.
   - **No positioning problem detected** if prospects understand the product quickly, best-fit customers move through buying fast, price objections are rare, and churn is low.

8. **Recommend next steps.** Based on the verdict, output a prioritized action list:
   - If confirmed → suggest running `/identify-best-fit-customers` to anchor repositioning, then `/list-competitive-alternatives`
   - If likely → suggest running `/review-positioning-health` for a full component audit
   - If none detected → note that positioning appears healthy; suggest scheduling a periodic review

## Verify

The diagnosis is complete and coherent when:

- [ ] All eight symptom rows in the checklist table are filled with a ✅ or ❌ and a brief evidence note
- [ ] The description gap analysis names specific words or frames from user input — not generic observations
- [ ] At least one root-cause anti-pattern is named (or explicitly ruled out) with a reason
- [ ] A clear verdict (confirmed / likely / none) is stated
- [ ] At least one concrete next-step command is recommended

## Notes

- This command diagnoses *whether* a positioning problem exists. It does not fix positioning. Use the recommended next-step commands to begin the 10-step positioning process.
- If the user cannot supply prospect language (Step 3), instruct them to run the field test from the book: show the product to 3–5 people who would be genuine prospects (not friends or family), ask them to describe what they saw, and return with those descriptions before continuing.
- Deliberate vs. default positioning is a critical distinction — see [positioning foundations](../skills/obviously-awesome/references/core/positioning-foundations.md) for the two traps that arise from defaulting.
- For a full catalog of anti-patterns and their fixes, see [positioning anti-patterns](../skills/obviously-awesome/references/anti-patterns/positioning-anti-patterns.md).
- If the diagnosis reveals misfit-customer churn, the fix begins with understanding who your best-fit customers actually are — see [best-fit customers](../skills/obviously-awesome/references/core/best-fit-customers.md).
