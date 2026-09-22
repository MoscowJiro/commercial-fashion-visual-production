# 未生成图片清单与生图提示词

**统计口径：** 只列“从未返回可供 QC 的候选图”的正式交付项；已经生成但被 `REJECT` 的图片不列入。多次失败的同一目标只计 1 项。  
**总数：** 19 张（Phase 02：5；Phase 03：6；Phase 04：7；Phase 05：1）  
**全局锁定：** 前襟恰好 3 颗纽扣；2 个腰部翻盖口袋；cream/ivory；短款 regular fit；经典缺口驳领；不规则细密毛呢纹理。

## 使用方法

每张图的完整提示词 = 对应 Phase 的“共用提示词” + 表格中的“单图附加提示词”。每个目标必须独立调用一次生图，并在生成后执行 `PRODUCT_SPEC.md` QC。

## Phase 02 — Product Assets（5 张）

**对应文件夹：** `02_PRODUCT_ASSETS/`

### Phase 02 共用提示词

```text
Use case: product-mockup
Asset type: standard e-commerce product reference asset
Input image 1: 01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png, the authoritative complete product reference.
Input image 2: 02_PRODUCT_ASSETS/RP_07_FABRIC_MACRO_v01.png, authoritative for shell color and texture.
Input image 3: 02_PRODUCT_ASSETS/RP_08_BUTTON_DETAIL_v01.png, authoritative for button appearance.
Scene: seamless neutral light warm-gray studio, no props, text, logo or watermark.
Style: photorealistic restrained commercial product photography, invisible support, no mannequin, hanger or human.
Lighting: broad soft neutral studio light; accurate cream/ivory color; texture and stitching readable.
Locked product: short upper-hip regular-fit women's wool-blend jacket, slight waist shaping, structured shoulders, full straight sleeves, classic moderate-width notch lapel, deep V, exactly THREE warm-brown marbled round four-hole front buttons when visible, exactly TWO waist-level horizontal flap pockets, curved front hem, centered back seam and one center vent, fine tone-on-tone stitching, irregular fine nubby matte wool texture.
Constraints: no added or removed seams, darts, pockets, buttons, vents, belt, zipper, piping, embroidery, label, logo, trim or decoration. No color, proportion, length, lapel, pocket, button, fabric or stitching change.
```

| ID / 目标文件名 | 状态 | 单图附加提示词 |
|---|---|---|
| `RP_03_LEFT_v01.png` | 未生成 | `Strict 90-degree left-side view, full garment centered, normal perspective. Show collar profile, shoulder-to-sleeve relationship, short length, light waist shaping, sleeve length and only the physically visible edge of the waist flap pocket. Do not expose or invent hidden internal/cuff construction.` |
| `RP_04_RIGHT_v01.png` | 未生成 | `Strict 90-degree right-side view matching RP-03 in camera height, scale and light. Preserve garment depth, collar profile, short length and sleeve geometry. Do not mirror-invent unsupported details; show only reference-supported structure.` |
| `RP_05_3Q_FRONT_v01.png` | 未生成 | `Front three-quarter view at about 35–45 degrees, full garment centered. Jacket closed; all THREE front buttons and both flap pockets must remain countable and structurally correct. Preserve lapel depth, pocket level, sleeve volume and hem length under perspective.` |
| `RP_06_3Q_BACK_v01.png` | 未生成 | `Rear three-quarter view at about 35–45 degrees, full garment centered. Clearly preserve centered back seam, exactly one center vent, rear collar, light waist shaping, sleeve volume and continuous rear hem. No side vents or extra back seams.` |
| `RP_11_STITCHING_DETAIL_v01.png` | 未生成 | `Square 1:1 extreme macro of one confirmed clean garment edge seam with fine even tone-on-tone stitching. Diagonal seam across frame, enough fabric on both sides to verify continuous irregular nubby texture. No contrast thread, double decorative rows, embroidery, binding, quilting, fraying or skipped stitches.` |

## Phase 03 — Model Images（6 张）

**对应文件夹：** `03_MODEL_IMAGES/`

### Phase 03 共用提示词

