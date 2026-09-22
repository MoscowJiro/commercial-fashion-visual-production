# Commercial Fashion Visual Production

*以商品真实性、视觉一致性与商业交付为核心的 AI-assisted Fashion Visual Production Case Study。*

<p align="center">
  <img src="./03_MODEL_IMAGES/M02_3Q_FULL_BODY_v02.png" width="760" alt="Commercial Fashion Visual Production">
</p>

<p align="center">
  <a href="https://moscowjiro.github.io/commercial-fashion-visual-production/"><strong>View Live Portfolio</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="./PRODUCT_SPEC.md">Product Specification</a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="./06_QC/">Visual QC</a>
</p>

---

## Project Overview

这是一个面向 **商品视觉制作 / AI修图 / AIGC Visual Production** 的商业视觉项目。

项目围绕一款女式短款羊毛混纺外套，建立从 **Ground Truth、商品资产、模特应用、AI-assisted Retouching、Visual QC 到 Multi-format Delivery** 的完整生产流程。

项目重点不是单纯生成漂亮图片，而是在使用生成式 AI 提高视觉生产效率的同时，持续控制商品的颜色、版型、结构、纽扣、口袋与面料特征。

> **Product truth over visual effect.**

Generative AI was used for image production and controlled editing, while human direction governed product specifications, reference control, consistency checks, and final QC decisions.

---

## Final Visuals

以下图片均来自最终 **QC-PASS** 资产池。

<table>
  <tr>
    <td width="50%">
      <img src="./02_PRODUCT_ASSETS/RP_01_FRONT_v05.png" alt="Product Front">
    </td>
    <td width="50%">
      <img src="./02_PRODUCT_ASSETS/RP_06_3Q_BACK_v05.png" alt="Product 3/4 Back">
    </td>
  </tr>
  <tr>
    <td align="center"><sub>Product Front · PASS</sub></td>
    <td align="center"><sub>Product 3/4 Back · PASS</sub></td>
  </tr>
  <tr>
    <td>
      <img src="./03_MODEL_IMAGES/M01_FRONT_FULL_BODY_v02.png" alt="Front Full Body">
    </td>
    <td>
      <img src="./03_MODEL_IMAGES/M02_3Q_FULL_BODY_v02.png" alt="3/4 Full Body">
    </td>
  </tr>
  <tr>
    <td align="center"><sub>Front Full Body · PASS</sub></td>
    <td align="center"><sub>3/4 Full Body · PASS</sub></td>
  </tr>
  <tr>
    <td>
      <img src="./03_MODEL_IMAGES/M05_MID_SHOT_v02.png" alt="Mid Shot">
    </td>
    <td>
      <img src="./03_MODEL_IMAGES/M06_NATURAL_WALK_v02.png" alt="Natural Walk">
    </td>
  </tr>
  <tr>
    <td align="center"><sub>Mid Shot · PASS</sub></td>
    <td align="center"><sub>Natural Walk · PASS</sub></td>
  </tr>
</table>

姿势、景别和构图可以变化，但商品的衣长、领型、纽扣、口袋和面料特征必须保持一致。

---

## Production Workflow

**Ground Truth**  
↓  
**Product Assets**  
↓  
**Model Application**  
↓  
**E-commerce / Lifestyle / Editorial**  
↓  
**AI-assisted Retouching**  
↓  
**Visual QC**  
↓  
**Multi-format Delivery**

只有通过 Visual QC 的素材才能进入正式资产池与最终交付。

---

## Ground Truth & Product Lock

<p align="center">
  <img src="./01_GROUND_TRUTH/ground_truth_womens_short_wool_jacket.png" width="900" alt="Ground Truth Product Reference">
</p>

Ground Truth 用于建立商品的原始视觉依据，并将关键商品特征转化为后续生成与 QC 可以执行的 Product Lock。

| Locked Feature | Production Standard |
|---|---|
| **Color** | Cream / Ivory，不允许明显色彩漂移 |
| **Silhouette** | 短款、Regular Fit、轻微收腰 |
| **Closure** | 恰好 3 颗暖棕色四孔仿玳瑁纽扣 |
| **Pockets** | 恰好 2 个腰部水平翻盖口袋 |
| **Fabric** | 细密、不规则、哑光的羊毛混纺纹理 |

完整规范：

[`PRODUCT_SPEC.md`](./PRODUCT_SPEC.md)

---

## AI-assisted Retouching

Retouching 的目标是改善图片呈现，而不是重新设计商品。

<table>
  <tr>
    <th width="50%">BEFORE</th>
    <th width="50%">AFTER · PASS</th>
  </tr>
  <tr>
    <td>
      <img src="./05_RETOUCHING/CASE_A_BACKGROUND_CLEANUP/BEFORE.png" alt="Before Retouching">
    </td>
    <td>
      <img src="./05_RETOUCHING/CASE_A_BACKGROUND_CLEANUP/AFTER.png" alt="After Retouching">
    </td>
  </tr>
