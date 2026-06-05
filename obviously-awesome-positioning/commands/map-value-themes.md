---
description: Map product attributes to value themes using the features→benefits→value chain
argument-hint: "[product name or positioning doc]"
---

# Map Value Themes

**Purpose:** Walk through Steps 5 and 6 of the positioning process — isolating unique attributes, then mapping them through the features→benefits→value chain into 1–4 coherent value themes. Use this command after you have a competitive alternatives list and before you select a market frame of reference.

## When to use

- You've completed Step 4 (competitive alternatives list) and are ready to move to value mapping
- Your current positioning describes features but doesn't connect them to customer goals
- You're repositioning and need to re-examine what value your product actually delivers
- Your sales team pitches features but struggles to articulate why customers should care

## Steps

1. **Collect inputs.** Ask the user to provide:
   - The competitive alternatives list from Step 4 (or run `list-competitive-alternatives.md` first if it doesn't exist)
   - A product description, feature list, or existing positioning doc — any artifact describing what the product does or has

2. **Isolate unique attributes (Step 5).** Build a raw attribute table. For each attribute:
   - List every capability, characteristic, or company-level trait the product has that competitive alternatives do **not** — include weak candidates and those of uncertain value
   - For tech products, start with patented or technically proprietary features; for service companies, start with team skills, specialized experience, partnerships, and proprietary processes
   - Ask the user: "Why did your happiest customers choose you?" — surface any attributes hidden in customer language
   - For each claimed attribute, apply the provability test: is this based on an objective, measurable fact? If the attribute is a benefit claim ("easy to use", "great support"), ask the user for the underlying measurable attribute or flag it for removal
   - Accept third-party validation (analyst reports, independent reviews, approved customer quotes) as proof for otherwise subjective attributes
   - Flag each attribute as **Consideration** (matters at purchase time) or **Retention** (matters at renewal); mark consideration attributes as higher priority for positioning
   - Do **not** rank or group yet — capture the broadest possible set

   Output a table:

   | # | Attribute | Provable? (Y/N/Third-party) | Consideration or Retention |
   |---|-----------|----------------------------|---------------------------|
   | 1 | …         | …                          | …                         |

   Offer the user the blank template at `../skills/obviously-awesome/templates/unique-attributes.md` — populate it directly with the generated attribute table, or hand it over for the user to fill in.

3. **Build the features→benefits→value chain (Step 6, part 1).** For each attribute from the table above:
   - **Feature** — what the product does or has (carry forward from Step 5)
   - **Benefit** — what the feature enables for customers (functional outcome)
   - **Value** — how the benefit maps to a specific goal the customer is trying to achieve, expressed in the customer's own terms

   Note: a single feature can yield multiple value points. A combination of features may yield additional value points not visible from any single feature alone. Capture all of them.

   Output a table:

   | Feature | Benefit | Value (customer goal) |
   |---------|---------|----------------------|
   | …       | …       | …                    |

4. **Cluster into value themes (Step 6, part 2).** Review the full list of value points:
   - Identify natural groupings — value points that serve the same or closely related customer goals
   - Name each cluster in customer-facing language (e.g., "supports remote environments", "reduces compliance risk")
   - Consolidate until you have **1–4 value themes** that represent the most critical, differentiating value of the product
   - If the exercise produces a single value theme, that is a valid outcome — do not force additional clusters

   Output a numbered list:

   1. **[Theme Name]** — [1-sentence description of the customer goal this theme serves]
      - Supporting value points: …
   2. …

   Offer the user the blank template at `../skills/obviously-awesome/templates/value-themes.md` — it captures both the features→benefits→value chain (Step 6 part 1) and the 1–4 value theme summary. Populate it directly with the generated tables, or hand it over for the user to fill in.

5. **Prioritize consideration attributes.** Review the final themes. Flag any theme that is supported exclusively by retention attributes — these are important for customer success but should not anchor external positioning. Confirm at least one theme is anchored in consideration attributes.

6. **Hand off to next steps.** Present the 1–4 value themes as input-ready for:
   - Step 7: target segmentation (who cares most about which themes?) — see `target-segmentation.md`; offer the user the blank template at `../skills/obviously-awesome/templates/target-segment-profile.md` to capture the who-cares segment definition
   - Step 8: market frame of reference selection — see `select-market-frame.md`

## Verify

The command succeeds when:

- [ ] Every attribute in the Step 5 table is either marked provable or flagged for removal/evidence
- [ ] Every attribute has at least one row in the features→benefits→value chain table
- [ ] The final output contains 1–4 named value themes (no more, no fewer)
- [ ] Each theme is expressed in customer goal language, not product feature language
- [ ] At least one theme is anchored in consideration attributes

If any theme is still expressed as a feature or benefit rather than a customer goal, cycle back through the chain for that theme.

## Notes

**Anti-patterns to watch for:**

- **Frankencake** — a positioning attempt that lists every attribute without clustering, producing a message customers cannot process. See [positioning anti-patterns](../skills/obviously-awesome/references/anti-patterns/positioning-anti-patterns.md) for the full catalog.
- Unprovable benefit claims masquerading as attributes (e.g., "industry-leading support") are a foundational mistake — enforce the provability test in Step 2 above.

**Related reference files:**

- [Unique attributes deep dive](../skills/obviously-awesome/references/topics/unique-attributes.md) — consideration vs. retention attributes, provability requirements
- [Value themes deep dive](../skills/obviously-awesome/references/topics/value-themes.md) — the features→benefits→value chain, clustering rules, 1–4 cluster guidance
- [Five (plus one) components](../skills/obviously-awesome/references/core/five-plus-one-components.md) — where value themes fit in the full positioning model
- [Competitive alternatives](../skills/obviously-awesome/references/topics/competitive-alternatives.md) — Step 4 output that feeds this command
- [Unique Attributes template](../skills/obviously-awesome/templates/unique-attributes.md) — fillable blank for this command's output
- [Value Themes template](../skills/obviously-awesome/templates/value-themes.md) — fillable blank for this command's output
- [Target Segment Profile template](../skills/obviously-awesome/templates/target-segment-profile.md) — fillable blank for the Step 7 hand-off
