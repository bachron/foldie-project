# Handoff: Brompton G Line (upgraded, bought used) build plan and chosen upgrades
**Project**: Foldie Project (G Line build, separate from the T20 and the Black Lacquer C Line)
**Date**: 2026-11-19 (work done 18 Nov 2026 on the iMac; handoff written afterwards from the MacBook Air because none was left)
**App version at time of handoff**: n/a (research docs only)

## Goal
Plan the rebuild of a used Brompton G Line Asri bought on 18 Nov 2026 (Carousell, size S, Juin hydraulic brakes, SRAM Force AXS 1x12, SMC carbon wheels): list what it has, choose weight-saving upgrades, and convert it from size S to size M.

## Done this session
Nine commits on 18 Nov, 12:49 to 13:57 (`17eebeb` to `0d48cdc`):
- `G_Line_Upgraded_Build.md`: spec as listed, price check (new G Line S$4,950; rebuilding this spec new about S$9,200-10,900), S to M conversion notes, brake swap plan with the mini velo, why the wheelset swap with the mini velo is a no, open actions. Price paid and delivery are deliberately not recorded (public repo).
- `G_Line_Current_Parts_List.md`: current parts with estimated weights and S$ prices. Today's weight is about 12.0 kg (range 10.9-13.1), unweighed. Stock G Line is about 14.8 kg.
- `G_Line_Build_Plan.md`: sectioned plan (frameset, drivetrain, brakes, wheels and tyres, cockpit, small parts), benchmarks, weight and cost scenarios, open decisions.
- `G_Line_Tyre_List.md`: 406 tyre options and the choice below.
- `README.md`: G Line row added; T20 row relabelled "separate from the Brompton G Line build".
- **Five upgrades chosen** (estimate about 9.8 kg, about -2.2 kg, about S$2,755 total):

| Part | Replacement | Price (S$) |
|---|---|---|
| Stem | Ti stem, Chris Yeo | 980 |
| Fork + rear triangle | Silverrock carbon set, Chris Yeo (the quote is fork **and** triangle, corrected 18 Nov) | 1,580 |
| Handlebar | Schmolke carbon 31.8mm | free (provided) |
| Pedals | Carbon look-alike sold as WOOdman, Carousell | about 55 |
| Tyres | Continental Contact Urban 50-406 (860g pair) | about 140 (est., SG price not found) |

## Pending edits not yet built
- None.

## Not yet done
In rough priority order (full list in `G_Line_Build_Plan.md` section 8):
1. Weigh the bike, then the stock bar, pedals, fork, stem, seatpost, saddle, and one tyre. This settles most "estimate" rows.
2. Confirm with Chris Yeo: the Ti stem is **M height** and fits the **Chris King** headset; the Silverrock set fits (142x12 rear hub, flat-mount rear caliper, derailleur hanger, Juin rear block; fork flat mount, 100x12, 160mm rotors, tyre clearance for 50mm and 54mm).
3. Seatpost for the M conversion: the current Hexagon Ti post may be too short.
4. Test ride S and M before committing to the M conversion (a 177cm tester found M too big).
5. Mini velo: measure brake mount type and tyre clearance before moving the Juin 4-pot set to it; fit R1 hybrids with Extralite UltraLevers 3S on the G Line.
6. Check rim width with SMC (Plume DW2 C22-25 or T22-30) and find a Singapore price for the tyres.
7. Check the look-alike pedals on arrival (thread, quick-release fit, real weight).
8. Decide whether a child seat goes on this bike (the Ti stem is the one that fits the Thule Yepp Mini mount).
9. Ask Asri to pick further candidates from the T20 tables (crank and M30 bottom bracket, saddle, rack, dropout hanger). Target weight is not set.

## Broken / failed approaches (don't repeat)
- Silverrock was first read as a stem quote; it is the fork and rear triangle set. Fixed on 18 Nov.
- T20 plan's Shimano XT M8100 derailleur does not fit this bike (XDR 12-speed); T20 centre-lock rotors do not fit (6-bolt here).
- Swapping wheelsets with the mini velo does not work (54mm tyres will not clear, thru-axle vs QR, XDR vs HG 11-speed).
- Cautions for the carbon parts: low rider-weight limits, and a child seat can void the warranty.

## Key decisions
| Decision | Rationale |
|---|---|
| Ti stem (not carbon) | Only the Ti stem meets G Line geometry for the Thule Yepp Mini mount |
| Silverrock fork + triangle set, S$1,580 | Best value per kg saved (about S$1,300/kg); stacks with the stem |
| Contact Urban 50-406, not 55-406 | Saves weight (about -115g) instead of adding about 145g; keeps puncture protection for city use |
| Rule: a part moves from "Candidates" to "Chosen" only when Asri says so | Keeps the plan Asri's, not Claude's |
| Keep: Chris King headset, Juin blocks and easy wheels, XDR wheelset, chain tensioner, rotors | Nothing lighter fits or the gain is not worth it |

## Reference (don't duplicate, just point to it)
- `G_Line_Build_Plan.md`, `G_Line_Upgraded_Build.md`, `G_Line_Current_Parts_List.md`, `G_Line_Tyre_List.md`
- `T20_Build_Plan.md` and `T20_Build_Options.md` (candidate menu; unchanged, separate build)
- Latest earlier handoff: `HANDOFF_donor-shortlist-K-and-start-offers_2026-11-14.md` (C Line donor shortlist; no seller contacted yet, still open)

## Known issue to fix
- `README.md`: a blank line sits between the C Line row and the G Line row, so the G Line row (and the Aceoffix row below it) renders outside the table in most viewers. Remove the blank line.

## Resume instructions
Start from `G_Line_Build_Plan.md` section 8. First ask Asri whether the bike has been weighed and whether Chris Yeo has confirmed the M stem height and the Silverrock fit, then update the plan with the answers. Fix the README blank line first (one-line change). Don't mark any new part "Chosen" until Asri says so. Keep the price paid out of the repo.

Reminders: think before coding, simplicity first, surgical changes. Show the donor shortlist table exactly if asked.
