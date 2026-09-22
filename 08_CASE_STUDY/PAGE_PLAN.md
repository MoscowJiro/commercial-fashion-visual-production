# Commercial Fashion Visual Production Case Study — PAGE PLAN

**目标岗位：** 商品视觉制作（AI修图 / AIGC方向）  
**页数：** 15 页  
**叙事重点：** 商品真实性、生产判断与 QC 能力，不把生成数量包装成成果  
**状态：** `PLAN ONLY — AWAITING CONFIRMATION`

## 整体设计系统

- **画幅建议：** 16:9 横版，适合网页嵌入、面试演示与 PDF 阅读。
- **气质：** minimal、editorial、premium fashion。
- **底色：** 暖白与浅灰为主，局部使用 charcoal 黑和参考商品的 warm brown。
- **字体：** 一套高对比衬线体用于标题；一套中性无衬线体用于说明和数据。中文与英文保持统一字重关系。
- **版式：** 大图、宽留白、短标题；每页最多一个主结论。避免卡片式仪表盘、渐变、发光、网格科技感。
- **图片规则：** 不拉伸，不把 REJECT 图当成成品。REJECT 图片必须带清晰状态与错误指示。
- **文案语气：** 直接、克制、可核验。避免夸张的效率或质量宣称。
- **页码与标记：** 小号页码置于固定角落；`PASS / REJECT / UNCERTAIN` 使用低饱和状态色，不使用霓虹色。

## 15 页结构

### 01 — Cover

**核心信息：** 这是一个以商品真实性为中心的 AI 服装视觉生产项目。

- 标题：`Commercial Fashion Visual Production`
- 副标题：`AI Retouching / AIGC Product Workflow`
- 小字：Women's Short Wool Jacket · Portfolio Case Study
- 视觉：Ground Truth 中一张干净商品局部或面料/纽扣特写，大面积留白。
- 来源：`01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png` 的非重复裁切。
- 版式：单图占约 45%，标题居左或居下；不放流程图与长说明。

### 02 — Brief

**核心信息：** 任务不是生成漂亮图片，而是模拟真实商品视觉生产与交付。

- 内容：岗位目标、项目范围、八项能力目标。
- 重点文字：商品信息理解、真实性保持、多图一致性、Visual QC、批量生产、多渠道适配、AI 与人工判断边界。
- 视觉：一条极简生产范围索引，不使用复杂流程图。
- 来源：用户 Brief 与项目目录结构。
- 版式：左侧短文，右侧 8 个简洁能力词；无图片或只用极淡面料背景。

### 03 — Ground Truth

**核心信息：** 一张参考图承担唯一商品视觉基准。

- 内容：展示完整 Ground Truth，并说明它同时提供多角度、材质、工艺、模特与色彩参考。
- 视觉：Ground Truth 全图为主，旁边仅放 3 条证据说明。
- 来源：`01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png`。
- 版式：图片占 70% 以上；不叠加大量标注。

### 04 — Product Analysis

**核心信息：** 生成前先把商品拆成 LOCKED、VARIABLE 与 UNKNOWN。

- 内容：精选 6–8 个关键锁定项，包括 cream/ivory、短款 regular fit、缺口驳领、3 颗纽扣、2 个翻盖口袋、中心背缝/单开衩、不规则毛呢纹理。
- 同页补充：UNKNOWN 示例，包括精确尺寸、材质物理参数、品牌/尺码标签。
- 视觉：Ground Truth 的 front、button、pocket、fabric、back crops，采用编辑式散点布局，不做 UI 卡片。
- 来源：`PRODUCT_SPEC.md` 与 Phase 06 Ground Truth crops。
- 版式：一条主商品轮廓，周围少量文字标签。

### 05 — Production Plan

**核心信息：** 生产顺序由结构母版和 QC 门禁决定。

- 内容：Reference Pack 的 11 个镜头与三批次顺序：结构母版、旋转视图、材质工艺。
- 强调：Front / Back 不通过时，不应扩散到模特和商业场景。
- 视觉：精简的阶段序列与代表缩略图位置，不展示全部失败图。
- 来源：`02_PRODUCT_ASSETS/IMAGE_PLAN.md`。
- 版式：横向单线叙事；每阶段一个图像锚点。

### 06 — Product Assets

**核心信息：** 严格 QC 后，只有 Fabric Macro 与 Button Detail 成为可信商品资产。

- 内容：2 张 PASS 大图；旁注说明其他结构图因驳领、口袋、面料与后开衩漂移被拦截。
- 视觉：`RP_07_FABRIC_MACRO_v01.png` 与 `RP_08_BUTTON_DETAIL_v01.png`。
- 数据：`2 PASS`，其余结构资产未进入 Approved。
- 来源：`06_QC/PHASE_02_QC_REPORT.md`、`06_QC/CORRECTION_GENERATION_QC_2026-09-21.md`。
- 版式：两张图一大一小，状态标记克制；避免“成功率”图表。

### 07 — Model Application

**核心信息：** 自然人物表现不能弥补商品结构错误。

- 内容：展示一张人物观感合格但商品口袋结构错误的模特图。
- 对比：人物真实性通过；商品结构未通过；整体仍为 REJECT。
- 视觉：`06_QC/M01_FRONT_FULL_BODY_v01_REJECT.png`，以清晰错误框或引线指出口袋问题。
- 来源：`06_QC/PHASE_03_MODEL_QC_REPORT.md`。
- 版式：一张大图加一个局部放大；避免多图堆叠。

### 08 — Retouching Case A

**核心信息：** 背景清理的目标是减少干扰，不是抹平真实面料。

