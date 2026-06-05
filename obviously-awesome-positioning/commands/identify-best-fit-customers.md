---
description: Identify best-fit customers to anchor all subsequent positioning work
argument-hint: "[product name or context]"
---

# Identify Best-Fit Customers

**Purpose.** This command walks you through Step 1 of the positioning process: isolating the customers who love your product most, finding patterns in why they love it, and compiling a short best-fit customer list that anchors every downstream positioning decision.

**When to use:**
- You are starting the positioning exercise for the first time
- You are repositioning an existing product and need to re-anchor to real customer evidence
- You have been defaulting to investor-pitch framing in customer-facing materials
- You are unsure whether it is the right time to tighten up your positioning at all

---

## Steps

1. **Check readiness to proceed.** Ask the user: "Do you have enough happy customers to see a consistent pattern in who loves the product and why?" Apply the decision rule:
   - **Yes →** Continue to Step 2.
   - **No (early-stage, limited data) →** Advise the user to hold off on tightening positioning until that pattern is visible. Quote the rule: *"Hold off on tightening up positioning until you have enough happy customers to see a clear pattern in who loves your product and why."* Stop here and suggest revisiting once more customer data exists.

2. **Clarify scope: product vs. company positioning.** Ask the user how many products their company sells and how customers typically first encounter them. Apply the decision rule:
   - **Single-product company →** Position product and company as the same thing; no separate company brand exercise needed now.
   - **Multi-product company, product-led entry →** Position the primary entry product first before tackling company-level positioning.
   - **Multi-product company, bundle-led entry →** Position the company first; individual product positioning comes later.
   Record the scope decision before proceeding.

3. **Confirm investor vs. customer story separation.** Ask the user: "Are you working from an investor pitch deck or a company-level narrative?" If yes, flag it explicitly: the investor positioning story may look dramatically different from the customer-facing story. Set aside any investor framing for this exercise.

4. **Review the full customer base.** Ask the user to think through (or retrieve from CRM / sales records) their complete customer list. Prompt: *"Which customers understood the product quickly and bought quickly — with little hand-holding or objection-handling?"* Have the user name or describe those accounts.

5. **Filter for raving fans.** From the fast-to-close group, ask: *"Which of these customers became raving fans — referred other companies, acted as a reference, championed the product internally, or renewed and expanded without prompting?"* Narrow the list to those accounts.

6. **Apply the 'perfect customer' filter.** Ask: *"Of the raving fans, which represent the type of customer you most want buying from you in the short term — in terms of company profile, use case, and the problems they needed solved?"* This is the best-fit customer sub-set.

7. **Compile the best-fit customer list.** Produce a structured output: a short numbered list of best-fit customers (anonymized if needed) with one sentence per entry noting:
   - Why they bought quickly
   - What they love most about the product
   - Why they represent the ideal customer type

   Format:
   ```
   1. [Customer name / profile] — bought quickly because [X]; loves [Y]; ideal because [Z]
   2. ...
   ```

   Offer the user the blank template at `../skills/obviously-awesome/templates/best-fit-customers.md` — populate it directly with the generated anchor table and scope decision, or hand it over for the user to fill in.

8. **Save the list as a positioning anchor.** Instruct the user to keep this list visible throughout Steps 2–10. Every subsequent decision — competitive alternatives, unique attributes, value themes, market frame of reference — should be evaluated through the lens of *"does this resonate with these best-fit customers?"*

---

## Verify

The step succeeds when:
- [ ] You have confirmed it is the right time to tighten positioning (pattern is visible in the customer base)
- [ ] Scope is decided: product positioning, company positioning, or both
- [ ] Investor narrative has been explicitly set aside
- [ ] A short list (ideally 3–10 customers) exists with clear notes on why each is a best-fit
- [ ] The list reflects customers who bought quickly, became raving fans, and represent the type you want more of

If the list contains customers who were slow to close, required heavy discounting, or whose use case feels like an edge case — remove them. They will distort the pattern.

---

## Notes

- **Anti-pattern to avoid:** Do not start from product features or company-level branding and work backward to customers. The workflow runs in one direction: customers first, then everything else.
- **Anti-pattern to avoid:** Do not conflate investor positioning with customer positioning. Your investor deck may frame the market opportunity in terms that mean nothing to a buyer evaluating alternatives.
- For the full treatment of how best-fit customers interact with the rest of the positioning components, see [best-fit customers](../skills/obviously-awesome/references/core/best-fit-customers.md).
- For an overview of all five positioning components that this list will anchor, see [five-plus-one components](../skills/obviously-awesome/references/core/five-plus-one-components.md).
- [Best-Fit Customers template](../skills/obviously-awesome/templates/best-fit-customers.md) — fillable blank for this command's output
- Once this list is compiled, proceed to [`list-competitive-alternatives.md`](list-competitive-alternatives.md) (Step 4) or run the full sequence via [`agents/positioning-planner.md`](../skills/obviously-awesome/../../../agents/positioning-planner.md).
