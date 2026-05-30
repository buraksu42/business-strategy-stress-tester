# Business Strategy Stress Tester

A Claude Code / Claude.ai **skill** that puts an *existing operating business* through a structured, brutally honest strategic stress test — Socratic dialogue, deep web research, devil's-advocate critique — across three axes (**model viability × disruption pressure × transformation capacity**), then ships a printable HTML verdict report.

It's not a validation of an idea. It's not a brainstorm. It's not a friendly second opinion. It's the conversation you'd have with an experienced operator who's seen the category turn before: sharp, honest, useful — designed to find the load-bearing assumptions your *current* model rests on and pressure-test each one until it holds up or breaks, before another quarter is lost defending the wrong thing.

> **Pre-build idea?** Use the sibling skill [business-idea-stress-tester](https://github.com/buraksu42/business-idea-stress-tester) instead. This one is for businesses that already have revenue, customers, and momentum.

## What it does

The skill runs a 6-phase stress test:

1. **Map the current reality** — interview until the archetype, revenue mix, customer concentration, margin shape, and origin story are concrete (not abstract)
2. **Operating reality** — concentration & retention, cost structure & margin trajectory, cash & transformation capacity, and AI substitution exposure (value-chain scored GREEN/YELLOW/RED/BLACK)
3. **Devil's advocate** — pressure-test every assumption across model, disruption, and capacity; no escape ramps
4. **Deep research + macro audit** — 6–10+ web searches (competitors, AI-native entrants, category economics, shutdowns, regulation) plus a 5-box macro risk audit
5. **Verdict synthesis** — three independent axes → one of **EXPAND / DEFEND / REPOSITION / RESHAPE / HARVEST / EXIT** with confidence %, plus a named growth/transformation play with an explicit success threshold
6. **Visual report** — single-file HTML artifact, editorial or infographic style, print-ready

Built-in mechanics that keep it honest:

- **Customer Voice Test** — produce one verbatim customer quote from the last 90 days, or the verdict confidence is capped at 60% and EXPAND is off the table
- **On-screen unit economics** — when the user proposes "we'll add an AI tool" / "hire offshore" / "a junior can handle it", the math is computed live with realistic local rates, not waved at abstractly
- **Origin-pattern test** — surfaces the agency-built-product trap (relationship pull-through masquerading as product-market fit)
- **Competitor structure verification** — web research surfaces *visibility*; the operator carries *structure*. When they diverge, the operator wins and the disruption axis is re-scored
- **Pivot containment** — Phase 3 diagnoses, never offers exit doors; repositioning only surfaces in the Phase 5 verdict
- **Macro risk audit** — AI substitution / platform-supplier / commoditization / regulatory / demand-cycle, surfaced explicitly before the verdict
- **Local context aware** — adapts to the user's market (regulatory regime, talent costs, capital structure, sales cycle, competitive composition), responds in the user's language

## Triggers

The skill auto-activates when a user asks about the future direction of a running business — phrases like *"what should my agency do"*, *"should I expand or defend"*, *"is my model still viable"*, *"AI is killing our category"*, *"should we reposition"*, *"time to exit"*, *"how do I grow this"*, *"next 3 years for [industry]"* — or describes structural pressure (margin compression, AI commoditization, platform dependency, customer concentration), even conversationally without asking for analysis.

It does **not** trigger for pre-build ideas — those go to [business-idea-stress-tester](https://github.com/buraksu42/business-idea-stress-tester).

## Install

### Claude Code (CLI)

Drop the skill into your skills directory:

```bash
git clone https://github.com/buraksu42/business-strategy-stress-tester ~/.claude/skills/business-strategy-stress-tester
```

That's it. Next time you start a Claude Code session and describe an operating business under pressure, the skill activates automatically.

To update later:

```bash
cd ~/.claude/skills/business-strategy-stress-tester && git pull
```

### Claude.ai (web / desktop)

Download `business-strategy-stress-tester.skill` from this repo, then upload it via your Claude settings → Skills page.

## Usage

Just talk to Claude about your business. No slash command, no special invocation. Example openings that trigger the skill:

> *"We run a 15-person performance-marketing agency and AI is eating our deliverables. What do we do over the next 3 years?"*
>
> *"Our retention looks fine but margin's been compressing for two years. Expand or defend?"*
>
> *"A platform we depend on just changed their terms. Is the model still viable?"*

Claude will respond as the stress-tester: questions first, then research, then verdict, then HTML report. The whole flow takes 30–60 minutes of dialogue depending on how much pushback the model survives.

## Output

A standalone HTML report (printable to PDF) with:

- Verdict banner (EXPAND / DEFEND / REPOSITION / RESHAPE / HARVEST / EXIT + confidence %)
- Three score-meters (Model viability / Disruption pressure / Transformation capacity)
- TL;DR, the business overview, operating reality scored with reasoning
- AI substitution exposure — value-chain decomposition table with GREEN/YELLOW/RED/BLACK scoring and revenue-weighted exposure %
- Competitive landscape table
- Macro & disruption risk audit (5-box)
- Top 5–7 ranked devil's-advocate findings with mitigations
- A named growth/transformation path structured as 6–10 prioritized action blocks, ending in a milestone gate that defines when the verdict would flip
- All sources cited

Editorial style by default; ask for *"infographic-style"* / *"more visual"* / *"dashboard view"* to switch to the data-dense variant (radial gauges, 2×2 risk matrix, hero stats, heat-shaded value chain).

## Philosophy

> Honesty over politeness. Time over feelings.

A robust business defended by an exhausted founder, a strong team running an eroding model, or a great strategy with no cash to execute it — all three fail the same way: slowly, expensively, and in retrospect. The cost of being too soft is the operator spending another 18 months defending a position that already fell. The cost of being too sharp is one uncomfortable conversation.

You're not here to be encouraging. You're here to be useful.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, modify it, re-share it.

## Contributing

Issues and PRs welcome. The skill is intentionally a single SKILL.md file — keep it that way unless something genuinely needs reference material extracted (see "Notes & Roadmap" at the bottom of `SKILL.md`).
