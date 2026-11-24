# Handoff: G Line drivetrain confirmed, shifter logged, tool kit shortlist
**Project**: foldie-project (G Line / mini velo / T20)
**Date**: 2026-11-24
**App version at time of handoff**: n/a

## Goal
Answer whether the mini velo's freehub can move to the G Line (Shimano HG vs SRAM XDR), then log
confirmed G Line parts and shortlist a one-set bike tool kit.

## Done this session
- Explained that the freehub body (HG vs XDR) decides cassette fit, while the derailleur and shifter
  only have to match each other. Oleg (Twisted Wheels) running XDR + Neutron cassette + Red AXS needs no
  Shimano derailleur. Shimano and SRAM 12-speed cog spacing differ, so an HG cassette would not index
  properly on the Force AXS derailleur.
- Corrected my own error: I cited the T20's Nuton 11-50T and XT M8100 as the mini velo's. The mini velo
  is Ultegra R8000 11-speed, 11-32 HG, rear QR (~130mm assumed) per `G_Line_Upgraded_Build.md:10`.
- Owner physically checked the G Line: cassette is SRAM Force, rear derailleur is SRAM Force AXS.
  Logged in `G_Line_Current_Parts_List.md` rows 15 and 18 (commit pushed).
- Owner uses the AXS Rocker Paddle. Logged in row 16 (commit pushed). Weight and battery not found.
- Compared Rocker Paddle vs Pod Ultimate from reviews and forums: same shifting, differs in feel.
  Pod Ultimate listed at ~50 g (Vital MTB); rocker weight not found. Recommended keeping the rocker.
- Researched one-set tool kits (BikeRadar, Cyclist, Cycling News): recommended PRO Advanced Toolbox
  plus a separate torque wrench.
- Claude in Chrome setup: extension installed, `claudeInChromeDefaultEnabled` already true, Chrome
  launched, but the extension still reports no connected browsers (likely signed out).

## Pending edits not yet built
- None.

## Not yet done
- Price the PRO Advanced Toolbox and Park Tool SK-4 from Singapore and overseas sellers (incl. shipping
  and import tax); owner offered no go-ahead yet.
- Choose a torque wrench (Cycling News guide lists options).
- Verify the kit's cassette tool fits the XDR lockring (only "12-speed compatible" confirmed).
- Look up AXS Rocker Paddle weight; confirm shifter battery.
- Owner to sign in to the Claude in Chrome extension, then retry connection.
- Confirm the SMC hub's actual freehub body (read off the hub or ask SMC); XDR only inferred from
  the listing and cassette.

## Broken / failed approaches (don't repeat)
- Claude in Chrome: `tabs_context_mcp` and `list_connected_browsers` return not connected even with
  Chrome open. Needs the owner to sign in; do not retry blindly.
- Do not cite T20 parts (Nuton cassette, XT M8100) as the mini velo's.

## Key decisions
| Decision | Rationale |
|---|---|
| Keep G Line on XDR + SRAM Force AXS, buy a Neutron/XDR cassette if swapping | Matched SRAM 12-speed system; HG cassette would mis-index |
| Keep the AXS Rocker Paddle | Same shifting as Pod Ultimate; reviewers prefer the rocker feel; no confirmed weight gain from switching |
| One-set tool kit: PRO Advanced Toolbox + separate torque wrench | 12-speed compatible tools, right Torx sizes, cheaper than 36-37 tool kits; torque wrench matters for carbon and titanium |

## Reference (don't duplicate, just point to it)
- `G_Line_Current_Parts_List.md` for the current G Line parts and weights.
- `G_Line_Upgraded_Build.md` for the owned bikes (mini velo, P Line, T20) and the brake swap plan.
- `T20_Build_Plan.md` for the T20 only (HG freehub, Nuton cassette, XT M8100).
- Previous handoff: `HANDOFF_g-line-seatpost-gearing-weight_2026-11-22.md`.

## Resume instructions
1. `git pull --ff-only`, then ask the owner whether to price the tool kits (PRO Advanced Toolbox vs
   Park Tool SK-4) from Singapore and overseas sellers; show a table with a recommendation under it.
2. Check whether the owner has signed in to the Claude in Chrome extension; retry
   `tabs_context_mcp`.
3. Optional: find the Rocker Paddle weight and log it in row 16.
