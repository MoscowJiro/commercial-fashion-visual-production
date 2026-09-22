# 用户补充图片校对报告

**审核日期：** 2026-09-21  
**审核范围：** `MISSING_IMAGE_GENERATION_MANIFEST.md` 中原缺失的 19 个正式目标  
**对照基准：** Ground Truth、`PRODUCT_SPEC.md`、QC-PASS Fabric Macro、QC-PASS Button Detail  
**结论：** 19/19 文件已找到；0 PASS，19 REJECT

> 本报告只进行审核，不移动、覆盖或删除用户补充文件。由于这些图片当前位于生产目录，但未通过 QC，不得进入 Delivery 或 Portfolio。

## Phase 02 — Product Assets

| 文件 | Color | Silhouette / Proportion | Structure | Fabric / Stitching | 结论 | 主要 REJECT 原因 |
|---|---|---|---|---|---|---|
| `RP_03_LEFT_v01.png` | PASS | REJECT | REJECT | REJECT | **REJECT** | 侧面出现未锁定的胸部袋口与翻盖下方贴袋轮廓；面料趋向规律压纹；衣身比例偏长/偏收腰 |
| `RP_04_RIGHT_v01.png` | PASS | REJECT | REJECT | REJECT | **REJECT** | 新增胸袋和贴袋式轮廓；结构不再是仅有两个简单腰部翻盖口袋；面料纹理规律化 |
| `RP_05_3Q_FRONT_v01.png` | PASS | REJECT | REJECT | REJECT | **REJECT** | 虽为 3 颗纽扣，但新增胸袋、贴袋轮廓和示例品牌标签；驳领/口袋比例漂移；面料压纹化 |
| `RP_06_3Q_BACK_v01.png` | PASS | REJECT | REJECT | REJECT | **REJECT** | 后片新增明显纵向公主线/分割线；收腰过强；表面呈规律浮雕纹，非 Ground Truth 的不规则毛呢纹理 |
| `RP_11_STITCHING_DETAIL_v01.png` | PASS | N/A | REJECT | REJECT | **REJECT** | 线迹偏粗且间距/走向不够细密均匀；画面引入被裁切的纽扣干扰，未形成纯粹可验证的缝线基准；纹理颗粒偏粗 |

## Phase 03 — Model Images

| 文件 | Model consistency | Product structure | Composition | 结论 | 主要 REJECT 原因 |
|---|---|---|---|---|---|
| `M02_3Q_FULL_BODY_v01.png` | REJECT | REJECT | PASS | **REJECT** | 模特身份与套图其他图片不稳定；翻盖下方出现贴袋轮廓；衣长/收腰与 Ground Truth 不一致 |
| `M03_SIDE_v01.png` | REJECT | REJECT | PASS | **REJECT** | 人物身份漂移；侧面仍露出不应存在的贴袋结构；商品体量与 M02 不一致 |
| `M04_BACK_v01.png` | REJECT | REJECT | PASS | **REJECT** | 人物身份不一致；后片收腰过强、纵向分割线明显；中心开衩不够清晰；面料呈规则浮雕纹 |
| `M05_MID_SHOT_v01.png` | REJECT | REJECT | REJECT | **REJECT** | 新增胸袋；只显示 2 颗纽扣且裁掉下摆/关键口袋信息，不满足要求的 3 颗纽扣和完整商品地标 |
| `M06_NATURAL_WALKING_v01.png` | REJECT | REJECT | REJECT | **REJECT** | 人物身份与前述图片不同；手和动作遮挡口袋/下摆；新增胸袋或不明前片结构，无法完成商品一致性核验 |
| `M07_DETAIL_v01.png` | REJECT | REJECT | REJECT | **REJECT** | 模特身份继续漂移；新增胸袋；口袋和衣摆被裁切/遮挡，不能作为要求中的完整商品 Detail |

### Phase 03 套图一致性结论

