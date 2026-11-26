# Handoff: mini velo front bag carrier mount (Brompton-style block)
**Project**: Foldie Project (this session was about the mini velo, not the T20 or G Line)
**Date**: 26 Nov 2026 (iMac session)
**App version at time of handoff**: n/a (research only)

**Status: parked.** The user could not find inserts and said "nvm". Don't restart the search unless they ask.

## Goal
A front-bag mount for the mini velo that works like the Brompton front carrier block. The frame has no mounting holes, so the mount must clamp on with screws and provide the block itself. No drilling, no straps, solid rings preferred.

## Measurements (from the user)
- Head tube diameter: 41mm.
- Top-to-bottom clearance: first 61mm, later "okay with a 91mm clearance" if one ring clamps at the top or bottom end, not the middle.
- From an angled photo (bike upside down) I estimated about 14mm / 70mm / 14mm of bare tube, split by two welded frame tubes. Estimates only; not measured.

## Done this session
- Researched clamp-on carrier blocks and custom inserts (Firecrawl and the built-in browser). Chat only; no project files changed apart from this handoff.

## Where it stands
- **Best candidate:** [TWTOPSE Birdy 2 mount](https://www.aliexpress.com/item/3256803188218009.html). Listing picture shows 41mm rings, 87mm tall, split rings tightened by screws. Needs no inserts. **Fit on this frame is not verified.**
  - Select "Birdy 2" (US$47.39 was shown with Birdy 3 selected, US pricing; Birdy 2 price not checked). Confirm the carrier block is included.
  - 4.8 from 4 reviews, 25 sold. Claims 15kg for its intended bikes, no test proof seen. I advised under 5kg including bag.
- **Inserts (51mm to 41mm):** no ready-made one found. Closest: [Ken-Lab two-piece Delrin bushing](https://www.ken-lab.com/store/p41/post-clamp-reducer-bushings.html) (US$50, custom, shown unavailable). On-Point motorcycle sleeves only go 50mm to 48/45/43mm and were unavailable. Shopee and Lazada were not searched properly.
- **If custom:** 6061 aluminium, two sleeves of two half-shells, nominal 41mm inside / 51mm outside, gaps lined up with the clamp split, sized from the real rings. Workshops listed, neither confirmed for bike parts, no price: [The Monster Builder](https://www.themonsterbuilder.com/services/cnc-machining-services-singapore/) (in-house design), [Additive Inn](https://www.additiveinn.com/services/cnc) (needs a 3D file or design service).

## Not yet done (only if the user returns to this)
1. Ask the seller each ring's height and the clear gap between rings (I guessed about 12mm per ring from the picture).
2. Cardboard 87mm template: both rings on bare tube all round, not on welds or headset cups; 41mm at both positions.
3. Cables cross where the block and bag would sit: no pinching; may need rerouting (bike shop).
4. Check bag clearance with the bike upright against tyre, brake, drop bars and levers at full turn.

## Open safety check (raised, no reply yet)
The Kids Ride Shotgun child seat mount appears, from the photo, to be clamped around a carbon tube by the stem. Advised: confirm the seat maker and fork maker allow it, and have a bike shop inspect it before carrying a child again.

## Broken / failed approaches (don't repeat)
- Options that need frame holes (MiniMODs, bare Brompton block): the user wants an adapter that brings its own holes.
- Straps (Rhinowalk): rejected. CYKE stem-faceplate mount: not a frame mount.
- Birdy 3 / folding-bike sizes (49-59mm: Mr.TiPARTS Birdy3, MEROCA, MUQZI-type) don't fit 41mm without inserts. I missed the 41mm Birdy 2 size until the user found it.
- Also seen: Mr.TiPARTS 25-42mm quick-detach (uses stainless screw bands, 5kg) and Ridea FCB5-40 (max 40mm).
- Insert searches that gave nothing suitable: exhaust adapters, motorcycle fork/headlight brackets, fork bushings, UTV and truss clamps.
- Firecrawl hit robot checks on AliExpress and Lazada (AliExpress was readable in the built-in browser); Crawl4AI refused the connection (ECONNREFUSED).

## Reference (don't duplicate — just point to it)
- Mini velo spec: `G_Line_Upgraded_Build.md` line 10.
- G Line / T20 work still open: `docs/handoffs/HANDOFF_rotors_combined_parts_451_2026-11-25.md`.

## Resume instructions
1. `git pull --ff-only` in `~/Developer/foldie-project`.
2. Default next work is the T20 / G Line list in the 25 Nov handoff.
3. Only if the user raises the bag mount again: get a straight side photo of the head tube with a ruler, plus the Birdy 2 ring heights, then check the layout before they order.
