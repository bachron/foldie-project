# Handoff: 160mm rotor list, combined T20 + G Line parts table, 451 wheel option
**Project**: Foldie Project (T20 + Brompton G Line builds)
**Date**: 25 Nov 2026 (iMac session)
**App version at time of handoff**: n/a (research docs only)

## Goal
Answer the weight of a Carbon-Ti Carousell rotor, then compile 160mm rotor options, merge the T20 and G Line parts lists into one table with a Bike column, and add the 451 wheel option after the user saw Oleg (Twisted Wheels) run 451 wheels with 35mm tyres.

## Done this session
- `G_Line_Current_Parts_List.md` row 12 and `G_Line_Build_Plan.md` rotor row: added published Carbon-Ti SteelCarbon 3 160mm weights (6-bolt 80g, Centerlock 98g; SteelCarbon 2 no longer on Carbon-Ti's site, est. 80-85g, unconfirmed).
- New `Rotor_List_160mm.md`: the existing T20 and G Line rotors merged, plus 19 new options (one short of the 20 asked for), and Centerlock shop prices for the Carbon-Ti SC3. Sources are Ti-Parts' measured weigh-in, Modern Bike (US$, no weights), Weight Weenies, Fair Wheel Bikes, absoluteBLACK, and the user's Google screenshots for Galfer in S$.
- New `T20_G_Line_Parts_List.md`: 64 rows, one per part, nothing merged. Bike column = `T20`, `G Line` or `Both`. 16 rows marked `Both` (#3, 12, 13, 14, 39, 40, 45, 47, 49, 51, 53, 54, 55, 56, 58, 59), applied on the user's "apply all". Rows #63 and #64 are the 451 wheelset and 35mm Box One tyre as G Line options.
- `G_Line_Tyre_List.md`: added a 451 option section and the confirmed Twisted Wheels 7.48 kg build spec (451mm BSD wheels 764g pair, 35mm Box One semi-slicks, Silverrock fork and triangle, 140mm Centerlock rotors 74g).
- All of the above committed and pushed to GitHub (`origin/main`).

## Pending edits not yet built
- None listed by the user.

## Not yet done
1. Verify the Box One tyre's real ETRTO size, weight and price (I did not check; I did not find any 35-451 tyre in my own searches).
2. 451 wheelsets: SMC 451 and Nonplus/Light Bicycle prices and weights not found; XDR freehub, rotor mount and 142x12 on the 451 options not checked.
3. Confirm the user's current rotor model and mount on the G Line (6-bolt confirmed, brand unknown) so the weights in the parts list can be real.
4. Rotor list gaps: no weights for Hope, SRAM, Magura, TRP, Campagnolo, Tektro, Shimano RT54/RT64; no 160mm 6-bolt Galfer found; shipping to Singapore not checked for Carbon-Ti direct.
5. T20 side: the extra T20 options (cranks, calipers, saddles, pedals, racks) stay in `T20_Build_Plan.md` and `T20_Build_Options.md`; the user has not yet merged those into the combined table.
6. Rows 13, 14, 40, 47, 55, 56 marked `Both` still need the checks: Praxis Doon crank and M30 bottom bracket on the G Line, which Ergon grips the G Line has, and whether the child seats move between bikes.
7. Weigh the G Line parts (the 10 kg measurement shows the estimates run about 17 percent high).

## Broken / failed approaches (don't repeat)
- Firecrawl cannot read Facebook, Reddit or YouTube; the Crawl4AI MCP failed to connect this session (ECONNREFUSED). Claude in Chrome worked, but only on tabs it opens itself: ask the user for the link, it cannot see tabs the user opened.
- Early answer used an eBay-derived estimate for the SteelCarbon 2 instead of opening Carbon-Ti's own site; the user caught it. Check the maker's site first.
- An early guess that Twisted Wheels used Panaracer Agilest came from a search excerpt and was wrong; the video says Box One.
- I first built a rotor table without checking the T20 files, which already had one (`T20_Build_Plan.md` section 3). Search the repo before building a new table.
- The first push failed with a GitHub "Internal Server Error" and went through on retry.
- Tyre fit: 406 and 451 are not interchangeable. 415 is not a size I could confirm.

## Key decisions
| Decision | Rationale |
|---|---|
| One table, one row per part, no merging; a Bike column of T20 / G Line / Both | The user wants to pick which parts go on which bike; identical parts get their own rows and are flagged "same as #N" |
| Marked 16 rows `Both` | The user said "apply all" to my suggested list; the Juin stem cap, seatpost clamp, rear block and easy wheels are marked `Both` because the T20 frame was bought unassembled |
| 451 added as options #63/#64, not replacements | The user has not chosen to change wheels; the G Line stays on 406 until they say so |
| G Line weights stay as estimates | The owner's 21 Nov weigh-in showed the bike at about 10 kg, so listed weights run about 17 percent high |

## Reference (don't duplicate — just point to it)
- `T20_G_Line_Parts_List.md`: the combined table (source of truth for the Bike column).
- `Rotor_List_160mm.md`: all rotor options and shops.
- `G_Line_Tyre_List.md`: 406 tyre options, plus the 451 section and the Twisted Wheels build.
- `G_Line_Build_Plan.md` and `G_Line_Current_Parts_List.md`: G Line plan and current parts.
- `T20_Build_Plan.md` and `T20_Build_Options.md`: T20 decisions and the full candidate lists.
- Source video: Twisted Wheels, "I Built the World's Lightest Brompton G-Line!" (YouTube, id R48IisijkLE; wheels chapter 7:44-11:27).

## Resume instructions
1. Run `git pull --ff-only` in `~/Developer/foldie-project`, then open `T20_G_Line_Parts_List.md`.
2. Ask the user which rows to change next; the likely next steps are confirming the six conditional `Both` rows (13, 14, 40, 47, 55, 56) and deciding whether to switch the G Line to 451 wheels (rows #63, #64).
3. If they want the 451 option researched further, find the Box One 35mm 20" tyre's ETRTO size, weight and price from Box One's site first, then the SMC and Light Bicycle 451 wheel prices.
4. If they want rotors bought, remember the G Line takes 6-bolt (Carbon-Ti SC3 6-bolt 160mm, 80g each, EUR 185 incl. VAT) and the T20 takes Centerlock.
