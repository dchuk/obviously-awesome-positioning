# Best-Fit Customers

Positioning has a chicken-and-egg problem. To define your market frame of reference you need to know your target customers. To identify target customers you need to know your value. To articulate value you need to know your competitive alternatives. And your competitive alternatives depend on who the target customers are. Every component depends on the others — so where do you start?

The answer is your best-fit customers: the people who already love what you built.

## The Circular Dependency Problem

When you sit down to write positioning, the tempting move is to open a spreadsheet of product features. That feels productive, but it anchors you immediately to a competitor frame *you* invented — one that may look nothing like how your best customers actually experience the market. You end up optimizing for a fight that isn't happening.

The resolution is to break the circle at a single fixed point: a short list of your happiest customers. Every other positioning component — competitive alternatives, unique attributes, value themes, market frame of reference — flows from understanding who those people are and why they love your product. _source: ch04 opening paragraphs_

## Who Counts as a Best-Fit Customer

Best-fit customers are customers who:

- Understood your product quickly
- Bought quickly
- Became raving fans
- Referred others without being asked
- Represent the perfect type of customer you want buying from you

They hold the key to understanding what your product is and what its positioning should be. _source: ch04 §'The first step in the positioning exercise'_

**The first step in the positioning exercise is to make a short list of your best customers and use it as a reference point for the rest of the exercise.**

## Why Surveying All Customers Fails

A common mistake is surveying the entire customer base — happy and less happy alike — to find positioning signals. The results are muddy with no clear pattern.

Filtering to only the ecstatic, best-fit customers before analyzing patterns in satisfaction and preference reveals consistent signals that can guide marketing and sales focus. Moderately satisfied customers dilute the signal. Only the most ecstatic fans share the consistent pattern that tells you where your product truly wins. _source: ch04 §'Looking back at the first few times I repositioned a product'_

## Customer Positioning vs. Investor Positioning

Your investor pitch tells a story about future vision and market leadership — disruption, category creation, where you'll be in five years. That story is legitimate, but it is not customer positioning.

Customer-facing positioning addresses immediate problems and present value. Customers who hear "disruption" language think you're about to replace something they've invested in. That can be confusing or terrifying rather than compelling.

**Do not use your investor pitch positioning as your customer-facing positioning.** The story in your investor pitch deck may look dramatically different from the story in your sales deck. _source: ch04 §'Shouldn't we position our product for customers the same way we position it for investors?'_

## Product Positioning vs. Company Positioning

Product positioning helps customers understand why they might buy a specific product. Company positioning is a broader umbrella that helps customers understand why they should consider multiple offerings from the same company.

### Decision rule: which do you position first?

| Situation | What to position first |
|---|---|
| Single-product company | Product and company as the same thing |
| Multi-product; most customers enter through one product | That one product first |
| Multi-product; customers mainly buy a bundle | Company first |

For a single-product company, focus energy on marketing and selling the product — not on building a separate company brand. Customers have fewer things to remember, and separate company and product brands create unnecessary cognitive overhead when there is only one offering. _source: ch04 §'Am I positioning my product, my company or both?'_

## Loose Positioning Before Pattern Emergence

Early guesses about ideal customers are frequently wrong. Before you have enough happy customers to see a clear pattern in who loves your product and why, keep positioning loose and minds open. Think of it as fishing with a wide net before you know which fish are most catchable. Broad market exposure reveals actual fit before you lock in narrow positioning.

**Hold off on tightening up positioning until you have enough happy customers to see a clear pattern in who loves your product and why.** _source: ch04 §'What if I don't have any super-happy customers yet?'_

## When to Use / When NOT to Use

**Use this guidance when:**
- You are beginning the positioning process for the first time or repositioning an existing product
- You have at least a handful of paying customers and need to know which signals to trust
- Your positioning feels generic, muddy, or like it describes too many types of buyers

**Do NOT use this guidance when:**
- You have no customers yet — at that stage you have no pattern to find; keep positioning loose and treat early sales as experiments
- You are writing an investor narrative — customer-facing positioning and investor positioning serve different audiences and should be developed separately

## Code Examples

The following rules encode the book's decision logic for best-fit customers directly:

```
# Rule: ch04.rule.make-best-customer-list
WHEN: Beginning the positioning process
DO: Make a short list of your best customers as the first step,
    and use it as a reference point for the rest of the exercise.

# Rule: ch04.decision.tighten-positioning-now
IS IT TIME to tighten positioning?
  YES if: You have enough happy customers to see a clear pattern
          in who loves your product and why.
  NO if:  You are in the early days and still learning what
          customers love and hate about your offering.
  NO if:  You cannot yet see a consistent pattern in who is
          happiest and why.

# Rule: ch04.decision.product-vs-company-positioning
WHICH do you position first?
  PRODUCT == COMPANY if: Single-product company.
  PRODUCT first      if: Most customers encounter you through
                         one product; you sell a product to
                         start a relationship and expand later.
  COMPANY first      if: You mainly sell a group of products
                         together.
```

## Anti-Patterns to Avoid

**Feature-first positioning** — Starting by laying out unique features anchors you to a competitor frame you invented, which frequently differs from how customers actually see competition. Fix: start with a list of best-fit customers and use their frame of reference. _source: ch04 §'But I want to start with my product, not my customers!'_

**Using investor positioning for customers** — Applying "disruption" or future-vision language to customer-facing materials. Customers hear it as threatening, not compelling. Fix: create separate positioning for customers focused on immediate problems and immediate value. _source: ch04 §'Shouldn't we position our product for customers the same way we position it for investors?'_

**Surveying the entire customer base** — Including moderately satisfied customers dilutes the signal. Results show no consistent pattern. Fix: filter to only ecstatic, best-fit customers before analyzing. _source: ch04 §'Looking back at the first few times I repositioned a product'_

**Premature tight positioning** — Locking in narrow positioning before having real customer data. Early guesses about ideal customers are frequently wrong. Fix: keep positioning loose and broad until patterns emerge from actual customer experience. _source: ch04 §'What if I don't have any super-happy customers yet?'_

## Related References

- [Positioning Foundations](positioning-foundations.md) — Why positioning matters and what weak vs. strong positioning looks like
- [Five (Plus One) Components](five-plus-one-components.md) — The full set of positioning components that best-fit customers anchor
- [Positioning Team and Vocabulary](positioning-team-and-vocabulary.md) — Who should be in the room when you build the best-fit customer list
- [Competitive Alternatives](../topics/competitive-alternatives.md) — Step 4: once you have your best-fit customers, map what they would use without you
- [Target Segmentation](../topics/target-segmentation.md) — Step 7: refining who cares most after patterns have emerged
- [Positioning Anti-Patterns](../anti-patterns/positioning-anti-patterns.md) — Full catalog of mistakes, including the four anti-patterns from this chapter
- [Identify Best-Fit Customers command](../../../../commands/identify-best-fit-customers.md) — Interactive command that walks you through building your best-fit customer list
