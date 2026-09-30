# Writing TODO（会议版总控）

> 用途：追踪占位、命名统一、已知冲突与下一节写作顺序。  
> 原则：先定名 → 再写正文 → 最后统一 BibTeX 自动编号。

---

## 0. 已锁定结论

| 项 | 结论 |
|----|------|
| adaptation branch | **有训练**（cross-attention + lightweight fusion；称 VGGT-Depth） |
| GT depth | **重建阶段使用** → Setup 已声明 |
| Setup depth 模型 | **VGGT / VGGT-Depth**；无 ZoeDepth |
| Ablation 第三列 | **Visibility Balancing\*** + 脚注 = DVR |
| Discussion | 只用 **DVR** |
| DVR 首次 `(DVR)` | **3.1** |
| 原 Fig.3 | **默认删除** |
| Results 结构 | **合成** `\subsection{Quantitative and Qualitative Results}`（含 compact Gradient） |
| Setup baselines | **E2=A**：指向 Tables 1–2，不列方法名单 |
| 数据集表题 | **LLFF 360**（正文/Setup/表题统一） |
| Table 3 LPIPS | 与 Table 1/2 同为 **LPIPS\***（$\times 10^{2}$） |
| Fig.5 | Mip-NeRF 360、**4-view**、会议版**一行** |

### 三模块
```text
Visual Hull Initialization
  → VGGT / Depth-Guided Densification
  → Dynamic Visibility Regularization (DVR)
```

---

## 1. 参考文献预留

- [ ] `\bibliography{references}`；占位 → 真实 key；BibTeX 自动编号

| 占位 | 位置 |
|------|------|
| `ref2`,`ref3` | Introduction (sparse-view challenges) |
| `ref6`–`ref16` | Related Work / Intro priors |
| `ref10`,`ref11` | Intro 3DGS |
| `ref24`–`ref30` | Method / Intro SfM |
| `ref25`,`ref26`,`ref37` | Intro init / visibility |
| `ref36`–`ref43` | 3.4 |
| `ref44`,`ref45` | Setup（Mip-NeRF 360 / LLFF 360） |

---

## 2. 图片 / 表格

| 资源 | 状态 |
|------|------|
| `fig:framework` / `fig:vggt_depth` | 注释占位 |
| `fig:dvr`（Fig.3） | 默认删 |
| `fig:gradient`（Fig.4） | 正文已写；图注释占位 `figures/gradient.pdf` |
| `fig:qualitative`（Fig.5） | 正文已写；一行裁切待贴 `figures/qualitative.pdf` |
| `tables/mip360_results.tex` | 表壳 + caption；**数值待从原稿粘贴** |
| `tables/llff_results.tex` | 表壳；caption = **LLFF 360**；数值待贴 |
| `tables/ablation.tex` | 壳 + PSNR 17.51/24.96/26.18；SSIM/LPIPS\* 待贴；脚注已写 |

---

## 3. 术语词典（强制）

| 术语 | 用法 |
|------|------|
| Visual Hull Initialization / Depth Densification / DVR | 正文模块 |
| Visibility Balancing\* | 仅 Ablation 表 + 脚注 |
| LLFF 360 | Setup + Table 2 + 正文 LLFF 段 |
| LPIPS\* | Tables 1–3 统一 $\times 10^{2}$ |
| ~~ZoeDepth~~ / ~~SparseNeRF 统一名单~~ | Setup 已不列具体 baseline |

---

## 4. 已落实

- [x] Method 3.1–3.4
- [x] Setup：VGGT + GT depth；baselines → Tables~\ref{tab:mip360},~\ref{tab:llff}；LLFF 360
- [x] Results 合并正文（诚实写 LPIPS / 9-view）
- [x] Ablation 正文 + 表壳 + DVR 脚注
- [x] Introduction（补齐叙事；三模块正式名；itemize 贡献；无 `(DVR)` / 无 opacity compensation）
- [ ] 从原稿粘贴 Table 1–3 完整数值
- [ ] 贴 Fig.4 / 单行 Fig.5 并取消注释
- [x] Conclusion（三模块正式名；无 LPIPS 句；半句 future work on densification efficiency）
- [ ] 从原稿粘贴 Table 1–3 完整数值
- [ ] 贴 Fig.4 / 单行 Fig.5 并取消注释
- [ ] bib；`main.tex` 骨架

---

## 4c. Introduction — 已确认并写入

| # | 结论 |
|---|------|
| I1 | 补齐叙事的 conference Intro 骨架 |
| I2 | 统一 **VGGT / Depth-Guided Densification** |
| I3 | **itemize** |
| I4 | SynGS 总述点名三模块正式名 |

---

## 4d. Conclusion — 已确认并写入

| # | 结论 |
|---|------|
| C1 | **不加** LPIPS vs D²GS |
| C2 | **加半句** future work（densification efficiency） |
| 命名 | Dynamic Visibility Regularization；无旧长名 |

---

## 5. sections/ 进度

| 文件 | 状态 |
|------|------|
| `01_introduction.tex` | 已写 |
| `02_related_work.tex` | 初稿 |
| `method/01`–`04` | Method 齐 |
| `experiments/01`,`02`,`05` | 已写 |
| `05_conclusion.tex` | **已写** |

### 工程
- [ ] `main.tex` 改论文骨架
- [ ] title / authors / keywords

---

## 6. 下一步

1. 粘贴 Table 1–3 数值 + 图文件
2. bib → `main.tex` 骨架（`\input{sections/...}`）

---

## 7. 投稿前

- [ ] checklist；无 `??`；术语/表题一致
- [ ] 全文 cite 映射与 bib 对齐（原稿编号错位）
- [ ] Discussion/旧稿若再压缩：删 Densification-Progressive… 旧名
