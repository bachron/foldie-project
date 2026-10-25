# Handoff: Donor table layout, A-H relabel, Aceoffix T1 fork note
**Project**: Foldie project (C Line Black Lacquer Superlight build)
**Date**: 2026-10-25
**App version at time of handoff**: n/a (markdown repo plus one published claude.ai page)

## Goal
Make the donor shortlist table compact and readable so the Upgrades and Remarks columns get the room, relabel the builds, record the Aceoffix T1 carbon fork lead, and rank the donors by negotiation value.

## Done this session
- `C_Line_Donor_Shortlist.md` (repo, pushed): Ti parts column is bulleted one part per line (Stem, Fork, Triangle); Condition column is one word per line ("Lightly<br>used", "Like<br>new").
- Builds relabelled A-H in the same order: A=A, B=B, **D→C, E→D, G→E**, F=F, **H→G, I→H**. Headings, table rows, Quick read, route comparison, 6-speed wheelset note and "candidate H" reference all updated.
- `C_Line_Build_Options.md` (repo, pushed): new subsection "Carbon fork to explore: Aceoffix T1 (untested, dimensions unknown)" in §2 Forks, above "Fit unknowns for every aftermarket fork". Records the owner's lead (older Aceoffix fork conventional, newer one has the Mk2 / T Line look), the fit risk, and a seller checklist. Marked unverified, not ranked in the table.
- **Foldie Build page** (https://claude.ai/artifact/Jga26EY9GJLgF9oPCTejtZ, version 47): same Condition and Ti parts line breaks, A-H relabel, and the Aceoffix T1 fork note were applied to the page's own embedded copy. Donor table CSS now uses fixed layout with percentage widths: letter 3%, model 13%, ask 6.5%, condition 9%, gears 6.5%, Ti parts 8%, Upgrades 31%, Remarks 23%, minimum width 940px (scrolls sideways on narrow screens). Checked on screen in Claude in Chrome at about 1,080px wide.
- Negotiation ranking given in chat (not saved in a file): B, C, E, D, A, F, H; G (frame only) left out as a different route.

## Pending edits not yet built
- None listed.

## Not yet done
- Remarks column is still empty ("—") for every build. Owner tracks the negotiation there: 1. Arrange for viewing · 2. Viewed · 3. Nego (price offered) · 4. Reject / counter offer (price).
- Aceoffix T1 fork: ask the seller for generation, steerer, brake mount, fork length/offset, dropout width, weight, limits (checklist is in `C_Line_Build_Options.md`). No web research was done on it.
- Not checked: the page on a phone-width screen; the page's lower text sections after the relabel (only the table was viewed).
- Negotiation ranking is not written into the repo or the page. Offer figures were my estimates.

## Broken / failed approaches (don't repeat)
- The Foldie Build page is a separate static copy: the repo's markdown was pasted into its HTML at publish time, and nothing syncs it. Editing the repo does not change the page. The page's embedded text is also older than the repo in places (the owner chose to keep it that way for the Forks section).
- First width attempt (page version 43) used `width:1%` on narrow columns plus a 130px Model column with auto layout; it crushed the Model column to one letter wide. Fixed in version 44 with `table-layout:fixed`. Do not use auto layout with 1% widths there.
- A signed-out browser pane shows "Sign in to view this page" for the private artifact; viewing it needs Claude in Chrome (the owner's signed-in browser).

## Key decisions
| Decision | Rationale |
|---|---|
| Edit the page's embedded copy directly instead of building a sync script | Owner said "keep it that way" when offered a script that rebuilds the page from the repo files |
| Use percentage column widths with fixed layout | Pixel widths left Remarks taking all spare space on wide screens, so Upgrades looked smaller than Remarks |
| Keep "A-E" as the complete-bike range after relabel | After relabelling, A-E are still the five complete C Line bikes |

## Reference (don't duplicate, just point to it)
- Donor facts, scoring and inspection checklist: `C_Line_Donor_Shortlist.md`, `C_Line_Used_Bike_Shortlist.md`
- Fork options and fit unknowns: `C_Line_Build_Options.md` §2
- Aceoffix C5 / T1 bike research: `Aceoffix_C5_T1_Build_Plan.md`
- Earlier handoffs: `docs/handoffs/HANDOFF_donor-upgrades-filled_2026-10-25.md` and `HANDOFF_donor-list-upgrades_2026-10-25.md` (they use the OLD letters A, B, D, E, G, F, H, I)
- Brain Studio status was not reported this session.

## Resume instructions
1. `git pull --ff-only` in `~/Developer/foldie-project`.
2. If the owner asks for further changes to the donor table or notes, edit the repo file first, then apply the same edit to the page copy: read https://claude.ai/artifact/Jga26EY9GJLgF9oPCTejtZ, edit the saved HTML (strip the outer skeleton before `<title>`), republish to the same URL, and verify in Claude in Chrome (reload with cmd+r, open C Line, then Donor shortlist tab).
3. Next likely work: fill the Remarks column as negotiations start, and chase the Aceoffix T1 fork dimensions with the seller.
