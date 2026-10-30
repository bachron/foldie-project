# Handoff: C Line crank arms table and donor shortlist re-rank
**Project**: Foldie project (C Line black lacquer Brompton build)
**Date**: 2026-10-30
**App version at time of handoff**: n/a (markdown research repo)

## Goal
Clean the C Line crankset research down to single-ring crank arms, then add new Carousell listings (I, J) to the donor shortlist and re-rank it for Asri's mod plan and budget.

## Done this session
- `C_Line_Parts_List.md`: replaced the "Cranksets and crank arms" table with a crank-arms-only, single-ring table plus a fit gate (stock JIS square-taper 119 mm BB vs 24/28/30 mm spindle arms). Dropped 2x/road sets (Praxis Zayante, Alba-GR, Doon+rings, Shimano 105, FSA Gossamer, Ridea BCSB). `C_Line_Parts_Research.md` still holds the old raw table.
- `C_Line_Donor_Shortlist.md`: added **I** (H6L Black Edition, S$1,950) and **J** (C Line "7speed", S$2,500), each with a detail section; table rows reordered by recommendation (letters unchanged): B, E, I, C, F, J, A, D, H, G; replaced the recommendation block with a dated one for the mod plan.
- Memory notes saved: show shortlist table with recommendation at the bottom; Asri's mod plan and budget.

## Pending edits not yet built
- None.

## Not yet done
- Ask sellers: B (confirm the SMC carbon bar and other mods), E (frame year vs Ti triangle fit), I (receipt, frame year, bar), J (what the "7speed" hub/derailleur is), C/F/H per existing "Ask" lists.
- Verify crank-arm fit on a C Line: which arms take the stock JIS BB, whether a 30 mm BB needs the shell faced and re-tapped (Condor claim, one source), and the H&H square-taper set (about 400 g arm + spider, price not re-checked).
- Aceoffix CNC Brompton crank (320 g set, S$162.50) was not found in searches; unverified.
- Remarks column is still "—" for every bike (nobody contacted or viewed).
- Detail sections below the table are still in old letter order (A..J), not recommendation order.

## Broken / failed approaches (don't repeat)
- WebFetch on bromptonkitchen.com returned 429; WebSearch snippets gave the H&H specs instead.
- Carousell needs Claude in Chrome (wait ~6 s, then `get_page_text`); built-in fetch tools get blocked.
- Repo is public: no seller names, phone numbers or tracking-param URLs in the files.

## Key decisions
| Decision | Rationale |
|---|---|
| Single chainring only, arms-only table | Asri cannot build a Brompton with 2 chainrings; ring and spider chosen separately |
| Paper trail and service history not valued | Asri said they are not needed; plan replaces tyres/tubes/cables/wheels anyway |
| Rank by cash outlay vs planned mods already fitted | Tight budget, mods done later; plan is Ti triangle + fork, carbon 6-7 speed wheels (new derailleur), carbon bar, carbon ring + crank |
| B ranked first | Only bike with a planned mod already on (SMC carbon bar), plus carbon post and saddle |
| J ranked 6th | S$300-800 above B/E/I/C; moves to about 3rd-4th only if the 7-speed is a real conversion |
| Table always shown with recommendation at the bottom | Asri's standing request |
| Every new shortlist entry gets a new recommendation | Asri's standing request |

## Reference (don't duplicate — just point to it)
- `C_Line_Donor_Shortlist.md` for the table, detail sections, the dated recommendation and negotiation anchors.
- `C_Line_Used_Bike_Shortlist.md` for scoring method and inspection checklist.
- `C_Line_Build_Plan.md` and `C_Line_Build_Options.md` for the 6-speed wheelset decision, Ti parts and crank/BB notes.
- `docs/handoffs/HANDOFF_foldie-build-hub-and-parts_2026-10-25.md` for the earlier hub work.

## Resume instructions
Run `git pull --ff-only`, then open `C_Line_Donor_Shortlist.md`. If Asri sends another Carousell link: open it in Claude in Chrome, add a row and detail section, re-order the table by the new ranking, rewrite the recommendation block, and show the table with the recommendation underneath. If Asri reports a seller reply, fill the Remarks column (1 Arrange for viewing, 2 Viewed, 3 Nego, 4 Reject/counter) and re-rank.
