# Handoff: T20 chosen parts on the Foldie Build page
**Project**: Foldie Project (repo `bachron/foldie-project`, Brain Studio id `t20-bike-builder`)
**Date**: 2026-10-25
**App version at time of handoff**: n/a (artifact Foldie Build, version 33)

## Goal
Owner asked why the G Line / T20 build on the Foldie Build page did not show the parts planned earlier, then asked to fill them in and republish.

## Done this session
- Cause found: the T20 "Chosen and confirmed" list is hand-typed in `picks` inside `private/build_hub.py`, not read from `T20_Build_Plan.md`. It held only the Nuton cassette. The plan and options files were already on the page's tabs; the T20 Parts book is the C Line catalogue with a fit warning, so it was never a T20 list.
- `private/build_hub.py`: T20 `picks` now has 19 rows taken from `T20_Build_Plan.md`. Confirmed: frame and rear triangle, Ti stem, tyres, grips, child seats, dropout hanger. Chosen: fork, crankset, spider, chainring, cassette, seatpost, carbon bar. Leaning: bottom bracket, 11/12-speed, flat-mount brakes, UltraLevers 3S, SMC Plume wheelset, pedals.
- Rebuilt `private/foldie-build.html` and republished to https://claude.ai/artifact/Jga26EY9GJLgF9oPCTejtZ (version 33). Compared with the live version first: only the builds data line differed.
- Copied the new `private/build_hub.py` to the iMac over SSH and checked it there. The rebuilt `foldie-build.html` was not copied.

## Pending edits not yet built
- None listed by the owner.

## Not yet done
1. Open the published page and look at the T20 Overview list (not viewed after publishing).
2. Items from `HANDOFF_foldie-build-hub-and-parts_2026-10-25.md` still stand (click-through test, seller questions, Jagwire kit and lever choice, estimated cells).

## Broken / failed approaches (don't repeat)
- Publishing to the artifact is refused until the live version has been read; the refusal saves it to a file. Compare against it (the live file has one extra wrapper line at the top), `Read` a few lines of it, then publish again.

## Key decisions
| Decision | Rationale |
|---|---|
| Bar shown as "Chosen" with the model open | Plan says carbon is decided and not to be reopened; the model is not decided |
| UltraLevers 3S, wheelset, BB, pedals, brakes marked "Leaning" | Plan still lists them as open or preferred |
| T20 status stays "On hold (parts list only)" | Owner has not restarted T20 decisions |

## Reference (don't duplicate, just point to it)
- Source of the picks: `T20_Build_Plan.md`. Hub assembly: `private/build_hub.py`, `private/hub_template.html` (git-ignored; copied by hand to both Macs).
- Earlier hub handoff: `docs/handoffs/HANDOFF_foldie-build-hub-and-parts_2026-10-25.md`.

## Resume instructions
1. `git pull --ff-only` in `~/Developer/foldie-project`.
2. If the T20 plan changes, edit the `picks` list for `"id":"t20"` in `private/build_hub.py`, run `python3 private/build_hub.py`, publish `private/foldie-build.html` to the same artifact URL (read the live version first), and copy `build_hub.py` to the other Mac.