- 脸型、眼鼻比例、发型轮廓与肤色在 6 张之间不稳定，无法视为同一模特。
- 驳领宽度、胸袋有无、腰袋拓扑、衣长和收腰程度跨图变化。
- 因此即使单张观感自然，也不能组成商业生产所需的一致套图。

## Phase 04 — Commercial Visuals

| 文件 | Model consistency | Buttons | Pockets / Structure | Brief match | 结论 | 主要 REJECT 原因 |
|---|---|---|---|---|---|---|
| `A1_FRONT_FULL_BODY_v01.png` | REJECT | PASS | REJECT | PASS | **REJECT** | 3 颗纽扣正确，但翻盖下方出现成对贴袋轮廓；人物身份与其他候选不一致 |
| `A2_3Q_FULL_BODY_v01.png` | REJECT | REJECT | REJECT | PASS | **REJECT** | 可见纽扣不足 3 颗且间距/遮挡不可验证；贴袋轮廓仍存在；模特身份漂移 |
| `B2_NATURAL_WALK_v01.png` | REJECT | REJECT | REJECT | PASS | **REJECT** | 生成 4 颗纽扣；腰袋结构错误；直接违反最终 3 颗纽扣锁定 |
| `B3_WINDOW_3Q_v01.png` | REJECT | PASS | REJECT | PASS | **REJECT** | 3 颗纽扣正确，但腰部仍为翻盖加贴袋轮廓；人物身份不一致 |
| `C1_GEOMETRIC_SHADOW_FULL_v01.png` | REJECT | PASS | REJECT | REJECT | **REJECT** | 新增/强化贴袋轮廓，且场景变成建筑街景并加入手袋，偏离指定的极简几何影棚构图 |
| `C2_SEATED_3Q_v01.png` | REJECT | REJECT | UNCERTAIN | PASS | **REJECT** | 坐姿遮挡商品，仅能确认 2 颗纽扣；口袋/下摆不能完整 QC；人物身份与套图不一致 |
| `C3_TURNING_STEP_v01.png` | REJECT | PASS | UNCERTAIN | REJECT | **REJECT** | 实际输出为腰部特写而非 full-body turning step；人物身份不可验证，商品一侧被手臂与裁切遮挡 |

## Phase 05 — CASE C AFTER

| 文件 | Edit scope retention | Product structure | Model retention | 结论 | 主要 REJECT 原因 |
|---|---|---|---|---|---|
| `05_RETOUCHING/CASE_C_MINOR_CORRECTION/AFTER.png` | REJECT | REJECT | REJECT | **REJECT** | 编辑目标只是移除两条错误口袋轮廓，但 AFTER 删除了整个人物、姿势、裤装、背景和原构图；同时新增胸袋、示例品牌/尺码标签，且贴袋轮廓仍存在。属于全图重生成，不是 minor correction |

## 关键问题频次

| 问题 | 观察结果 |
|---|---|
| 新增胸袋 | 多张 Product / Model / Retouch 图出现；Ground Truth 与 PRODUCT_SPEC 未锁定该结构 |
| 翻盖下方贴袋轮廓 | 多数正面/3/4 图出现，是本批最稳定的 hallucination |
| 纽扣数量漂移 | Phase 04 B2 为 4 颗；A2/C2 无法确认完整 3 颗 |
| 面料压纹化 | Product Back/Side 与部分 Model 图把不规则毛呢变成规律浮雕纹 |
| 版型漂移 | 多张图收腰过强、衣长或后片分割线变化 |
| 模特不一致 | Phase 03 与 Phase 04 候选无法维持同一身份 |
| 编辑范围失控 | Phase 05 CASE C AFTER 将局部修补变成整图重生成 |

## 最终处置

- **PASS：0**
- **REVISE：0** — 当前问题均涉及结构、身份或编辑范围的硬失败，不适合直接小修后放行。
- **REJECT：19**
- 建议将这些文件继续保留为 Phase 06 的 AI Failure / QC 证据，但不要作为 Approved Final Assets。
