# PHASE 03 — MODEL IMAGES QC REPORT

**Reference policy:** Ground Truth + QC-PASS Product Assets (`RP_07`, `RP_08`)  
**Garment lock:** Exactly 3 front buttons; latest user instruction supersedes earlier 4-button rule  
**Admission rule:** Only `PASS` may enter `03_MODEL_IMAGES`  
**Run result:** No image passed

## Generated candidate QC

| Shot | Version | Person realism | Color | Silhouette | Proportion | Lapel | Buttons | Pockets | Fabric | Stitching | Overall |
|---|---:|---|---|---|---|---|---|---|---|---|---|
| 01 Front Full Body | v01 | PASS | PASS | PASS | PASS | PASS | **PASS** | **REJECT** | PASS | UNCERTAIN | **REJECT** |

### 01 Front Full Body v01 — rejection evidence

- Model, anatomy, restrained makeup, skin texture, studio background and lookbook tone are acceptable.
- Jacket displays **3 front buttons**, which now passes the revised final button-count rule.
- Additional rectangular/patch-like outlines appear around or below the two flap pockets, creating unsupported pocket construction.
- The unsupported pocket construction remains an automatic `REJECT`; changing the button rule does not upgrade this image.
- File retained only as `06_QC/M01_FRONT_FULL_BODY_v01_REJECT.png`.

## Shot status

| ID | Shot | Status | Reason |
|---|---|---|---|
| 01 | Front Full Body | **REJECT** | Button count now passes at 3, but candidate still changed pocket construction; prior correction attempts targeted the superseded 4-button rule and failed at transport level |
| 02 | 3/4 Full Body | **UNCERTAIN** | No generated candidate available for QC |
| 03 | Side | **UNCERTAIN** | No generated candidate available for QC |
| 04 | Back | **UNCERTAIN** | No generated candidate available for QC |
| 05 | Mid Shot | **UNCERTAIN** | No generated candidate available for QC |
| 06 | Natural Walking | **UNCERTAIN** | No generated candidate available for QC |
| 07 | Detail | **UNCERTAIN** | No generated candidate available for QC |

## Production decision

- `03_MODEL_IMAGES` contains no generated image.
- The rejected candidate must not be used as a pose, identity, or garment master in later phases.
- Resume from Shot 01 when the image service can complete edits reliably; do not progress to cross-view production without a PASS structural front master.