</table>

在 Background Cleanup 过程中，纽扣形状、四孔结构、缝线、颜色和周围面料尺度保持不变。

AI 可以处理已经确认的视觉问题，但不能：

- 重新解释商品结构
- 增加不存在的设计细节
- 改变商品颜色与材质
- 在信息不足时自行补全商品结构

---

## Visual QC

每张候选图片均与 `PRODUCT_SPEC.md` 以及已经通过 QC 的 Product Assets 进行对比。

重点检查：

**Color · Silhouette · Proportion · Lapel · Buttons · Pockets · Fabric · Stitching**

### QC Case — Button-count Hallucination

<table>
  <tr>
    <th width="33%">GROUND TRUTH</th>
    <th width="33%">AI OUTPUT · REJECT</th>
    <th width="33%">CORRECTED · PASS</th>
  </tr>
  <tr>
    <td>
      <img src="./06_QC/AI_FAILURE_CASES/CASE_01_BUTTON_COUNT/GROUND_TRUTH.png" alt="Ground Truth">
    </td>
    <td>
      <img src="./06_QC/AI_FAILURE_CASES/CASE_01_BUTTON_COUNT/AI_OUTPUT_REJECT.png" alt="AI Output Reject">
    </td>
    <td>
      <img src="./06_QC/AI_FAILURE_CASES/CASE_01_BUTTON_COUNT/CORRECTED_VERSION.png" alt="Corrected Version">
    </td>
  </tr>
</table>

AI Output 将前襟纽扣从 **3 颗增加为 4 颗**，改变了商品 Locked Feature。

因此即使图片本身具有较高视觉完成度，也会被直接标记：

`REJECT`

校正版本恢复正确商品结构后，才可重新进入 QC。

> **A visually strong image is not a usable commercial asset if the product information is wrong.**

---

## Multi-format Delivery

通过 QC 的源文件进一步适配不同商业渠道。

<table>
  <tr>
    <td width="50%">
      <img src="./07_DELIVERY/PHASE_07_CHANNEL_ADAPTATION/PDP/PDP_1x1_BUTTON_DETAIL.png" alt="E-commerce PDP">
    </td>
    <td width="50%">
      <img src="./07_DELIVERY/PHASE_07_CHANNEL_ADAPTATION/SOCIAL/SOCIAL_4x5_FABRIC_DETAIL.png" alt="Social Media">
    </td>
  </tr>
  <tr>
    <td align="center"><sub>E-commerce PDP · 1:1</sub></td>
    <td align="center"><sub>Social Media · 4:5</sub></td>
  </tr>
  <tr>
    <td>
      <img src="./07_DELIVERY/PHASE_07_CHANNEL_ADAPTATION/MOBILE/MOBILE_9x16_FABRIC_DETAIL.png" alt="Mobile">
    </td>
    <td>
      <img src="./07_DELIVERY/PHASE_07_CHANNEL_ADAPTATION/CAMPAIGN/CAMPAIGN_16x9_BUTTON_DETAIL.png" alt="Campaign Banner">
    </td>
  </tr>
  <tr>
    <td align="center"><sub>Mobile · 9:16</sub></td>
    <td align="center"><sub>Campaign · 16:9</sub></td>
  </tr>
</table>

| Ratio | Commercial Use |
|---|---|
| **1:1** | E-commerce PDP |
| **3:4** | Product Image |
| **4:5** | Social Media |
| **9:16** | Mobile / Story |
| **16:9** | Campaign / Desktop |

跨尺寸适配优先使用 **Cropping / Reframing / Canvas Planning**，避免人物或商品非等比拉伸，同时保持颜色、纹理尺度和商品结构一致。

---

## Role

**Visual Direction · AI Production Workflow · Prompt / Reference Control · Product Consistency · Visual QC · Commercial Delivery**

在项目中，我负责将 Ground Truth 转化为可执行的商品规范，建立 Reference Control，控制生成与修图边界，筛选 PASS 资产，识别 AI Hallucination，并完成最终多渠道视觉交付。

---

## Tools

- **OpenAI ImageGen** — Reference-led Generation & Controlled Editing
- **AI Agent Workflow** — Production Planning, Asset Organization & QC Documentation
- **HTML / CSS / JavaScript** — Responsive Portfolio Website
- **PowerShell / .NET Imaging Utilities** — Cropping, Dimension Check & Asset Validation
- **Git / GitHub** — Version Control & Portfolio Deployment

---

## Live Portfolio

### [View Full Interactive Portfolio →](https://moscowjiro.github.io/commercial-fashion-visual-production/)

The interactive portfolio contains the complete visual presentation of the project.

---

<sub>Commercial Fashion Visual Production · AI-assisted Workflow · Product Accuracy · Visual Consistency · Quality Control</sub>
