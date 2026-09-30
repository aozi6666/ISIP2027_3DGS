# 参考文献占位：待你检索补全

> 原则：下列条目**未当作定稿**；请按检索方式核对 PDF 后改 `references.bib`。  
> 当前 bib **共 48 条**（与原列表条数一致）。

---

## P0 — 实验表已用，必须补全

### 1) `PLACEHOLDER_D2GS`
- **用途**：主实验 / LLFF 表中的 D$^2$GS baseline  
- **当前**：仅有题名占位  
- **检索**：
  1. Google Scholar：`D2GS Depth-and-Density Guided Gaussian Splatting`
  2. 项目页：https://insta360-research-team.github.io/DDGS-website/
  3. arXiv：`2510.08566`；ICLR 2026 PDF（若已公开）
- **补进 bib**：完整 `author`、正式 `booktitle`/`year`/`pages`，然后把 key 改成如 `Lin26_D2GS`，并在 Setup/Related 需要处 `\cite{...}`  
- **改完后**：删除 `PLACEHOLDER_D2GS` 这条 `@misc`

---

## P1 — 作者不全 / 仅转录自旧列表（未 cite 也可先核）

| BibTeX key | 检索词（Scholar） | 要核对 |
|------------|-------------------|--------|
| `Yang23_OpticsVH` | `Real-time light-field generation visual hull Optics Express 2023` | 完整作者 |
| `Li24_AOM_VH` | `visual hull carbon nanotubes photo-imager Advanced Optical Materials 2024` | 完整作者 |
| `Xiao23_LevelS2fM` | `Level-S2fM Structure from Motion CVPR 2023` | 完整作者（**不要**当传统 SfM 主引用；SfM 已用 COLMAP） |
| `Huang24_SCNeuS` | `SC-NeuS AAAI 2024` | 作者/页码 |
| `Zou24_Sparse3D` | `Sparse3D Distilling multiview-consistent diffusion AAAI 2024` | 作者/页码 |
| `Gao24_LOP_3DGS` | `Advances in differentiable rendering 3D Gaussian Laser Optoelectronics Progress 2024` | 完整作者 |
| `Zhang24_CoRGS` | `CoR-GS ECCV 2024` | ECCV **最终页码**（现有 arXiv note） |
| `Ding25_EyeNavGS` … `Zhang25_GlossyGaussian` | 用各条目 `title` 原样搜 | 作者/`et al.` 展开、页码、年份 |

---

## 已稳定、不要再按旧编号改的（正文已挂上）

| Key | 用途 |
|-----|------|
| `Yang23_FreeNeRF` | Intro 稀疏过拟合 |
| `Niemeyer22_RegNeRF` | Intro 几何模糊；Related |
| `Kerbl23_3DGS` | 3DGS / rasterization / color loss |
| `Schonberger16_COLMAP` | **SfM**（替代旧错号） |
| `Chung24_DepthRegGS` | 初始化稳定性 |
| `Xu25_DropoutGS` / `Park25_DropGaussian` | floater / 弱梯度 / compensation 对比 |
| `Li24_DNGaussian` `Zhu24_FSGS` `Xiong24_SparseGS` `Zhang24_CoRGS` | Related sparse 3DGS |
| `Mildenhall21_NeRF` + SparseNeRF/DS-NeRF | Related NeRF |
| `Wang25_VGGT` | 3.3 |
| `Laurentini94_VisualHull` `Lysykh25_VisualHull` | 3.2 VH |
| `Balta18_SOR` | 去离群点 |
| `Barron22_MipNeRF360` `Mildenhall19_LLFF` | Setup 数据集 |
| `Wang04_SSIM` `Zhang18_LPIPS` | 在 bib 中保留；正文 loss 跟 Kerbl |

---

## 已删除（不要再加回）

| 原稿 | 原因 |
|------|------|
| #3 学位论文 | 会议不宜 |
| #4 地方期刊 SIFT | 弱相关 |
| #11（=#5 重复） | 重复 |
| #25 加纳社科论文 | 污染 |
| #45 综述 Kathariya | 为腾名额给必需文献；且曾被错挂为 LLFF |

## 为保持 48 条而新增

`Schonberger16_COLMAP`，`Park25_DropGaussian`，`Laurentini94_VisualHull`，`Zhang24_CoRGS`，`PLACEHOLDER_D2GS`