```text
Use case: photorealistic-natural
Asset type: commercial fashion lookbook model image
Input image 1: 01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png, authoritative for complete garment and intended model identity/mood.
Input image 2: 02_PRODUCT_ASSETS/RP_07_FABRIC_MACRO_v01.png, authoritative fabric.
Input image 3: 02_PRODUCT_ASSETS/RP_08_BUTTON_DETAIL_v01.png, authoritative button.
Scene: clean neutral light warm-gray studio, no props, text, logo or watermark.
Model: the same consistent adult East Asian woman identity across the set; distinctive natural non-influencer face, restrained makeup, dark natural hair, visible real skin texture, realistic anatomy and hands. Same plain cream knit top, cream tailored trousers and minimal black shoes.
Jacket: exact short cream/ivory regular-fit wool-blend jacket; structured shoulders; full straight sleeves; classic notch lapel; exactly THREE front buttons; exactly TWO simple waist flap pockets; curved front hem; irregular nubby matte texture. No added structure.
Priority: product truth over pose or beauty. No garment redesign, obstruction, aggressive retouching or body distortion.
```

| ID / 目标文件名 | 状态 | 单图附加提示词 |
|---|---|---|
| `M02_3Q_FULL_BODY_v01.png` | 未生成 | `Full-body 3/4 pose at about 30 degrees, head to shoes visible, calm stance, arms away from jacket. Jacket closed; all 3 buttons, both pocket flaps, hem and sleeve length readable.` |
| `M03_SIDE_v01.png` | 未生成 | `Full-body strict side pose, neutral posture, hair kept clear of collar and shoulder. Preserve jacket depth, short length, shoulder/sleeve relationship and pocket projection; do not invent hidden front or back details.` |
| `M04_BACK_v01.png` | 未生成 | `Full-body strict back pose, arms relaxed slightly away from torso. Clearly show rear collar, centered back seam, one center vent, short hem and regular-fit silhouette. No extra vents or back decoration.` |
| `M05_MID_SHOT_v01.png` | 未生成 | `Straight front mid shot from head to upper thigh. Jacket closed; moderate notch lapel, all 3 buttons, both simple flap pockets and full hem visible. Hands must not cover product landmarks.` |
| `M06_NATURAL_WALKING_v01.png` | 未生成 | `Full-body natural slow walking pose, torso front-biased, low arm swing clear of jacket. Keep all 3 buttons and both flap pockets visible; fabric drape must remain physically plausible without changing length or fit.` |
| `M07_DETAIL_v01.png` | 未生成 | `Close commercial detail on upper torso and waist, including lapel, all 3 front buttons, both pocket flaps and true wool texture. Preserve natural skin/hands only if visible; no crop that hides the required product landmarks.` |

## Phase 04 — Commercial Visuals（7 张）

### A. E-commerce Studio

**对应文件夹：** `04_LIFESTYLE_EDITORIAL/A_ECOMMERCE_STUDIO/`

```text
Use case: photorealistic-natural
Asset type: Phase 04 A E-commerce Studio candidate
References: Ground Truth for complete jacket and consistent adult East Asian female identity; PASS fabric macro; PASS button detail.
Scene: seamless clean neutral warm light-gray studio, no props, text, logo or watermark.
Model/styling: same adult East Asian woman, natural face and skin, restrained makeup, dark hair; same cream knit top, cream wide-leg trousers and black shoes.
Jacket lock: exact short cream/ivory regular-fit jacket, moderate notch lapel, exactly THREE buttons, exactly TWO simple flap pockets with no patch outlines, irregular nubby texture, no extra seams or decoration.
Lighting: identical broad soft neutral studio light. Product truth over visual effect.
```

| 目标文件名 | 状态 | 单图附加提示词 |
|---|---|---|
| `A1_FRONT_FULL_BODY_v01.png` | 未生成 | `Strict front full-body pose, centered, head to shoes visible, arms relaxed away from torso. Jacket closed; all 3 buttons and both pocket flaps countable, normal lens perspective.` |
| `A2_3Q_FULL_BODY_v01.png` | 未生成 | `Full-body 3/4 view rotated about 30 degrees, centered, subtle weight shift, hands away from jacket. All 3 buttons and both simple flap pockets remain readable.` |

### B. Minimal Lifestyle

**对应文件夹：** `04_LIFESTYLE_EDITORIAL/B_MINIMAL_LIFESTYLE/`

```text
Use case: photorealistic-natural
Asset type: Phase 04 B Minimal Lifestyle candidate
References: Ground Truth for exact jacket/model identity; PASS fabric and button references.
Scene: quiet minimal contemporary interior in warm neutral stone, plaster and pale wood; uncluttered daylight; no props touching garment; no text, logo or watermark.
Model/styling: same adult East Asian woman and same cream knit, cream trousers and black shoes across the set.
Jacket lock: exact cream/ivory short regular-fit jacket, classic notch lapel, exactly THREE buttons, exactly TWO simple waist flap pockets without patch outlines, irregular nubby matte fabric, no extra seams or design changes.
Priority: product truth over lifestyle atmosphere; accurate neutral color.
```

