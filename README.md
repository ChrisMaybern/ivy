# IVY — Intelligent Voice for You

Real-time sales companion by Maybern. Listens to the room, detects signals, pushes rebuttals, tracks discovery depth, and coaches reps through M1 and M2 conversations.

## Quick Start

1. Open `ivy.html` in Chrome
2. Enter PIN: `2026`
3. Fill in pre-call data (GP name, AUM, fund count, competitor tools)
4. Hit **START SESSION** → **LIVE**
5. IVY listens and reacts in real-time

## Files

| File | What It Is |
|------|-----------|
| `ivy.html` | The app — open in Chrome, sit next to Zoom |
| `brain.json` | The intelligence engine — questions, rebuttals, stories, signals |

## Brain Stats

- **63 top-level keys** across sales intelligence, pricing, competitor routing, customer stories
- **32 M1 questions** + **19 M2 questions** with L1/L2/L3 depth levels
- **18 signal rebuttals** triggered by 23 detection groups (70+ phrases)
- **26 customer stories** surfaced contextually as proof points
- **15 competitor talk tracks** with specific reframe strategies
- **Priority tiers** (must-ask / situational / depth) on every question
- **Dynamic queue** re-ranks after every client response
- **Thread continuity** keeps discovery flowing on the same topic
- **Vagueness detection** pushes L2 when client hedges
- **Talk-time nudge** warns when rep is monologuing

## Features

- **Voice-first** — Web Speech API, no typing needed
- **Signal detection** — hears objections and pushes rebuttals in royal blue
- **Proof points** — customer stories surface in purple when pain signals fire
- **Competitor intel** — pink cards with specific talk tracks when a competitor is named
- **Karaoke tracking** — words highlight as the rep speaks the rebuttal
- **Pre-call data** — GP name, AUM, fund count personalize question wording
- **Buyer profile routing** — in-house/outsourced/hybrid auto-detected, irrelevant questions hidden
- **Stage progression** — auto-detects open → advancing → confirming
- **Post-call export** — downloads markdown summary with MEDDPICC coverage
- **Session persistence** — pre-call data survives page refresh
- **PIN protected** — default PIN: 2026
- **Sidebar optimized** — 380px default, 520px expanded mode

## Updating the Brain

Edit `brain.json` directly. Key areas:

- `meeting_types[0].stages[].discovery_questions` — M1 questions
- `meeting_types[1].stages[].discovery_questions` — M2 questions  
- `signal_bridge_rebuttals` — signal-triggered responses
- `customer_story_bank` — proof point stories
- `competitor_responses` — competitor talk tracks
- `pricing_intelligence` — pricing rebuttals and prevention plays

Push changes to main. The app loads the brain on startup.

## Deploy

**GitHub Pages:** Settings → Pages → Source: main branch → Save. Live at `[org].github.io/ivy`

**Custom domain:** Add CNAME file with `ivy.maybern.com`, configure DNS.

---

Built by Maybern. Confidential.
