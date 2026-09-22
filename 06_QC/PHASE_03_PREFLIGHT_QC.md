# PHASE 03 — MODEL IMAGES / PREFLIGHT QC

**Requested outputs:** Front Full Body, 3/4 Full Body, Side, Back, Mid Shot, Natural Walking, Detail  
**Required clothing reference policy:** Only Product Assets that passed QC may be used as clothing image references  
**Decision:** `CLEARED` after user authorization to use archived Ground Truth as an additional clothing image reference

## Available PASS references

| Asset | What it reliably defines | What it does not define |
|---|---|---|
| `RP_07_FABRIC_MACRO_v01.png` | Cream/ivory color family; soft fine irregular nubby wool-blend surface; matte material response | Full silhouette, length, lapel, pockets, sleeves, front closure placement, back seam, center vent |
| `RP_08_BUTTON_DETAIL_v01.png` | Warm-brown marbled tortoiseshell-look appearance; round four-hole construction; attachment thread | Four-button spacing and placement on garment; full front construction; any other garment geometry |

## Coverage audit

| Required locked feature | Covered by PASS Product Assets? | Gate |
|---|---:|---|
| Color / fabric texture | Yes | Clear |
| Button appearance | Yes | Clear |
| Exactly 3 front buttons | Partial — count is user-locked and supported by the clearest isolated front view, but spacing and full placement lack a PASS structural asset | Hold |
| Short regular-fit silhouette | No | Hold |
| Jacket length and proportions | No | Hold |
| Classic notch lapel geometry | No | Hold |
| Two flap pockets and placement | No | Hold |
| Sleeve length / cuff structure | No | Hold |
| Back seam / single center vent | No | Hold |
| Cross-view garment identity | No | Hold |

## Shot decisions

| Shot | Status | Reason |
|---|---|---|
| 01 Front Full Body | **UNCERTAIN / HOLD** | Full front construction cannot be anchored by current PASS references |
| 02 3/4 Full Body | **UNCERTAIN / HOLD** | Requires verified front, side, lapel, pocket and sleeve geometry |
| 03 Side | **UNCERTAIN / HOLD** | Requires verified side silhouette and sleeve/cuff structure |
| 04 Back | **UNCERTAIN / HOLD** | Requires verified center seam and center vent asset |
| 05 Mid Shot | **UNCERTAIN / HOLD** | Would expose unsupported lapel, pocket and closure geometry |
| 06 Natural Walking | **UNCERTAIN / HOLD** | Motion increases garment deformation risk without a structural master |
| 07 Detail | **UNCERTAIN / HOLD** | A fabric/button-only crop is possible, but would not satisfy the requested model-lookbook set as a coherent production run |

## QC conclusion

Generating now would require AI to invent garment structure from generic fashion priors. That would violate the LOCKED FEATURES policy and make every structural shot presumptively `REJECT`.

At preflight time, no Phase 03 image had been generated or admitted to `03_MODEL_IMAGES`. The user subsequently authorized Ground Truth as an additional reference, clearing this gate.

## Required release condition

Before Phase 03 may start under the stated reference policy, `02_PRODUCT_ASSETS` needs PASS structural masters covering at minimum:

1. Front — full silhouette, length, lapel, four-button placement, both pockets and sleeves.
2. Back — silhouette, center seam and center vent.
3. Side or 3/4 — garment depth, shoulder/sleeve relationship and pocket projection.

Alternative release condition: the user explicitly authorizes the archived Ground Truth itself as an additional clothing image reference for Phase 03. **COMPLETE.**