| 目标文件名 | 状态 | 单图附加提示词 |
|---|---|---|
| `B2_NATURAL_WALK_v01.png` | 未生成 | `Full-body slow natural walk across the sparse interior, torso nearly front-facing, low arm swing clear of garment. All 3 buttons and both pockets visible; realistic drape.` |
| `B3_WINDOW_3Q_v01.png` | 未生成 | `Three-quarter-length portrait near a large diffused window, subtle 25-degree body turn, hands at sides. Jacket closed; lapel, all 3 buttons, both pockets and hem fully visible.` |

### C. Fashion Editorial

**对应文件夹：** `04_LIFESTYLE_EDITORIAL/C_FASHION_EDITORIAL/`

```text
Use case: photorealistic-natural
Asset type: Phase 04 C Fashion Editorial candidate with strict product fidelity
References: Ground Truth for complete jacket and same adult East Asian female identity; PASS fabric and button references.
Model/styling: same natural adult model, restrained makeup, real skin texture; same cream knit and tailored trousers.
Exact jacket: short cream/ivory regular fit; classic moderate notch lapel; exactly THREE visible front buttons; exactly TWO simple waist flap pockets with no patch outlines; curved hem; irregular nubby matte surface; no extra seam, dart, pocket, belt, zipper, logo or trim.
Editorial direction: refined modern minimalism and controlled light, while every product landmark remains readable. Product truth has priority over drama.
```

| 目标文件名 | 状态 | 单图附加提示词 |
|---|---|---|
| `C1_GEOMETRIC_SHADOW_FULL_v01.png` | 未生成 | `Full-body front-facing portrait against a sculptural matte warm-gray wall with one broad geometric shadow. Arms down; all 3 buttons, both simple flap pockets and hem visible.` |
| `C2_SEATED_3Q_v01.png` | 未生成 | `Restrained seated-perch pose on a plain low neutral block, torso upright and nearly front-facing, hands away from jacket. All 3 buttons, both flap pockets and hem unobscured.` |
| `C3_TURNING_STEP_v01.png` | 未生成 | `Full-body profile-to-3/4 transition pose, gentle turn toward camera, one step paused, arms away from torso. Exact closure and pockets visible; minimal warm-gray cyclorama and subtle long shadow.` |

## Phase 05 — Retouching（1 张）

**目标文件夹：** `05_RETOUCHING/CASE_C_MINOR_CORRECTION/`  
**目标文件名：** `AFTER.png`  
**当前状态：** `UNCERTAIN / NOT PRODUCED`；四次编辑请求均在服务传输层失败。

### 完整编辑提示词

```text
Use case: precise-object-edit
Asset type: Phase 05 CASE C Minor Visual Correction
Input image 1: 05_RETOUCHING/CASE_C_MINOR_CORRECTION/BEFORE.png, edit target.
Input image 2: 01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png, authoritative complete jacket reference.
Input image 3: 02_PRODUCT_ASSETS/RP_07_FABRIC_MACRO_v01.png, approved fabric reference.
Input image 4: 02_PRODUCT_ASSETS/RP_08_BUTTON_DETAIL_v01.png, approved button reference.
Primary request: remove only the two unsupported rectangular patch-pocket outline seams beneath and surrounding the two existing waist flap pockets. Replace only those thin erroneous seam-line regions with seamless matching cream/ivory nubby wool texture. Keep exactly the two original simple horizontal flap pockets, unchanged in location, size and shape.
Preserve absolutely everything else: the adult model identity, face, natural skin, hair, expression, body, pose, hands, trousers, shoes, background, framing, camera, lighting, shadows, jacket color, short silhouette, regular-fit proportion, length, shoulders, sleeves, classic notch lapel, deep V, curved hem, fabric texture, stitching and exactly THREE visible front buttons in the same positions.
QC-critical constraints: exactly 3 front buttons; exactly 2 flap pockets; no patch-pocket bodies or outline seams; no new or removed garment panels, darts, seams, folds, buttons, pockets, trims, logos or decoration. No beauty retouching. Do not change any area outside the erroneous pocket outline seams. Repaired fabric must match the approved irregular matte wool texture with no blur, clone repetition or visible patch boundary.
```

## 不计入“未生成”的项目

- Phase 02 Front / Back / Pocket / Lapel：图片已生成，但 QC 为 `REJECT`。
- Phase 03 Front Full Body：图片已生成，但口袋结构错误，QC 为 `REJECT`。
- Phase 04 A3 / B1：图片已生成，但结构错误，QC 为 `REJECT`。
- Phase 07：6 张渠道适配均已生成并 `PASS`。
