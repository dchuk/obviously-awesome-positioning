---
name: obviously-awesome-positioning
description: "Helps founders, marketers, and executives deliberately position products using April Dunford's 10-step methodology from Obviously Awesome. Use when diagnosing weak positioning, repositioning a product, building a sales story, selecting a market frame of reference, or reviewing positioning health. Trigger phrases: \"position my product\", \"why aren't we resonating with customers\", \"pick a market category\", \"build a sales narrative\", \"fix our messaging\"."
allowed-tools:
  - Grep
  - Glob
  - Read
  - Task
---

# Obviously Awesome Positioning

This plugin gives you a repeatable, field-tested methodology for deliberately positioning products — drawn directly from April Dunford's *Obviously Awesome*. Whether you're positioning a new product from scratch or repositioning one that's drifting, the plugin walks you through the five (plus one) components, the 10-step process, and the three market positioning styles: **Head to Head**, **Big Fish Small Pond**, and **Create a New Game**. It's built for founders, product marketers, and executives who want positioning that makes the right customers say "this was made for me."

---

## 10-Step Positioning Process — Reference Map

| Step | Step Name | Reference |
|------|-----------|-----------|
| Step 1 | Understand the Foundations | [Positioning Foundations](references/core/positioning-foundations.md) |
| Step 2 | Understand the Five (Plus One) Components | [Five (Plus One) Components](references/core/five-plus-one-components.md) |
| Step 3 | Identify Best-Fit Customers | [Best-Fit Customers](references/core/best-fit-customers.md) |
| Step 4 | List Competitive Alternatives | [Competitive Alternatives](references/topics/competitive-alternatives.md) |
| Step 5 | Isolate Unique Attributes | [Unique Attributes](references/topics/unique-attributes.md) |
| Step 6 | Map Attributes to Value Themes | [Value Themes](references/topics/value-themes.md) |
| Step 7 | Determine Who Cares a Lot | [Target Segmentation](references/topics/target-segmentation.md) |
| Step 8 | Find a Market Frame of Reference | [Market Positioning Styles](references/patterns/market-positioning-styles.md) |
| Step 9 | Layer on a Relevant Trend (optional) | [Trend Layering](references/topics/trend-layering.md) |
| Step 10 | Capture and Implement Positioning | [Sales Story and Messaging](references/topics/sales-story-and-messaging.md) |

---

## Market Positioning Style Catalog

On first use, always consider all three styles together. Each has different risk, effort, and reward profiles.

| Style | When to use | One-line summary | Reference |
|-------|-------------|------------------|-----------|
| **Head to Head** | You can win on the existing category's purchase criteria | Compete directly against established players to lead the whole category | [Market Positioning Styles](references/patterns/market-positioning-styles.md) |
| **Big Fish Small Pond** | Category leader doesn't serve a meaningful subsegment you can own | Carve off a subsegment where the rules favor your strengths | [Market Positioning Styles](references/patterns/market-positioning-styles.md) |
| **Create a New Game** | Your value doesn't map to any existing category; you have patience and capital | Define an entirely new category and set the purchase criteria yourself | [Market Positioning Styles](references/patterns/market-positioning-styles.md) |

---

## Anti-Pattern Quick Reference

| Anti-pattern | Why harmful | Reference |
|--------------|-------------|-----------|
| **Weak Positioning** | Fails to communicate what your product is, why it's special, or why it matters — results in confused prospects, long sales cycles, heavy discounting, and high churn | [Positioning Foundations](references/core/positioning-foundations.md) |
| **Using a Traditional Positioning Statement** | Fill-in-the-blank templates reinforce the status quo and anchor you to existing competitors rather than guiding creative repositioning | [Five (Plus One) Components](references/core/five-plus-one-components.md) |
| **Defining Competitive Alternatives as Direct Product Competitors Only** | Customers may substitute spreadsheets, manual processes, doing nothing, or hiring someone — missing these distorts your unique attributes and value | [Competitive Alternatives](references/topics/competitive-alternatives.md) |
| **Listing Features Instead of Value Themes** | Features don't explain why customers should care; skipping the features→benefits→value chain leaves prospects unable to justify the purchase | [Value Themes](references/topics/value-themes.md) |
| **Firmographic-Only Segmentation** | Targeting by company size or industry alone doesn't identify who actually cares about your value — you need behavioral and attitudinal signals | [Target Segmentation](references/topics/target-segmentation.md) |
| **Trend Without Market Declaration** | Latching onto a trend (AI, sustainability, etc.) without anchoring it to a clear market category leaves customers without a frame of reference | [Trend Layering](references/topics/trend-layering.md) |
| **Positioning in a Vacuum** | Without a cross-functional team aligned on shared vocabulary, positioning breaks down between product, sales, and marketing | [Positioning Team and Vocabulary](references/core/positioning-team-and-vocabulary.md) |

Full anti-pattern catalog: [Positioning Anti-Patterns](references/anti-patterns/positioning-anti-patterns.md)

---

## What Would You Like to Do?

- **"Is my positioning broken?"** — Run `/diagnose-positioning` or read [Positioning Foundations](references/core/positioning-foundations.md) for the symptoms of weak positioning
- **"Who are my best-fit customers?"** — Run `/identify-best-fit-customers` or read [Best-Fit Customers](references/core/best-fit-customers.md)
- **"What are my real competitive alternatives?"** — Run `/list-competitive-alternatives` or read [Competitive Alternatives](references/topics/competitive-alternatives.md)
- **"How do I turn features into a value story?"** — Run `/map-value-themes` or read [Value Themes](references/topics/value-themes.md)
- **"Which market category should I choose?"** — Run `/select-market-frame` or read [Market Positioning Styles](references/patterns/market-positioning-styles.md)
- **"How do I turn positioning into a sales narrative?"** — Run `/build-sales-story` or read [Sales Story and Messaging](references/topics/sales-story-and-messaging.md)
- **"Review my existing positioning copy"** — Use the [`positioning-reviewer` agent](../../agents/positioning-reviewer.md)
- **"Plan a full repositioning project"** — Use the [`positioning-planner` agent](../../agents/positioning-planner.md)

