# PHASE 07 — MULTI-CHANNEL VISUAL ADAPTATION

**Source policy:** QC-PASS final assets only  
**Method:** Pixel-preserving recomposition by crop; no stretch, geometric transform, generative reconstruction, or use of REJECT assets  
**Scope note:** No full-garment or model asset has passed earlier QC, so this delivery is intentionally product-detail-led.

## Source Assets

1. `05_RETOUCHING/CASE_A_BACKGROUND_CLEANUP/AFTER.png` — approved button/fabric detail.
2. `05_RETOUCHING/CASE_B_CANVAS_EXTENSION/AFTER.png` — approved portrait fabric macro.

## Deliverables

| Channel simulation | Ratio | Pixel dimensions | Asset | Recomposition decision | QC |
|---|---:|---:|---|---|---|
| E-commerce PDP | 1:1 | 1254 × 1254 | `PDP/PDP_1x1_BUTTON_DETAIL.png` | Preserve full approved square; centered button supports product-detail zoom | **PASS** |
| E-commerce PDP alternate | 3:4 | 939 × 1252 | `PDP/PDP_3x4_BUTTON_DETAIL.png` | Narrow portrait crop retains complete button and surrounding textile context | **PASS** |
| Social Media feed | 4:5 | 1120 × 1400 | `SOCIAL/SOCIAL_4x5_FABRIC_DETAIL.png` | Near-full portrait macro; diagonal fold remains the visual anchor | **PASS** |
| Mobile / Story | 9:16 | 783 × 1392 | `MOBILE/MOBILE_9x16_FABRIC_DETAIL.png` | Narrow center crop follows the fold vertically without changing fiber scale | **PASS** |
| Campaign Banner | 16:9 | 1248 × 702 | `CAMPAIGN/CAMPAIGN_16x9_BUTTON_DETAIL.png` | Horizontal crop places button with surrounding material field; no synthetic extension | **PASS** |
| Desktop hero/detail | 16:9 | 1120 × 630 | `DESKTOP/DESKTOP_16x9_FABRIC_DETAIL.png` | Wide crop follows diagonal texture ridge and preserves material readability | **PASS** |

## Cross-size Product Consistency QC

| Check | Result | Evidence |
|---|---|---|
| Color | **PASS** | All crops retain source pixels and the same warm cream/ivory values |
| Button geometry | **PASS** | Round outline, warm-brown marbling, four holes, and attachment thread remain unchanged |
| Fabric texture | **PASS** | Fiber scale, irregular nubby surface, fold direction, and matte response are unchanged |
| Proportion | **PASS** | No source pixel was non-uniformly scaled; crops only remove outer image area |
| Structure | **PASS within visible scope** | No seams, pockets, lapels, or garment geometry were generated or altered |
| Edge / crop safety | **PASS** | Button remains complete where present; fabric folds remain continuous and readable |

## Human QC Decision

- All six adaptations are approved for detail-led channel mockups.
- They do **not** substitute for full PDP hero, full model, or full campaign imagery.
- Full-garment channel adaptations remain unavailable until a complete structural product/model asset passes QC.

## Revalidation — 2026-09-21

- Rechecked after the user supplied the previously missing images and after corrective-generation attempts.
- No new full-product or model image achieved `PASS`; the Approved source pool is unchanged.
- All six delivery files exist and their pixel dimensions match the declared ratios exactly.
- SHA-256 integrity hashes were regenerated during revalidation.
- Existing adaptations remain `PASS`; no REJECT source was introduced and no asset was stretched or replaced.
