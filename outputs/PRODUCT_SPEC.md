# PRODUCT SPEC — Women's Short Wool Jacket

**Status:** Ground Truth indexed; specification baseline established  
**Ground Truth source:** `01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png`  
**Evidence rule:** The supplied sheet is the sole product-visual authority. Text labels are recorded as supplied; visible image evidence is used to verify construction. Any contradiction or non-visible fact is marked `UNCERTAIN`.

## LOCKED FEATURES

These attributes must remain unchanged in every generated or retouched product image.

| Feature | Locked specification | Evidence / confidence |
|---|---|---|
| Product category | Women's jacket | Product info; HIGH |
| Style / length | Short wool jacket; hem visually ends around upper-hip on the model reference | Product info + multi-view images; HIGH for short length, exact measurement unavailable |
| Main color | Cream / ivory, warm off-white appearance | Product info + color swatch + all views; HIGH for color family; no numeric color value supplied |
| Shell surface | Soft, visibly textured wool-blend surface; fine irregular/nubby texture, not smooth or glossy | Fabric close-up + garment views; HIGH |
| Material declaration | Wool blend: 70% wool, 30% polyamide | Product info; HIGH as supplied metadata, not visually testable |
| Lining | Smooth, light cream lining; declared 100% viscose | Lining close-up + product info; HIGH as supplied metadata |
| Silhouette / fit | Regular fit with lightly shaped waist; structured tailored shoulder; straight long sleeves | Front/back/model views; HIGH |
| Front construction | Single-breasted front with classic notch lapel and deep V opening | Front/detail/model views; HIGH |
| Collar | Classic notch lapel; moderate-width lapel with clean edge stitching | Product info + detail; HIGH |
| Front closure | **Exactly 3** brown/tortoiseshell-look round four-hole buttons arranged vertically | Button detail + clearest isolated front view + latest user decision; HIGH. Count revised and locked by user on 2026-09-20 |
| Front pockets | Two symmetrical waist-level flap pockets, one on each side; horizontal rectangular flaps with softly rounded lower corners | Product info + front/detail views; HIGH |
| Back | Clean center-back seam and one center vent at hem | Back view + vent detail; HIGH |
| Sleeve | Full-length set-in sleeves; one small matching four-hole button at each cuff; clean cuff finish without visible slit in supplied view | Side/detail images; HIGH for visible construction |
| Hem | Short, gently curved front hem; rear hem divided only by center vent | Front/back views; HIGH |
| Stitching | Fine, even, tone-on-tone stitching | Stitching detail; HIGH |
| Hardware/trim palette | Buttons are warm brown translucent/marbled tortoiseshell-look; no metal hardware is visible | Detail + garment views; HIGH |
| Prohibited additions | No extra pockets, buttons, belts, epaulettes, piping, embroidery, vents, trims, logos, or decorative seams | Entire reference sheet; HIGH within visible areas |

## VARIABLE FEATURES

These may vary only when the locked product structure remains intact.

| Feature | Allowed variation | Constraint |
|---|---|---|
| Model | Identity, hair, makeup, pose, and body proportions may vary | Garment fit must remain plausible; jacket silhouette and length may not be redesigned |
| Styling | Coordinating inner top, trousers/skirt, shoes, and accessories | Must not cover critical product features needed for QC; avoid color cast onto jacket |
| Jacket state | Open, naturally closed, or partially obscured by a physically plausible pose | Do not invent closure details; hidden details must not be reconstructed speculatively |
| Camera framing | Full body, three-quarter, mid shot, detail, front/back/side/oblique view | Perspective must not distort lapel, length, pocket position, or proportions |
| Pose / drape | Natural arm and torso poses with realistic fabric response | Preserve tailoring; no implausible stretch, warping, or asymmetry |
| Background | Neutral studio or restrained lifestyle/editorial setting | Background must not contaminate the cream/ivory color or conceal silhouette |
| Lighting | Soft natural/studio light; direction and intensity may vary | Maintain true cream/ivory appearance and readable wool texture; no clipping or heavy tint |
| Crop / output size | May vary by channel | Preserve adequate product visibility; do not crop away required QC landmarks |
| Retouching | Dust/temporary wrinkle cleanup, tonal balancing, edge cleanup | No texture erasure, reshaping, seam relocation, or false symmetry |

## UNKNOWN FEATURES

Every item below is `UNCERTAIN` and must not be invented. If visible in a future output, it requires new verified source material or deliberate concealment.

