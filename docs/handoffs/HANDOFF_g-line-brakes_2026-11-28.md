# Handoff: G Line brakes for the UltraLevers 3S
**Project:** foldie-project
**Date:** 28 Nov 2026
**Device:** iMac

## Goal
Asri has bought the Extralite UltraLevers 3S for the G Line. Pick the disc calipers, total the weight with the levers, and compare against other calipers, the current Juin hydraulic brakes and other hydraulic setups. Asri then asked for something even lighter, saying lighter 2-piston hybrids can be found, and asked about Lewis hydraulic brakes.

## Done this session
- [G_Line_Brake_Comparison.md](../../G_Line_Brake_Comparison.md) created, then updated with the lighter-hybrid search and a Lewis section. **All tables, weights, sources and "estimate" labels are in that file.** Committed and pushed.
- Tools used: Firecrawl, plus the built-in browser for one AliExpress search.

## Where it stands
- The 3S is a short-pull cable lever. It works with mechanical and cable-actuated hydraulic (hybrid) calipers, not full hydraulic ones.
- Recommendation: keep the owned **Juin R1** calipers: 284g a pair, 324g with levers, ~504g with cables and housing (cable weight is an estimate).
- No 2-piston cable hybrid lighter than ~137g each was found (web search only, not the whole market). Growtac Equal 137g and Juin GT-F 138g (4-piston) save only 8-10g a pair against the R1.
- Asri's figures, Juin F1 148g and F1-S 177g, match the file. Both are heavier than the R1.
- Lewis: every model opened is full hydraulic. On estimates a Lewis setup is ~80-114g lighter than R1 + 3S, but the 3S would go unused. The two lightest options mix R2 or BB2 SLR calipers with LV-BB levers: not sold as a set, compatibility unconfirmed. LV-BB is listed as a rear brake only.
- No proven weight saving over the current Juin hydraulic set (likely JF401, unconfirmed).
- Nothing has been chosen or ordered beyond the levers.

## Open items
1. Asri has not named the lighter 2-piston hybrid or sent a link.
2. Check on the parts: box says 3S (assumed); flat or post mount on the G Line fork, rear and the Silverrock set; mount type of the R1s.
3. The R1s are on the mini velo, which needs its flat-bar conversion before it can take the Juin hydraulic set.
4. Weigh the Juin hydraulic set when it comes off; weigh an R1 caliper if a gap of a few grams matters.
5. `T20_Build_Options.md` and `T20_Build_Plan.md` pair the long-pull UltraLevers 3 with short-pull calipers. That is wrong and has not been edited.
6. The mini velo front bag mount research is still parked: [HANDOFF_mini-velo-front-bag-mount_2026-11-26.md](HANDOFF_mini-velo-front-bag-mount_2026-11-26.md).

## Pending edits not yet built
None.

## Broken / failed approaches (don't repeat)
- Firecrawl does not support Reddit.
- The AliExpress item page showed a robot check in Firecrawl (not bypassed); the AliExpress search page in the built-in browser showed no results.
- Crawl4AI refused the connection (localhost:11235).

## Key decisions
| Decision | Rationale |
|---|---|
| Rank only cable-fed calipers for the 3S | The 3S has no master cylinder |
| Treat the Chapter 2 Cycle JF401 weights as unverified | The page contradicts itself on mount type and 82g is very low |
| Keep rotors out of every total | Same 160mm 6-bolt rotor in each setup |

## Resume instructions
Wait for Asri. If a hybrid link or model arrives, check with Firecrawl first that it is cable-fed (not hose-fed), suits short pull, which mount it uses and what its weight includes. Compare it with the R1 pair (284g), update `G_Line_Brake_Comparison.md`, commit and push. If Asri wants Lewis instead, confirm lever and caliper compatibility, brake fluid, front brake availability and hose length with Lewis or a shop before any order (Asri sends any message).
