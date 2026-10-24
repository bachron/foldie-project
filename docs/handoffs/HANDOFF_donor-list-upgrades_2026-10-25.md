# Handoff: Donor list edits and the Upgrades column
**Project**: Foldie Project (C Line black lacquer Superlight build)
**Date**: 2026-10-25
**App version at time of handoff**: n/a (markdown plus the private Foldie Build hub)

## Goal
Make the donor shortlist in `C_Line_Donor_Shortlist.md` usable for buying: clickable listing titles, new listings, a negotiation Remarks column, and an Upgrades column.

## Done this session
- Every donor title (table cell and section heading) links to its Carousell listing. Links live in the markdown itself (the repo is public, which Asri accepts).
- Added builds from listing links and screenshots. Letters are now: A, B, D, E, G, F, H, I (**C was removed**; letters were swapped around, so go by the table, not old notes).
  - A: C Line Explore S6R Black Edition, S$2,099
  - B: C Line black lacquer "dark bronze", S$2,000, treated as 6-speed
  - D: C Line Explore M6L, S$2,200
  - E: C Line M6L special Black Edition, S$2,400
  - G: 2021 M6L C Line Explore Black Edition with H&H parts, S$1,700
  - F: custom build with Ti22 fork and triangle, 3-speed, S$2,800
  - H: main frame only, S$1,299
  - I: Superlight S6L-X Black Edition, S$3,883, third-party titanium stem
- Table columns are now: Model (as listed), Ask (S$, price only), Condition, Gears (short), Already has Ti parts? (only "No" or fork / triangle / stem), Upgrades, Remarks.
- Remarks column tracks negotiation: 1 Arrange for viewing, 2 Viewed, 3 Nego (price), 4 Reject / counter offer (price). All rows are "—" so far.
- Added a Digirit carbon chainring row to the T20 chainring table in `T20_Build_Options.md` (130 BCD does not fit the 110 spider; no 110 version confirmed).
- Every change was pushed and the published Foldie Build page was republished (version 32).

## Pending edits not yet built
- None.

## Not yet done
1. **Fill the Upgrades column using Claude in Chrome** (Asri's request for the next session). Open each Carousell listing in Asri's own Chrome and list every upgraded part as simple bullets (`• part<br>• part` inside the table cell). Write **None** where there are no upgrades.
   - Still `TBD`: A, B.
   - Partial, from notes: D (44T chainring only), E (wheels and grips, details not given).
   - Filled from screenshots, to verify against the listing: F, G, I. H is `None`.
2. Remarks column: update as Asri reports viewings and offers.
3. Ask Asri to confirm anything that looks ambiguous in a listing, then edit the markdown only, never invent parts.

## Broken / failed approaches (don't repeat)
- **Carousell blocks every browser tool I had** (built-in browser, DevTools Chrome, Playwright, Firecrawl) with a Cloudflare check. Ticking the box did not help. Do not try to get around it.
- **Claude in Chrome tools did not exist in the session.** The extension is installed and signed in (native-messaging files exist). I set `claudeInChromeDefaultEnabled: true` in `~/.claude.json` (backup at `~/.claude.json.bak-chrome`), which should take effect in a new session. **Untested.** Start the session, search for tools named `mcp__claude-in-chrome__*`; if none appear, tell Asri and fall back to asking Asri to paste listing text or screenshots (they have worked well).
- The built-in browser pane could not open `file://` URLs; serving over a local `python3 -m http.server` worked.
- `sed -i` fails on macOS without a backup suffix; use Python for edits.

## Key decisions
| Decision | Rationale |
|---|---|
| Links go in the public markdown, not a private file | Asri said the links can stay public, and the published page reads the markdown |
| Swapping letters swaps whole rows and sections; positions stay fixed | Asri asked for swaps, not reordering. Moving a build to a new place is a different request |
| Ti column shows only "No" or fork / triangle / stem | Asri's request |
| Ask column shows only the price | Asri's request |

## Reference (don't duplicate — just point to it)
- Build hub: `private/build_hub.py` + `private/hub_template.html` produce `private/foldie-build.html` (gitignored folder). Rebuild with `python3 private/build_hub.py`.
- Published page (private artifact): https://claude.ai/artifact/Jga26EY9GJLgF9oPCTejtZ. Republish with the Artifact tool using that URL and `private/foldie-build.html`; capabilities carry over. Asri views it in Safari and must reload.
- Scoring method and buy/pass rules: `C_Line_Used_Bike_Shortlist.md`. Plan: `C_Line_Build_Plan.md`.
- Earlier handoffs in `docs/handoffs/`.

## Resume instructions
1. `git pull --ff-only`, confirm the device (`sysctl -n hw.model`), and note that `private/` is gitignored, so the hub files only exist on the Mac where they were built (this session: `Mac16,12`, taken to be the MacBook Air; check the iMac has `private/` before rebuilding there).
2. Check whether Claude in Chrome tools are available. If yes, open each listing from the table links (A, B, D, E, G, F, I) and fill the Upgrades cells. If no, say so and ask Asri to paste each listing's description.
3. Edit `C_Line_Donor_Shortlist.md`, run `python3 private/build_hub.py`, commit, push, republish the artifact, and say what changed.
