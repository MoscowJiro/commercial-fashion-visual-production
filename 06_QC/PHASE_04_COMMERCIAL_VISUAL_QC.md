# PHASE 04 — COMMERCIAL VISUAL QC REPORT

**Groups:** A. E-commerce Studio / B. Minimal Lifestyle / C. Fashion Editorial  
**Candidate target:** 3 compositions per group  
**Reference set:** Ground Truth + `RP_07_FABRIC_MACRO_v01.png` + `RP_08_BUTTON_DETAIL_v01.png`  
**Final closure lock:** Exactly 3 front buttons  
**Priority:** Product truth > visual effect  
**Selection rule:** Only QC-PASS images may be selected

## Candidate status

| Group | Candidate | Intended composition | Result | QC decision | Reason |
|---|---|---|---|---|---|
| A Studio | A1 | Front full body | No image returned | **UNCERTAIN** | Image service network failure |
| A Studio | A2 | 3/4 full body | No image returned | **UNCERTAIN** | Image service network failure |
| A Studio | A3 | Front mid shot | Candidate generated | **REJECT** | 3-button count passed, but unsupported vertical shaping seams changed the jacket construction |
| B Lifestyle | B1 | Front-biased full body in minimal interior | Candidate generated | **REJECT** | 3-button count passed, but extra rectangular/patch-pocket outlines appeared below both flap pockets |
| B Lifestyle | B2 | Natural walk in minimal interior | No image returned | **UNCERTAIN** | Image service network failure |
| B Lifestyle | B3 | Window-light 3/4 portrait | No image returned | **UNCERTAIN** | Image service network failure |
| C Editorial | C1 | Full-body geometric-shadow portrait | No image returned | **UNCERTAIN** | Image service network failure |
| C Editorial | C2 | Restrained seated 3/4 portrait | No image returned | **UNCERTAIN** | Image service network failure |
| C Editorial | C3 | Turning step editorial portrait | No image returned | **UNCERTAIN** | Image service network failure |

## Detailed QC — generated candidates

| Candidate | Model consistency | Color | Silhouette | Proportion | Lapel | Buttons | Pockets | Fabric | Stitching | Overall |
|---|---|---|---|---|---|---|---|---|---|---|
| A3 | PASS | PASS | REJECT | PASS | PASS | PASS | PASS | PASS | UNCERTAIN | **REJECT** |
| B1 | PASS | PASS | REJECT | PASS | PASS | PASS | REJECT | PASS | UNCERTAIN | **REJECT** |

### A3 evidence

- Adult model identity, natural skin, restrained makeup, neutral studio lighting and three-button closure are acceptable.
- Unsupported vertical shaping/princess-like lines alter the front-panel construction.
- File retained only as `06_QC/P04_A3_STUDIO_MID_v01_REJECT.png`.

### B1 evidence

- Model identity, minimal setting, color, three-button closure and general lookbook tone are acceptable.
- Both flap pockets acquire additional rectangular patch-pocket outlines not present in the locked specification.
- File retained only as `06_QC/P04_B1_LIFESTYLE_FRONT_v01_REJECT.png`.

## Group selection

| Group | Selected images | Decision |
|---|---:|---|
| A. E-commerce Studio | 0 | No PASS candidate; do not select a structurally altered image |
| B. Minimal Lifestyle | 0 | No PASS candidate; do not select a structurally altered image |
| C. Fashion Editorial | 0 | No candidate returned; selection remains `UNCERTAIN` |

## Delivery control

- No image was admitted to `04_LIFESTYLE_EDITORIAL`.
- No REJECT image may be reused as a product or model master.
- The two generated candidates remain in `06_QC` only as audit evidence.
- Phase 04 is incomplete and must resume with new candidates when image generation is available reliably.
