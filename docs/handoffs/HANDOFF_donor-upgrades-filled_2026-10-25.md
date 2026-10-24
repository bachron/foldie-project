# Handoff: Upgrades column filled for A, B, D, E; donor table layout
**Project**: Foldie Project (C Line black lacquer Superlight build)
**Date**: 2026-10-25
**App version at time of handoff**: n/a (markdown plus the private Foldie Build hub, published as version 41)

## Goal
Follow up `HANDOFF_donor-list-upgrades_2026-10-25.md`: fill the Upgrades column in `C_Line_Donor_Shortlist.md` for builds A, B, D and E from the Carousell listings, then tidy the table width.

## Done this session
- Claude in Chrome tools worked this time (`mcp__claude-in-chrome__*`). Carousell's security check cleared by itself after about 6 seconds of waiting; nothing was bypassed. The page text from `get_page_text` already contains the full description (clicking "Read more" added nothing).
- Upgrades filled, all pushed:
  - **A**: None (PPF wrap, rack and mudguards are standard or protective; saddle is going back to the factory original).
  - **B**: H&H carbon seatpost, Brooks Cambium C13 carbon saddle, Ti Parts Workshop Double X pedals, SMC carbon handlebar M40. **The seller lists none of these; they are Asri's reading of the photos.** B's section says to confirm with the seller.
  - **D**: 44T chainring only (original ring included).
  - **E**: upgraded wheels, upgraded grips (listing gives no brands).
- **B is a 6-speed with stock internal gearing**, confirmed by Asri. "(assumed)" and the old photo-doubt note were removed; the wheelset note now lists A, B, D, E as 6-speed.
- Table layout: **Gears** column shortened to `6`, `3`, `2/3 (mod)`, `—`. **Ti** header is now "Ti parts". **Model (as listed)** keeps the original listing names (restored from commit `992e3bf`).
- Narrower Model column done in the hub only: `private/hub_template.html` adds class `donors` to the donor table (second header starts with "Model") and sets that column to 150px with wrapping. Rebuilt with `python3 private/build_hub.py` and republished (version 41).
- Memory saved: `feedback_column-width-and-direct-answers.md`.

## Pending edits not yet built
- None.

## Not yet done
1. **Check the published page in Safari** (reload). The 150px Model column was never looked at in a browser: confirm the names wrap cleanly and Upgrades got the room. If wrong, adjust only the width rule in `private/hub_template.html`, rebuild, republish.
2. Verify F, G and I Upgrades against their listings (still "from screenshots"; not asked this session).
3. Confirm B's four parts with the seller. Ti pedals on B do not change the Ti parts column (it counts fork, triangle, stem only).
4. Remarks column: update as Asri reports viewings and offers (all "—").

## Broken / failed approaches (don't repeat)
- **I rewrote the listing names** when told to "reduce the model name column". "Reduce/shorten a column" means **width**, never wording. Never edit listing names unless Asri says to.
- I read B's photos wrongly (called the rear hub-only and possibly 2/3-speed). Asri corrected it. Do not write photo guesses into the repo as fact; label them or ask.
- A mid-turn question from Asri ("are you hallucinating?") was not answered first. Answer questions before any more tool calls.
- Publishing the artifact is refused until the live version has been read once; Read the first lines of the saved copy, then publish again. The saved copy only differs by the publish wrapper.

## Key decisions
| Decision | Rationale |
|---|---|
| Model column keeps the original listing names | Asri wants to see the listing name as posted |
| Narrow Model column is done in the hub CSS, not in the markdown | Words must stay unchanged; only width changes |
| Gears shown as just the number | Asri asked to reduce the Gears column |
| B's parts recorded from Asri's photo reading | Seller lists none; flagged as unconfirmed |

## Reference (don't duplicate — just point to it)
- Previous handoff: `docs/handoffs/HANDOFF_donor-list-upgrades_2026-10-25.md` (setup, hub build, republish steps).
- Build hub: `private/build_hub.py` + `private/hub_template.html` produce `private/foldie-build.html` (gitignored; exists on the Mac where it was built, this session `Mac16,12`).
- Published page (private artifact): https://claude.ai/artifact/Jga26EY9GJLgF9oPCTejtZ

## Resume instructions
1. `git pull --ff-only`; confirm device with `sysctl -n hw.model`.
2. Ask Asri whether the Model column width looks right on the published page; fix width only if not.
3. If asked, verify F, G, I upgrades with Claude in Chrome (wait about 6 seconds for the Carousell check; use `get_page_text`), edit `C_Line_Donor_Shortlist.md`, run `python3 private/build_hub.py`, commit, push, republish the artifact.
