# obviously-awesome-positioning

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) plugin based on *[Obviously Awesome](https://www.aprildunford.com/obviously-awesome)* by April Dunford.

It packages April Dunford's positioning methodology — the 10-step process, the five (plus one) components framework, the three market positioning styles, and the book's anti-pattern catalog — into commands, agents, and an auto-activating skill for product positioning work.

## Install

```bash
claude plugin marketplace add dchuk/obviously-awesome-positioning
claude plugin install obviously-awesome-positioning@obviously-awesome-positioning
```

## Skill

The plugin includes an auto-activating skill — `obviously-awesome-positioning` — that brings the methodology into any conversation when relevant, without you running a command. It triggers on phrases like *"position my product"*, *"why aren't we resonating with customers"*, *"pick a market category"*, *"build a sales narrative"*, or *"fix our messaging"*.

## Commands

Run these in order to work through the full positioning process, or invoke any one on its own. Each accepts an optional argument (a product name, description, or path to a positioning doc).

| Command | Purpose |
|---------|---------|
| `/obviously-awesome-positioning:diagnose-positioning` | Diagnose whether your product has a positioning problem using the book's symptom checklist |
| `/obviously-awesome-positioning:identify-best-fit-customers` | Identify best-fit customers to anchor all subsequent positioning work |
| `/obviously-awesome-positioning:list-competitive-alternatives` | List true competitive alternatives from the customer's perspective |
| `/obviously-awesome-positioning:map-value-themes` | Map product attributes to value themes using the features→benefits→value chain |
| `/obviously-awesome-positioning:select-market-frame` | Select a market frame of reference using Head to Head, Big Fish Small Pond, or Create a New Game |
| `/obviously-awesome-positioning:build-sales-story` | Build a sales story from completed positioning using the 7-step arc |
| `/obviously-awesome-positioning:review-positioning-health` | Conduct a periodic positioning review and decide whether to reposition or hold |

## Templates

Blank, fillable artifacts to capture the output of each step — kept in `skills/obviously-awesome/templates/`. They reuse each step's exact output structure and bake in the book's hard constraints (e.g. 2–5 competitive-alternative clusters, 1–4 value themes, provable attributes only), so an artifact stays consistent across sessions and can be versioned alongside your positioning work. Most back a command; the four that fill steps with no dedicated command are surfaced by the **planner agent** and the **skill registry**. Listed in 10-step order:

| Template | Step | Backed by | Captures |
|----------|------|-----------|----------|
| `positioning-diagnosis.md` | Diagnostic | `/diagnose-positioning` | Symptom checklist + customer-vs-prospect gap + verdict |
| `best-fit-customers.md` | 1 | `/identify-best-fit-customers` | 3–10 anchor customers + product-vs-company scope decision |
| `positioning-team-roster.md` | 2 | planner agent / skill | Cross-functional team + facilitator decision |
| `vocabulary-and-baggage.md` | 3 | planner agent / skill | Shared vocabulary + positioning-baggage audit |
| `competitive-alternatives.md` | 4 | `/list-competitive-alternatives` | Ranked 2–5 clusters of what customers would do without you |
| `unique-attributes.md` | 5 | `/map-value-themes` | Provable attributes with proof source + consideration/retention |
| `value-themes.md` | 6 | `/map-value-themes` | Features→benefits→value chain and the 1–4 named themes |
| `target-segment-profile.md` | 7 | planner agent / skill | Who-cares segment definition + worthiness test |
| `market-frame.md` | 8 | `/select-market-frame` | The three style decision tables + the chosen frame of reference |
| `sales-story.md` | 10 | `/build-sales-story` | The 7-stage sales narrative arc |
| `positioning-canvas.md` | 4–9 (capture at 10) | planner agent / skill | Five (plus one) consolidation; replaces the FOR/IS-A statement |
| `positioning-review-log.md` | Ongoing | `/review-positioning-health` | Append-only log of landscape changes and reposition decisions |

## Agents

- **obviously-awesome-positioning-planner** — Plans and sequences a positioning or repositioning effort, guiding you through the full 10-step process and adapting to whether you're positioning from scratch, repositioning an existing product, or responding to a competitive landscape change.
- **obviously-awesome-positioning-reviewer** — Reviews existing positioning (website copy, pitch deck, product description, messaging doc, or positioning statement) against the book's anti-pattern catalog, the five (plus one) components framework, and the three market positioning styles.

## Reference Files

The skill draws on 12 reference files:

- `references/core/` — positioning-foundations, five-plus-one-components, best-fit-customers, positioning-team-and-vocabulary
- `references/patterns/` — market-positioning-styles
- `references/topics/` — competitive-alternatives, value-themes, unique-attributes, target-segmentation, trend-layering, sales-story-and-messaging
- `references/anti-patterns/` — positioning-anti-patterns

## Layout

```
obviously-awesome-positioning/    # the plugin
├── commands/                     # 7 slash commands
├── agents/                       # 2 agents
└── skills/obviously-awesome/     # skill + 12 reference files + 12 templates
.claude-plugin/marketplace.json   # marketplace manifest
```

---

Generated by [Franklin](https://github.com/mcrundo/franklin) from *Obviously Awesome*.