---

## Commands Reference

| Command | What it does |
|---------|-------------|
| `/diagnose-positioning` | Evaluate current positioning against the symptoms of weak positioning ([details](../../commands/diagnose-positioning.md)) |
| `/identify-best-fit-customers` | Guide through finding your happiest customers and the patterns behind why ([details](../../commands/identify-best-fit-customers.md)) |
| `/list-competitive-alternatives` | Surface true competitive alternatives from the customer's perspective ([details](../../commands/list-competitive-alternatives.md)) |
| `/map-value-themes` | Walk the features→benefits→value chain and cluster into 1–4 value themes ([details](../../commands/map-value-themes.md)) |
| `/select-market-frame` | Evaluate all three positioning styles and select a market frame of reference ([details](../../commands/select-market-frame.md)) |
| `/build-sales-story` | Build a 7-step sales story arc from completed positioning ([details](../../commands/build-sales-story.md)) |
| `/review-positioning-health` | Periodic check for competitive drift, customer perception shifts, and market changes ([details](../../commands/review-positioning-health.md)) |

---

## Templates

Registry of all 12 fillable templates, in 10-step order. Paths are relative to this file (`skills/obviously-awesome/`).

| Template | Step | Backed by | Captures |
|----------|------|-----------|----------|
| [positioning-diagnosis.md](templates/positioning-diagnosis.md) | Diagnostic | `/diagnose-positioning` | symptom checklist + customer-vs-prospect gap + verdict |
| [best-fit-customers.md](templates/best-fit-customers.md) | 1 | `/identify-best-fit-customers` | 3–10 anchor customers + scope decision |
| [positioning-team-roster.md](templates/positioning-team-roster.md) | 2 | planner agent / skill | cross-functional team + facilitator |
| [vocabulary-and-baggage.md](templates/vocabulary-and-baggage.md) | 3 | planner agent / skill | shared vocabulary + baggage audit |
| [competitive-alternatives.md](templates/competitive-alternatives.md) | 4 | `/list-competitive-alternatives` | ranked 2–5 clusters of alternatives |
| [unique-attributes.md](templates/unique-attributes.md) | 5 | `/map-value-themes` | provable attributes + proof + consideration/retention |
| [value-themes.md](templates/value-themes.md) | 6 | `/map-value-themes` | features→benefits→value chain + 1–4 themes |
| [target-segment-profile.md](templates/target-segment-profile.md) | 7 | planner agent / skill | who-cares segment definition + worthiness test |
| [market-frame.md](templates/market-frame.md) | 8 | `/select-market-frame` | three style decision tables + chosen frame |
| [sales-story.md](templates/sales-story.md) | 10 | `/build-sales-story` | the 7-stage sales narrative arc |
| [positioning-canvas.md](templates/positioning-canvas.md) | 4–9 (capture at 10) | planner agent / skill | Five (plus one) consolidation; replaces the FOR/IS-A statement |
| [positioning-review-log.md](templates/positioning-review-log.md) | Ongoing | `/review-positioning-health` | append-only log of changes + reposition decisions |

---

## Reference Map

### Core Concepts
| File | What's inside |
|------|---------------|
| [Positioning Foundations](references/core/positioning-foundations.md) | What positioning is, why it matters, strong vs. weak positioning, the two positioning traps |
| [Five (Plus One) Components](references/core/five-plus-one-components.md) | The complete framework: competitive alternatives, unique attributes, value and proof, target market characteristics, market category, relevant trends |
| [Best-Fit Customers](references/core/best-fit-customers.md) | The circular dependency problem, how to identify best-fit customers as the anchor for all positioning work |
| [Positioning Team and Vocabulary](references/core/positioning-team-and-vocabulary.md) | Who belongs on the positioning team, business leader ownership, shared vocabulary alignment |

### Step-by-Step Topics
| File | What's inside |
|------|---------------|
| [Competitive Alternatives](references/topics/competitive-alternatives.md) | Step 4: what customers do without you, ranking by frequency, non-product alternatives |
| [Unique Attributes](references/topics/unique-attributes.md) | Step 5: consideration vs. retention attributes, provability requirements |
| [Value Themes](references/topics/value-themes.md) | Step 6: features→benefits→value chain, clustering into 1–4 value themes |
| [Target Segmentation](references/topics/target-segmentation.md) | Step 7: actionable segmentation, behavioral and attitudinal signals beyond firmographics |
| [Trend Layering](references/topics/trend-layering.md) | Step 9: the three-circle intersection model, when and how to layer a trend onto positioning |
| [Sales Story and Messaging](references/topics/sales-story-and-messaging.md) | Step 10: 7-step sales story arc, master messaging document, cross-team alignment |

### Patterns
| File | What's inside |
|------|---------------|
| [Market Positioning Styles](references/patterns/market-positioning-styles.md) | Head to Head, Big Fish Small Pond, and Create a New Game — when to use each, decision guidance, case studies |

### Anti-Patterns
| File | What's inside |
|------|---------------|
| [Positioning Anti-Patterns](references/anti-patterns/positioning-anti-patterns.md) | Full catalog organized by category: foundational mistakes, component-level errors, execution failures |
