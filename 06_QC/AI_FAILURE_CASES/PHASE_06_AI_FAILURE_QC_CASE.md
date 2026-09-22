# PHASE 06 — AI FAILURE & QC CASE

**Objective:** Demonstrate detection of product hallucination in AI-generated fashion imagery.  
**Final product lock:** Short cream/ivory wool-blend jacket; classic notch lapel; exactly 3 front buttons; exactly 2 waist flap pockets; irregular nubby matte texture; regular-fit proportions; center-back seam and one center vent.  
**Policy:** AI outputs remain visibly identified as `REJECT`. “Corrected Version” means a verified target derived from Ground Truth or an existing QC-PASS asset—not a cosmetically disguised error.

## Case 01 — Wrong Button Count

| Field | Record |
|---|---|
| GROUND TRUTH | Isolated front reference visibly shows exactly 3 vertically aligned front buttons. Latest user decision also locks the count at 3. |
| AI OUTPUT | `CASE_01_BUTTON_COUNT/AI_OUTPUT_REJECT.png` |
| ERROR | AI generated 4 front buttons and also drifted in lapel/pocket/fabric details. |
| REJECT REASON | Button count is a product-identity feature. One added button changes closure design and makes the image commercially inaccurate. |
| CORRECTED VERSION | `CASE_01_BUTTON_COUNT/CORRECTED_VERSION.png` — deterministic crop from Ground Truth; no generative correction claimed. |

**QC method:** Count every visible button; compare vertical spacing and placement before judging aesthetics.

## Case 02 — Wrong Pocket Structure

| Field | Record |
|---|---|
| GROUND TRUTH | Exactly 2 simple waist-level flap pockets; no patch-pocket bodies or rectangular outline seams below the flaps. |
| AI OUTPUT | `CASE_02_POCKET_STRUCTURE/AI_OUTPUT_REJECT.png` |
| ERROR | AI added large rectangular patch-pocket outlines beneath both legitimate flaps. |
| REJECT REASON | The model converted flap-pocket construction into a hybrid flap-plus-patch structure. Symmetry does not make the hallucination valid. |
| CORRECTED VERSION | `CASE_02_POCKET_STRUCTURE/CORRECTED_VERSION.png` — model crop from Ground Truth showing the intended clean flap-pocket topology. |

**QC method:** Trace each pocket opening and seam. Reject duplicate openings, added outlines, zippers, buttons, or invented pocket bodies.

## Case 03 — Wrong Lapel / Inner Construction

| Field | Record |
|---|---|
| GROUND TRUTH | Moderate-width classic notch lapel with smooth light lining visible inside the neckline. |
| AI OUTPUT | `CASE_03_LAPEL_LINING/AI_OUTPUT_REJECT.png` |
| ERROR | Lapel became too wide and the inner neckline was rendered in shell-like textured wool instead of smooth lining. |
| REJECT REASON | Both lapel geometry and material zoning changed. The image looks plausible as a generic blazer, but it is not this product. |
| CORRECTED VERSION | `CASE_03_LAPEL_LINING/CORRECTED_VERSION.png` — Ground Truth collar crop. Brand label is treated only as source-image content and not as confirmed brand metadata. |

**QC method:** Compare notch angle, lapel width, break line, collar scale, and the boundary between shell and lining.

## Case 04 — Fabric Texture Hallucination

| Field | Record |
|---|---|
| GROUND TRUTH | Soft fine irregular nubby/felted wool-blend texture with matte response and no regular weave motif. |
| AI OUTPUT | `CASE_04_FABRIC_TEXTURE/AI_OUTPUT_REJECT.png` |
| ERROR | AI converted the surface into a regular embossed/woven pattern across the back panel. |
| REJECT REASON | Texture is a material identity feature. A coherent repeating pattern is still wrong when the real fabric is irregular. |
| CORRECTED VERSION | `CASE_04_FABRIC_TEXTURE/CORRECTED_VERSION.png` — existing QC-PASS Fabric Macro asset. |

**QC method:** Inspect at fit-to-screen and 100%. Check repetition, fiber scale, directionality, gloss, tiling, and continuity across seams/folds.

## Case 05 — Silhouette / Back Vent Drift

| Field | Record |
|---|---|
| GROUND TRUTH | Regular fit with light waist shaping, centered back seam, and one clearly structured center vent. |
| AI OUTPUT | `CASE_05_PROPORTION_BACK_VENT/AI_OUTPUT_REJECT.png` |
| ERROR | AI exaggerated hourglass shaping, altered collar/back proportions, and made the center vent too shallow or ambiguous. |
| REJECT REASON | The result changes fit and back construction even though the color remains plausible. Color accuracy cannot compensate for silhouette failure. |
| CORRECTED VERSION | `CASE_05_PROPORTION_BACK_VENT/CORRECTED_VERSION.png` — deterministic Ground Truth back crop. |

**QC method:** Align shoulder width, waist suppression, sleeve length, hem width, center seam, and vent depth against the reference.

## QC Summary

| Case | Primary hallucination | Severity | Decision |
|---|---|---:|---|
| 01 | Added front button | Critical product identity | **REJECT** |
| 02 | Invented pocket bodies/seams | Critical construction | **REJECT** |
| 03 | Lapel and lining material drift | Critical construction/material zoning | **REJECT** |
| 04 | Regularized/changed fabric texture | Critical material identity | **REJECT** |
| 05 | Fit and center-vent drift | Critical silhouette/construction | **REJECT** |

## Human QC Boundary

- Photorealism is not proof of product accuracy.
- Symmetric errors are still errors.
- A visually attractive output is rejected when any locked feature changes.
- Correction is accepted only when the result can be compared with an authoritative reference; otherwise status remains `UNCERTAIN`.
- REJECT assets stay in QC evidence and never enter delivery or portfolio selections as finished product imagery.
