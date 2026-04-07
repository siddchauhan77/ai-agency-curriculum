# Build Recap — AI Agency Curriculum

**Date built:** April 7, 2026
**Built with:** Claude Code (claude-sonnet-4-6)
**Time to build:** ~1 session

---

## What Was Built

A single-file interactive curriculum tracker (`index.html`) designed to replace a $144/mo paid course. Built entirely from free public resources.

### Features
- 8 module cards with teal/dark AIS+-style aesthetic
- Per-lesson checkboxes, resource links, time estimates, and notes
- Progress bars per module + overall progress in the header
- Full `localStorage` persistence — survives page refreshes
- Reset all button with confirmation guard
- GitHub Pages hosted — accessible from any device

---

## How It Was Built

**Stack:** Single HTML file, Tailwind CSS (CDN), vanilla JS, localStorage

No framework, no build step, no dependencies. Opens instantly in any browser. Data model is a flat key-value object keyed by lesson ID, stored in `localStorage`.

**Security note:** All DOM construction uses `createElement`/`textContent`/`.value` — no `innerHTML` with user-controlled data. Notes (user input) are set via `textarea.value` property, not injected via template literals.

---

## Curriculum Research Sources

Content was sourced by searching and fetching the following:

- **Nick Saraev** — fetched `nicksaraev.com/5-more-automations-you-can-sell-today-for-1-500-or-10-000/` for his 5 specific builds + price ranges
- **Nate Herk** — fetched `startupseries.io/how-nate-herk-sold-ai-agents/` for the 4 agents he sold for $23k (build descriptions, prices, lessons)
- **Pricing data** — pulled from `digitalagencynetwork.com/ai-agency-pricing/` and `oreateai.com` for real 2025 market rates
- **Local sales scripts** — `sidehustlemastery.com` and `mewrcreate.com` for in-person + digital offer strategy
- **Justin Welsh** — 4 specific free articles linked directly for DMs and LinkedIn outreach

---

## Curriculum Decisions

**Why Nick Saraev + Nate Herk for portfolio builds?**
Both have documented, real client sales with prices attached. Not theory — Nate sold a personalised outreach writer for $1,650 and an AI concierge for ~$12,000. Nick's builds have a 3-component framework: clear deliverable, hot-button pain, templateable. These aren't random project ideas.

**Why 4 sales modules out of 8?**
Sales was the identified weak skill. Lead finding, outreach, closing, and pricing each get their own module rather than being bundled together.

**Why a local walk-in script in Module 4?**
Digital-only outreach is competitive. Local businesses (gyms, dentists, restaurants, real estate) have money, real pain, and almost no one walking in offering AI automation. Lower competition, faster trust.

**Why localStorage over a backend?**
Personal use only. No accounts, no server, no cost. Instant setup, works offline, survives indefinitely.

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | The full curriculum tracker app |
| `README.md` | Project overview + case study for GitHub |
| `RECAP.md` | This file — build decisions + session log |

---

## Next Steps (when ready)

- [ ] Complete Module 1 and Module 3 first — foundation + portfolio before any outreach
- [ ] Start with Build #4 (Nate Herk's Outreach Writer) — lowest complexity, proven $1,650 sell price
- [ ] Walk into 3 local businesses after first portfolio build is done
- [ ] Revisit pricing module before every client conversation
