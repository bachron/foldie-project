# Handoff: Helmet comparison table
**Project**: T20 G Line build (side task: helmet shopping)
**Date**: 2026-10-12
**App version at time of handoff**: n/a
**Branch**: `claude/helmet-comparison-table-yivvn9` (pushed; no PR opened)

## Goal
Build a comparison table of road/urban helmets the user is considering (weight, price, MIPS, notes), then find the cheapest place to buy the pick.

## Done this session
- Created `Helmet_Comparison.md`: 14 helmets, a lightest-to-heaviest ranking, and an "Items to confirm" list. Data is from web searches of retailer listings and reviews on 9 Oct 2026.
- Helmets: Giro Agilis MIPS, Giro Aries Spherical, POC Omne Air MIPS, POC Ventral Air MIPS, MET Trenta 3K Carbon MIPS, MET Rivale MIPS, Kask Elemento / Protone / Valegro / Utopia, Abus AirBreaker 2.0 MIPS, Bell XR Spherical, Thousand Heritage, Van Rysel RCR MIPS.
- Van Rysel: user wrote "R2R", which doesn't exist. They confirmed it is the **RCR MIPS** (270g claimed, 278.6g measured, £79.99).
- Cheapest RCR MIPS found: **€70 at Alltricks** (list €90). UK list is £79.99 at Van Rysel UK. The non-MIPS version is ~£60.

## Pending edits not yet built
- None.

## Not yet done
- Local pricing for the RCR MIPS: the user's country is unknown, and results so far are UK/EU only. Ask where they are, then search local stock.
- User has not answered the open questions in `Helmet_Comparison.md`: "met," with no model (skipped), POC "Omnie" assumed Omne Air MIPS, "Thousands" assumed Thousand Heritage, "Utpopia" assumed Kask Utopia.
- No final helmet pick made yet.

## Broken / failed approaches (don't repeat)
- "POC Omne Air Spherical" returned nothing; only the Omne Air MIPS, Lite and Ultra exist in results.
- Searching "Van Rysel R2R" finds nothing. Don't search it again.
- Kask "No MIPS" entries are confirmed only for the Elemento. The rest rely on general knowledge. Verify before relying on them.

## Key decisions
| Decision | Rationale |
|---|---|
| Weights are medium size unless noted; prices are approximate list prices | Sources disagree by size, region, certification (CE vs CPSC) and sale |
| Kept the file separate from the T20 build docs | Helmets aren't part of the bike parts tracker |

## Reference (don't duplicate, just point to it)
- `Helmet_Comparison.md` holds the full table and sources-of-doubt list.
- `T20_Build_Options.md` is the bike parts tracker. Its table style (Option / Weight / Notes) was the model for the helmet table.

## Resume instructions
1. Ask the user which country they're buying in, then search for the cheapest local RCR MIPS price.
2. Ask whether they want extra columns (aero, vents, Brompton fit) or a final recommendation.
3. Commit and push any changes to `claude/helmet-comparison-table-yivvn9`. Do not open a PR unless asked.