| Unknown / conflict | Why uncertain | Required handling |
|---|---|---|
| Front closure source discrepancy — RESOLVED | Product Info states 4 buttons while the clearest isolated product view visibly resolves 3. | **Final user decision on 2026-09-20: lock exactly 3 front buttons.** This supersedes the earlier temporary 4-button decision and governs all generated views. |
| Exact garment measurements | No shoulder, bust, waist, sleeve, back length, lapel width, pocket, or vent measurements are supplied | Preserve reference proportions visually; never state numeric measurements |
| Exact color value | No Pantone, LAB, RGB, HEX, or calibrated color target is supplied; display/lighting may shift appearance | Use the supplied swatch and garment views as visual reference; no invented numeric code |
| Exact fabric weave, weight, pile, and handfeel | Only composition and a visual close-up are supplied | Describe only as soft/textured wool blend; do not claim weave or GSM |
| Internal construction | Interfacing, shoulder pads, seam allowances, interior pockets, full lining pattern, and underside details are not shown | Keep hidden or mark `UNCERTAIN` |
| Pocket internals | Pocket depth, bag construction, and whether the flaps cover functional pockets are not directly demonstrated | Preserve visible flap structure only; do not show interiors without evidence |
| Cuff construction beyond visible face | A single cuff button is visible, but opening/placket and underside are not fully shown | Preserve the visible clean cuff and one button; avoid exposed underside |
| Button material | Caption says “Tortoiseshell,” but actual material (resin, horn, shell, etc.) is not established | Refer to appearance as tortoiseshell-look; do not claim material |
| Brand identity | Label reads “AURÉL,” but caption explicitly says “Brand Label (Example)” | Do not treat brand name as confirmed; remove/obscure in outputs unless user confirms use |
| Size | A small “S” tag appears only in the example label close-up | Do not claim the product size is S without confirmation |
| Season and target positioning | “Fall / Winter” and “Modern Minimal” appear as supplied merchandising metadata | May guide art direction, but they do not establish construction facts |
| True left/right hidden details | Some oblique views do not expose every seam and cuff face | Mirror only clearly symmetric confirmed features; otherwise keep hidden/mark `UNCERTAIN` |

## QC CHECKLIST

### A. Intake / source control

- [ ] Use only the archived Ground Truth file as the product-visual reference.
- [ ] Confirm the image is not color-profile-shifted, stretched, mirrored, or cropped before comparison.
- [x] Front-button conflict resolved by latest user instruction: exactly 3 front buttons are locked.
- [ ] Record every unresolved detail as `UNCERTAIN`; never complete it from model convention or prompt inference.

### B. Product identity — hard-fail checks

- [ ] Main color remains cream/ivory with no beige, yellow, gray, pink, or green cast.
- [ ] Jacket remains short and regular-fit with the same visual length and overall proportions.
- [ ] Classic notch lapel shape, width, break point, and V opening remain consistent.
- [ ] Front closure uses the confirmed button count after resolution; spacing and vertical placement match reference.
- [ ] Buttons remain round, four-hole, warm brown tortoiseshell-look; no metallic or fabric-covered substitutions.
- [ ] Exactly two waist-level flap pockets remain, with matching placement, scale, and flap geometry.
- [ ] Back center seam and single center vent remain present and correctly aligned.
- [ ] Sleeves remain full length with clean cuffs and one matching visible cuff button per side when exposed.
- [ ] No unsupported seams, darts, pockets, vents, fasteners, trims, logos, or decorative details appear.

### C. Material realism

- [ ] Wool-blend texture remains visible at the intended viewing scale.
- [ ] Texture direction, grain, and density remain continuous across sleeves, torso, lapels, pockets, and seams.
- [ ] Retouching does not make the shell plastic, smooth, waxy, fuzzy, over-sharpened, or uniformly tiled.
- [ ] Lining, when visible, remains smooth and light cream with physically plausible folds and sheen.
- [ ] Seams and tone-on-tone stitching are fine, even, continuous, and structurally plausible.
- [ ] Fabric folds respond naturally to pose and gravity without melted edges or impossible tension.

### D. Geometry / multi-image consistency

- [ ] Front, back, side, and oblique views describe the same garment volume and proportions.
- [ ] Shoulder line, waist shaping, hem level, sleeve length, lapel geometry, pockets, and vent align across the set.
- [ ] Left/right symmetry is preserved only where supported by Ground Truth.
- [ ] Perspective and pose do not falsely alter jacket length or pocket/button placement.
- [ ] Occluded construction is not hallucinated; uncertain regions are hidden or flagged.

### E. Color / lighting / retouching

- [ ] White balance preserves the warm cream/ivory reference and neutral background separation.
- [ ] Highlights retain texture; shadows retain seam and pocket detail.
- [ ] No local color mismatch occurs between body, sleeves, lapels, pocket flaps, and panels.
- [ ] No halos, cutout edges, doubled seams, ghost buttons, warped hands, fused garments, or generative artifacts remain.
- [ ] Retouching is restrained and does not erase authentic textile texture.

### F. Delivery decision

- [ ] Required product landmarks remain visible at final crop and channel size.
- [ ] Compare final output side-by-side with Ground Truth at fit-to-screen and 100% detail views.
- [ ] Assign one status: `PASS`, `REVISE`, `REJECT`, or `UNCERTAIN / HOLD`.
- [ ] Any hard-fail product-identity deviation = `REJECT`.
- [ ] Any unresolved construction detail presented as fact = `REJECT`.
- [ ] Any unresolved but safely hidden detail = `UNCERTAIN / HOLD` until explicitly reviewed.
- [ ] Only `PASS` assets may enter `07_DELIVERY` or the final portfolio.

## CURRENT GATE

**Status: `CLEARED` for front-facing generation.**  
The user's latest instruction on 2026-09-20 supersedes the earlier setting: all production assets must show exactly **3 front buttons** whenever the full closure is visible.