- 内容：Problem、Decision、AI Operation、Manual QC、Final Result。
- 视觉：CASE A BEFORE / AFTER 并排，使用同尺度裁切。
- 来源：`05_RETOUCHING/CASE_A_BACKGROUND_CLEANUP/`。
- 结论：PASS。
- 版式：左 BEFORE、右 AFTER，中间只放一句编辑边界。

### 09 — Retouching Case B

**核心信息：** 画布延展只服务版式，不应重绘中央商品证据。

- 内容：从 1:1 到 4:5 的构图需求、生成区域、人工作用边界。
- 视觉：CASE B BEFORE / AFTER；标出“source anchor”和“extended area”。
- 来源：`05_RETOUCHING/CASE_B_CANVAS_EXTENSION/`。
- 结论：PASS，但用途限定为 textile-detail layout。
- 版式：以 1:1 和 4:5 的比例差形成页面构图。

### 10 — Retouching Boundary

**核心信息：** 局部修正一旦变成整图重生成，必须拒绝。

- 内容：CASE C 的原始问题、局部编辑意图、错误 AFTER 与最终 REJECT。
- 视觉：BEFORE 与用户补充的 AFTER；突出人物消失、胸袋新增、贴袋轮廓仍存在。
- 来源：`05_RETOUCHING/CASE_C_MINOR_CORRECTION/`、`06_QC/USER_SUPPLIED_MISSING_ASSETS_QC.md`。
- 版式：BEFORE 占主位，AFTER 作为证据图；红色只用于错误指示。

### 11 — Visual QC Framework

**核心信息：** 每张图都按同一组商品维度检查，而不是凭整体观感判断。

- 内容：Color、Silhouette、Proportion、Lapel、Buttons、Pockets、Fabric、Stitching。
- 决策规则：结构偏差直接 REJECT；无法确认则 UNCERTAIN；只有 PASS 进入交付。
- 视觉：一张商品图配 8 个精简检查点，不做密集 checklist 页面。
- 来源：`PRODUCT_SPEC.md` 与各 Phase QC 报告。
- 版式：商品图为中心，检查词沿边缘排列。

### 12 — AI Failure Case I

**核心信息：** “看起来合理”仍可能不是同一件商品。

- 案例：错误纽扣数量、错误口袋结构、错误领型/内里。
- 每例只保留：Ground Truth、AI Output、一个错误句、REJECT。
- 视觉：Phase 06 Case 01–03 对照图。
- 来源：`06_QC/AI_FAILURE_CASES/`。
- 版式：三条纵向对照，不加入 Corrected Version 以免信息过满。

### 13 — AI Failure Case II

**核心信息：** 面料与比例漂移同样属于商品 hallucination。

- 案例：面料纹理规律化、收腰过度、后开衩/后片结构漂移。
- 视觉：Phase 06 Case 04–05，加一张 texture-only correction 仍失败的证据。
- 来源：`06_QC/AI_FAILURE_CASES/`、`06_QC/RP_06_3Q_BACK_v03_REJECT.png`。
- 结论：局部结构删除可能成功，但整件纹理锁定仍不可靠。
- 版式：一张材质大图 + 一张后视图，文字控制在 4 行以内。

### 14 — Multi-format Delivery

**核心信息：** Approved 细节资产可以通过裁切完成多渠道适配，而不需要拉伸或重生成。

- 内容：1:1、4:5、3:4、9:16、16:9 的渠道映射。
- 视觉：六张 Phase 07 成品按真实比例排列。
- 标注：PDP、Social、Mobile、Campaign、Desktop。
- 来源：`07_DELIVERY/PHASE_07_CHANNEL_ADAPTATION/`。
- 结论：全部比例精确匹配，商品像素未非等比变形。
- 版式：比例本身形成视觉节奏；不使用设备 mockup。

### 15 — Final Assets / Production Judgment

**核心信息：** 最终价值来自可靠筛选，而不是生成数量。

- 内容：最终 Approved 核心资产为 Fabric Macro、Button Detail、Retouching A/B，以及对应多尺寸裁切。
- 明确说明：完整商品与模特图没有通过结构 QC，因此没有进入 Final Assets。
- 能力总结：建立规格、定义门禁、执行生成、识别 hallucination、控制修图范围、完成可信交付。
- 视觉：4 张 Approved 资产精选排版；不放 REJECT 图。
- 来源：`02_PRODUCT_ASSETS/`、`05_RETOUCHING/`、`07_DELIVERY/`。
- 版式：安静收尾，大面积留白；底部用一句话结束：`Only verified assets move forward.`

## 页面节奏

- 01–03：建立项目与视觉基准。
- 04–06：展示商品理解和生产计划。
- 07–10：展示人物应用与修图边界。
- 11–13：展示 QC 方法和错误识别能力。
- 14–15：展示渠道交付与最终判断。

## 选材原则

- `PASS` 图片用于封面、成果和最终资产页。
- `REJECT` 图片只用于 Model Application、Retouching Boundary 与 AI Failure 页面，并明确标识。
- `UNCERTAIN` 不作为视觉成果，只在必要的过程说明中出现。
- 不使用 `work/` 中的审核联系表作为作品集视觉。
- 同一图片原则上只出现一次；Ground Truth 可按不同局部裁切承担不同证据角色。

## 制作前门禁

在进入实际制作前，需要确认：

1. 采用 15 页结构。
2. 采用 16:9 横版，而不是 A4/竖版 PDF。
3. 是否接受将“没有完整商品/模特 PASS 图”作为专业判断展示，而不是隐藏这一结果。
