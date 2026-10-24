# Handoff: Foldie Project rename and Black Lacquer Superlight build
**Project**: Foldie Project (repo and folder still named `t20-g-line`; Brain Studio id `t20-bike-builder`)
**Date**: 2026-10-23
**App version at time of handoff**: n/a (research docs and one artifact)

## Goal
Rename the project to Foldie Project (scope now: folding bikes in general), keep the T20 / G Line plan as it is, and add a second build: a used Brompton C Line / pre-C Line rebuilt around a Ti stem, lighter fork and Ti rear triangle. The owner then named it "Black Lacquer Superlight Build" and asked for a comparison artifact of the shortlisted used bikes.

## Done this session
- Renamed both T20 files' titles to start with "Foldie Project" (content unchanged); added `README.md` listing both builds.
- Ran six research agents and merged them into `C_Line_Build_Plan.md`, `C_Line_Build_Options.md`, `C_Line_Used_Bike_Shortlist.md`. Titles of all four C Line files carry the build name.
- Saved the owner's Carousell shortlist A-G and a Singapore live-price check in `C_Line_Donor_Shortlist.md` (no seller names or links, because the repo is public).
- Recorded the decision: **the wheelset is a 6-speed set for every candidate** (Plan, Shortlist, Options §6).
- Screenshots of listings A-D and G saved in `private/screenshots/` (git-ignored, iMac only). The screenshots for E and F were sent inline and were not saved as files.
- Built and published the artifact **Foldie Builds**: https://claude.ai/artifact/DjA9wEq9tJm4iDhSqKdDP9 (private). Source: `private/foldie-builds.html` (git-ignored, holds the ad links). Uses the `db` capability, doc `state/main`, for edits.
- Reported status to Brain Studio (id `t20-bike-builder`, status Building) and posted it to the dashboard.
- All work is committed and pushed; GitHub and the iMac are at commit cc83390.

## Pending edits not yet built
- None listed by the owner.

## Not yet done
1. The artifact's live page is untested: the built-in browser is not signed in to claude.ai. Not confirmed: that a reload restores saved edits from the db, and dark mode. Local checks (about 45) passed, apart from failures that were my own test mistakes.
2. Ask sellers the questions in `C_Line_Donor_Shortlist.md` (serial, receipt, model code, mods, weight; for F: year and warranty transfer; for G: Ti brand, stem, gearing).
3. Pin down what "6-speed" means: stock Brompton 6-speed (Sturmey Archer 3-speed hub + 2-speed derailleur, 112mm) or an external 6/7-speed freehub set. Asked in the Plan; owner has not answered.
4. Confirm the Ti rear triangle (tibicycles/COMEPLAY) rear spacing, derailleur/tensioner geometry, eyelets and pivot bore with the seller.
5. Child-seat checks: measure the Brompton stem tube against the Yepp Mini's 20-28mm range; Ti stem wall (UXN is 1.2mm) vs seat clamp; 150mm free seatpost for the Nexxt 2 Maxi.
6. Follow-up research still open: aftermarket cranks and chainring BCD, Extralite levers, brake pads, H&H / Silverock / Aceoffix product pages (none found), frame generation of each donor (Mk5 or older vs 2025+ "Advance" rear).
7. DONE 2026-10-24: repo and folders renamed to `foldie-project`. Rename "T20 Bike Builder" in Brain Studio's `studio.json` (the report script has no rename option).

## Broken / failed approaches (don't repeat)
- Carousell, eBay, Facebook Marketplace, BikeForums and WeightWeenies blocked WebSearch/WebFetch (403). **The built-in browser reads Carousell fine** (search pages and `a[href*="/p/"]` links via `javascript_tool`).
- The built-in browser renders local HTML files as static snapshots: `location.reload()` does nothing, colour-scheme emulation stays light. Navigate to the file again, or publish and test there.
- The artifact opens only for a signed-in owner; the built-in browser shows "Sign in" and must not be signed in by Claude.
- A combined `git add && commit && push` chained with the file edits was blocked once by the auto-mode classifier as an out-of-place publication (public repo). The owner approved pushes explicitly afterwards; ask before pushing new commits.
- No `node` on this iMac; JS syntax was checked in the browser instead.
- Some figures conflict between sources (stock fork 560-610g, Superlight crank 767g vs 2.29kg, Contact Urban 205-285g). The docs flag them; weigh the owner's own parts.

## Key decisions
| Decision | Rationale |
|---|---|
| Keep the T20 files, rename titles only | Owner said keep content as it is |
| Leave repo and folder named `t20-g-line` | Renaming breaks the clone paths on both Macs; owner has not asked |
| Keep ad links, screenshots and the artifact HTML out of the public repo | Repo is public; `private/` is git-ignored |
| Wheelset is a 6-speed set, stay in the Brompton 112mm system | Owner's decision; drops the custom 135mm triangle and 1x cassette route |
| Keep the steel main frame; Ti triangle, fork, stem are the headline upgrades | Ti main frame is riskier, no EN certification, weights unverified |
| Carbon seatposts excluded | Rear child seat clamps to the post |
| Web research used WebSearch/WebFetch/built-in browser only | CLAUDE.md requires asking before Crawl4AI or Browser Use; not used |

## Reference (don't duplicate, just point to it)
- Build plan, options and used-bike guide: `C_Line_Build_Plan.md`, `C_Line_Build_Options.md`, `C_Line_Used_Bike_Shortlist.md`, `C_Line_Donor_Shortlist.md`.
- T20 plan and tracker: `T20_Build_Plan.md`, `T20_Build_Options.md`; older handoffs in `docs/handoffs/`.
- Brain Studio dashboard: https://claude.ai/artifact/8P8cYkCitJKW4bcASZ3q75; report with `~/Developer/brain-studio/scripts/report-status.py --project t20-bike-builder`.
- Candidate summary (S$ asks): A 2,099 · B 2,000 · C 3,883 (Superlight, Ti fork+triangle already) · D 2,200 (serviced Aug 2026, best paper trail) · E 2,400 (unsold 3+ months) · F 1,299 (frame only) · G 2,800 (custom, Ti fork+triangle, 3-speed, 54T ring).

## Resume instructions
1. Start with `git pull --ff-only`; this handoff is the newest file in `docs/handoffs/`.
2. Ask the owner (a) which "6-speed" they mean and (b) for any seller replies, then update `C_Line_Donor_Shortlist.md` and the artifact's candidate data (edit `private/foldie-builds.html`, republish with the same file path and `capabilities: {"db": {}}`).
3. Ask the owner to open the artifact link signed in and confirm: edits survive a reload, dark mode reads well, links open the right ads.
4. Do not push new commits without asking.
