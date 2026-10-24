# Handoff: Foldie Build hub, parts research and Aceoffix plan
**Project**: Foldie Project (repo `bachron/foldie-project`, Brain Studio id `t20-bike-builder`)
**Date**: 2026-10-25
**App version at time of handoff**: n/a (docs plus one private artifact, now at version 7)

## Goal
Rename the project (done 24 Oct), research C Line parts at depth (weight and S$ price for every row), add a third build (Aceoffix C5 / T1), and turn the artifact into a build hub: pick or create a build, then open its plan, research and parts.

## Done this session
- Renamed repo and both Mac folders to `foldie-project`; README, Brain Studio entry and dev-migration cheatsheet updated (24 Oct).
- C Line decisions recorded in `C_Line_Build_Plan.md`: own external 7-speed drivetrain (no Brompton hub), 7 gears fine, Neutron B7 cassette chosen (7-speed 11-30T, 122 g, Shimano HG), Jagwire confirmed for brake housing (kit not chosen), SMC CW1FR front wheel + rear rim leaning (rear laced on an HG hub), Singapore dealer quotes (Comeplay fork+triangle S$600 raw / S$700 black, stem+fork+triangle S$1,250, SMC Plume 4-speed S$1,090).
- `C_Line_Build_Options.md` sections 7, 7a, 7b, 7c: wheelset shortlist, SMC and Light Bicycle details, Neutron cassette, SMC CW1FR-25.
- Parts research, two rounds plus add-ons, all merged: `C_Line_Parts_List.md` (compact) and `C_Line_Parts_Research.md` (full detail with links). 1,984 rows, about 880 with an estimated weight or price (`est.`, basis shown). Covers frame, wheels/hubs, cranks/BBs, chainrings, shifting, brakes/cables, cockpit, Bjorn Cycles (Slovenian carbon maker, only the Sedlo saddle is useful), BBInfinite and other T20-plan brands, Brombacher (Korean shop), Gemini Carbon and Sixweel (neither makes folder parts; rows kept because asked).
- New build plan `Aceoffix_C5_T1_Build_Plan.md` (C5 and "T1" look like the same bike; 7.5 kg claimed, 8.15 kg measured; S$1,360-1,640; 118 mm rear spacing). README lists three builds.
- T20 / G Line: only added the Neutron 11-speed (MK2) cassette as one row in `T20_Build_Options.md` (T20 decisions are on hold at the owner's request).
- Artifact **Foldie Build** (https://claude.ai/artifact/Jga26EY9GJLgF9oPCTejtZ, private, version 7, capabilities `db` and `user`): home = small square cards (bike cutout, name, status) for G Line / T20, C Line, Aceoffix C5 / T1 and "+ New build". Build pages have Overview, document tabs (rendered markdown with a jump menu), and a Parts book (sortable brand tables, row details under the table, back buttons). Custom builds are saved in the artifact database (`builds/{id}` with `parts` sub-collection). Parts book is shared by all three builds with a fit-check note on T20 and Aceoffix.
- Dock shortcut "Foldie Build" (folding-bike rider icon, white on black) on the MacBook Air and the iMac, app at `~/Applications/Foldie Build.app` opens the artifact link.

## Pending edits not yet built
- None listed by the owner.

## Not yet done
1. Click through the published artifact once signed in: create a custom build, add and remove a part, open each tab, check the card layout and bike cutouts. I could not sign in, so only the home render and script syntax were checked; the `builds` collection is empty.
2. Ask sellers / Chris Yeo: SMC CW1FR rear-rim build on an HG 112 mm hub and price; whether Plume (100-110 kg, ratchet hub) takes an HG cassette; Comeplay fork/triangle spacing and hanger; Aceoffix seller questions (118 mm spacing, stem tube, parts list).
3. Choose the Jagwire kit, a short-pull lever (Extralite UltraLevers 3S) and a caliper whose reach covers Brompton's 54-68 mm drop.
4. About 880 estimated cells in the parts list: confirm the ones that matter (thx4ride items, Brompton-specific derailleur sets) with sellers.
5. Owner asked for T20 additions to the parts list only; no T20 planning.
6. iMac Dock shortcut was added over SSH but not seen on the iMac screen.

## Broken / failed approaches (don't repeat)
- Carousell, Marketplace, Shopee, Lazada, eBay and several shops block fetch tools or show a bot check; do not bypass it. Marketplace prices are snippets or estimates.
- A research agent opened YouTube in the built-in browser and it played with sound. Never open video pages in the browser pane; use page text and search snippets.
- AppleScript `osacompile` apps keep the default scroll icon in the Dock; use a plain app bundle with `CFBundleIconFile` plus an `.icns`. The Dock also kept the old path after a rename, so remove the Dock entry and add a fresh one.
- The built-in browser could not open the local `private/foldie-build.html` (earlier file previews worked); check the script with JavaScriptCore instead: `osascript -l JavaScript` with `new Function(src)`.
- The product-name inconsistencies: "Bombracher" = Brombacher (Korean shop), "Eilileee" = Elilee, "Lunatee" = SMC Lunate.

## Key decisions
| Decision | Rationale |
|---|---|
| T20 and G Line are one build ("G Line / T20") | Repo already treated them as one; owner can split |
| Own external 7-speed HG drivetrain, no Brompton hub | Owner's choice; Neutron B7 needs a Shimano HG freehub, which favours Light Bicycle or a custom HG rear |
| 7 gears is fine (6-speed decision relaxed) | Owner confirmed 25 Oct |
| T20 on hold, parts list only | Owner wants to build the C Line |
| Parts book shared by all builds | Owner asked for Brombacher and Gemini/Sixweel parts in every build; fit notes carry the differences |
| Gemini Carbon and Sixwheels kept despite no folder products | Owner asked; flagged in the data and background notes |
| Artifact source kept in `private/` (git-ignored) | Repo is public and the page embeds prices and marketplace links |

## Reference (don't duplicate, just point to it)
- Plans: `C_Line_Build_Plan.md`, `T20_Build_Plan.md`, `Aceoffix_C5_T1_Build_Plan.md`; options: `C_Line_Build_Options.md`, `T20_Build_Options.md`.
- Parts: `C_Line_Parts_List.md`, `C_Line_Parts_Research.md`.
- Artifact source (not in git, copied to both Macs): `private/hub_template.html` (page code), `private/build_hub.py` (assembles the page from the repo markdown, `private/parts_merged.json` and `private/bike_images.json`), output `private/foldie-build.html`. To update: edit the template or data, run `python3 private/build_hub.py`, publish `private/foldie-build.html` with `capabilities: {"db":{},"user":{}}` to the same artifact URL.
- Brain Studio: `~/Developer/brain-studio/scripts/report-status.py --project t20-bike-builder`.

## Resume instructions
1. `git pull --ff-only` in `~/Developer/foldie-project`; this handoff is the newest file in `docs/handoffs/`.
2. Ask the owner to open the Foldie Build page (Dock shortcut) and say what looks wrong in the cards, tabs or Parts book; fix in `private/hub_template.html` and republish.
3. When the owner gets Chris Yeo's SMC price or seller answers, update `C_Line_Build_Plan.md`, the picks in `private/build_hub.py` and republish.
4. Do not start T20 decisions; only add parts to the T20 list when asked. Ask before pushing new commits only if the owner has said so; otherwise commit and push at the end per the global rule.
