# Handoff: G Line seatpost/saddle, gearing, tyre choice, 10 kg weight rebase
**Project**: foldie-project (`bachron/foldie-project`, `~/Developer/foldie-project`)
**Date**: 2026-11-22
**App version at time of handoff**: n/a (markdown research repo)

## Goal
Continue the Brompton G Line (bought used, size S, converting to M) build research: parts sourcing, seatpost/saddle tables, gearing, tyre choice, and a corrected weight baseline. HEXATI T20 files are separate and unchanged.

## Done this session (all committed and pushed; origin/main = HEAD)
- `G_C_Line_Seatpost_Saddle_List.md` (new): carbon seatpost table with fit columns for G Line M (560 mm max) and C/P Line, Carousell H&H 540 mm listings with weights, saddle table. Decision on file: **H&H carbon 540 mm fits both G Line and P Line.** The G Line's current Hexagon Ti post (about 170-240 g, estimated, 560 mm) is probably as light as any carbon post: weigh it first.
- `G_Line_Build_Plan.md`: gearing section for 54T Juin chainring x 10-36T 12-speed XDR cassette (**owner confirmed as final**). Tyres now 54-406 vs future 42-406: 54-406 gives 108 gear inches (10T) to 30 (36T); 42-406 gives 102 to 28 (about 5% easier). Circumferences are estimates (about 1,590 mm and about 1,505 mm, +/-1%).
- **Tyre choice switched to Continental Contact Urban 42-406** (710 g pair), in `G_Line_Tyre_List.md`, build plan and parts list.
- **Weight rebase:** owner weighed the current build at about **10 kg** (rough scale); the old 12.0 kg estimate was too high. Redone by scaling all old-part weights by 10/12 and subtracting new-part weights: savings about -1.5 kg (range -1.0 to -2.0), **finished bike about 8.5 kg (8.0-9.0)**. Per-upgrade savings: set -830 g, Ti stem -265 g, bar -190 g, pedals -105 g, tyres -100 g. S$ per kg: set about 1,900, Ti stem about 3,700, pedals about 500, tyres about 1,400, overall about 1,850.
- Earlier this session (already in repo): stem market scan (no used G Line M or Ti M stem found in Singapore), Quad Lock pricing, C Line bar diameter, 140 mm and 160 mm centre-lock/6-bolt rotor lists, brake-side explanation.

## Pending edits not yet built
- None batched.

## Not yet done
1. **Foldie Build hub not republished** (artifact `Jga26EY9GJLgF9oPCTejtZ`, built from `private/build_hub.py`): still shows the old 12.0 kg / 9.8 kg numbers. Owner was asked and did not answer.
2. **Brain Studio report not sent** (project id `t20-bike-builder`; CLAUDE.md says report on milestone changes).
3. **M stem still unsourced.** Options: Chris Yeo Ti M stem S$980 (now looks poor value: could save as little as about 150 g), new G/T-Line stem about GBP 400 at Brilliant Bikes, or a "wanted: G Line M stem" post (needs explicit owner yes before posting).
4. **Front brake side:** G Line front brake is on the right, all of the owner's other bikes use left. Swapping hoses between levers likely needs a bleed; best done with the M-stem/Silverrock fork work. Not decided.
5. **Saddles:** one for P Line, one for the mini velo (worn out). Table exists for Brompton saddles; **mini velo saddle not researched** (separate post and clamp).
6. 42-406 Contact Urban price and a Singapore seller not checked (S$140 is the 50-406 estimate).
7. Optional: add `G_Line_Tyre_List.md` and `G_C_Line_Seatpost_Saddle_List.md` to the README G Line row. Weigh stock stem, fork, bar, pedals, one G-One tyre and the Hexagon post to replace estimates.
8. Open checks: 50 T or 48 T chainring option on 42-406 (not checked with Juin); SRAM derailleur must be rated for 36T; chain length with tensioner; rim width and carbon fork/triangle clearance for 42-406 (ask Chris Yeo).

## Broken / failed approaches (don't repeat)
- Crawl4AI MCP failing to connect (ECONNREFUSED) all session; used Firecrawl then browsers per the web-tool order rule.
- Firecrawl cannot scrape reddit.com (search excerpts only). Carousell needs the built-in browser; Facebook needs Claude in Chrome.
- I wrongly said the M conversion needs a 600 mm/extended post. Owner: current post is 560 mm max and not fully used; 540 mm is fine. Corrected in file.
- The 12.0 kg baseline and the stock-part weights behind it were wrong; do not reuse them.

## Key decisions
| Decision | Rationale |
|---|---|
| Carbon seatpost 540 mm (H&H) for both G Line and P Line | Owner: 540 fits both; C and P share length |
| Cassette 10-36T 12-speed with 54T ring, final | Owner "quite sure" |
| Future tyre Contact Urban 42-406 | Owner plan 40-45-406; 42-406 is the Contact Urban in that range |
| Weight baseline 10 kg measured | Owner's own rough weighing |

## Reference (don't duplicate)
- `G_Line_Build_Plan.md` (sections 2 gearing, 4 tyres, 7 weight and cost), `G_Line_Current_Parts_List.md`, `G_Line_Tyre_List.md`, `G_C_Line_Seatpost_Saddle_List.md`
- Earlier handoff: `HANDOFF_g-line-build-plan-and-upgrades_2026-11-19.md`
- `C_Line_Build_Plan.md` for the carbon-post vs rear child-seat conflict
- Global `~/.claude/CLAUDE.md` for sync, Brain Studio and web-tool rules

## Resume instructions
`git pull --ff-only`, then ask the owner for go-ahead on the hub republish (run `private/build_hub.py`, republish artifact `Jga26EY9GJLgF9oPCTejtZ`) and send the Brain Studio report. Then pick up item 3 (M stem) or item 5 (P Line and mini velo saddles) as the owner chooses. Do not post anything on Carousell or Facebook without an explicit yes.
