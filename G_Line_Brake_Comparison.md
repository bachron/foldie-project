# G Line brakes: UltraLevers 3S setup vs Juin hydraulic

**Date:** 26 Nov 2026. **Bought:** Extralite UltraLevers 3S (levers). **Tools:** Firecrawl.
Weights exclude rotors (160mm 6-bolt in every case).

## Levers
UltraLevers 3S: 40g on [Extralite's page](https://www.extralite.com/products/901) (read as the pair; earlier repo note 41g). The [manual](https://admin-new.extralite.com/docs/docs_68247addcad1b.pdf) says caliper and cantilever brakes (short pull). They have no master cylinder, so they cannot drive a full hydraulic caliper.

## Cable setups with the 3S (short pull, flat mount)
Lines = cables + housing, **my estimate ~180g (150-220g)**. Caliper figures mix maker claims and weigh-ins.

| Caliper | Type | Each (g) | Pair (g) | + levers (g) | + lines, est. (g) | Source |
|---|---|---|---|---|---|---|
| Growtac Equal | Mechanical | 137 | 274 | 314 | ~494 | [Bikerumor, with pads](https://bikerumor.com/paul-klamper-mechanical-disc-brake-review-comparison-growtac-equal/) |
| Juin GT-F | Cable-hydraulic, 4-piston | 138 | 276 | 316 | ~496 | [Juin US](https://juintechus.com/product/juin-tech-gt-f-B09PV8FQN346) |
| **Juin R1 (owned, on mini velo)** | Cable-hydraulic | 142 | 284 | 324 | ~504 | [BikeRadar weigh-in](https://www.bikeradar.com/news/juin-techs-r1-disc-brakes-promise-cheap-yet-powerful-stopping) |
| Yokozuna Motoko | not checked | 142 | 284 | 324 | ~504 | [Yokozuna, with pads](https://www.yokozunausa.com/shop/yokozuna-motoko-road-disc-brake-flat-mount-2500) |
| TRP Spyre SLC | Mechanical | 146 | 292 | 332 | ~512 | [Competitive Cyclist](https://www.competitivecyclist.com/trp-spyre-slc-mechanical-flat-mount-disc-brake-caliper) |
| TRP Spyre | Mechanical | 154 | 308 | 348 | ~528 | repo / Bikerumor-era figure |
| TRP HY/RD | Cable-hydraulic | 195 | 390 | 430 | ~610 | claimed, quoted by BikeRadar |
| Paul Klamper (short pull) | Mechanical | 211 | 422 | 462 | ~642 | Bikerumor, with pads |

**Pick:** Juin R1 (already owned; the best buy-new option saves only ~10g). If buying new: GT-F.

## Current Juin hydraulic (likely JF401, model unconfirmed)
- [Chapter 2 Cycle](https://www.chapter2cycle.sg/products/juin-jf401-brake-setflat-mount-black) lists caliper 82g, lever 98g. The page says "post mount" in places and flat mount in others, and 82g is very low for a 4-piston caliper. **Treat as unverified.** Face value: 360g a pair + hoses/fluid ~90g (est.) = ~450g.
- Repo estimate: 450-600g (the bike's estimates ran about 17% high).
- So the R1 + 3S setup (~504g est.) shows **no proven weight saving**. Weigh the Juin set when removed.

## Other full hydraulic sets (own levers; 3S not used)
| Set | Pair (g) | With 2 post adapters, ~+32g | Note |
|---|---|---|---|
| Trickstuff Piccola Carbon | 341 | ~373 | [BikeRadar](https://www.bikeradar.com/features/trickstuff-piccola-first-look); about EUR 1,100; mount assumed post |
| Magura MT8 SL | 390-452 | ~422-484 | [Magura](https://magura.com/product/mt8-sl/) 195g per brake, post mount; BikeRadar quotes 452g |
| Shimano XTR M9100 | ~316-404 | ~348-436 | sources disagree ([retailer 158g a side](https://www.performancebike.com/shimano-xtr-m9100-hydraulic-disc-brake-set-grey-post-mount-right-im9100jrrxma170/p1563418), BikeRadar 404g) |
| Juin JF401 (current) | ~450 (see above) | no adapter (flat mount) | [Juin](https://www.juintechofficial.com/jf401-1) lists it for the G Line; no weight given |
| SRAM Level Ultimate | 532 | ~564 | BikeRadar figure, older model |
| Shimano XT M8100 | 573 | ~605 | repo figure (279g F + 294g R) |

What each published hydraulic weight includes (hose length, bolts) is mostly not stated.

## Check before fitting
- Box says **3S**. The plain UltraLevers 3 is for V-brakes (long pull).
- Flat or post mount on the G Line's current fork and rear, and on the Silverrock set.
- R1 mount type; the mini velo needs its flat-bar conversion before it can take the Juin hydraulic set.
- `T20_Build_Options.md` and `T20_Build_Plan.md` pair the long-pull UltraLevers 3 with short-pull calipers: that pairing is wrong (not edited here).
