# Writing TODO（会议版总控）

> 更新：2026-09-30 — 正文/表已齐；卡在 **main 骨架 + 图取消注释 + bib**。

---

## 0. 已锁定（勿再改名）

| 项 | 结论 |
|----|------|
| 三模块 | Visual Hull Initialization → **VGGT / Depth-Guided Densification** → **Dynamic Visibility Regularization (DVR)** |
| DVR 首次 `(DVR)` | **3.1**；Intro 只用全称 |
| Ablation 第三列 | Visibility Balancing\* + 脚注 = DVR |
| Setup | VGGT-Depth（有训练 adaptation）+ **GT depth**；baselines → Tables 1–2；**无 ZoeDepth** |
| 数据集名 | **LLFF 360** |
| LPIPS | Tables 1–3 均为 **LPIPS\***（$\times10^{2}$） |
| Results | Quant+Qual+Gradient **合并**一个 subsection |
| Fig.5 | Mip-NeRF 360、4-view、一行；文件现为 `qualitative.png` |
| 表样式 | 保留 `latex/` 彩色；方法名 **SynGS(Ours)** |

---

## 1. 还没做（按优先级）

### P0
- [x] **`main.tex` 论文骨架**（US letter；title/作者/摘要已按作者原文写入；样例备份在 `docs/SPIE_main_template_sample.tex`）
- [x] 表 packages + `\input{tables/table_style}`
- [x] 图环境已启用（qualitative 用 `.png`）
- [x] **keywords** / **通讯作者邮箱** 已按作者原文写入
- [ ] **Acknowledgments**：未写入（避免自造资助信息）

### P1 — 参考文献
- [ ] 清空 `references.bib` 样例，写入真实条目并映射 `refN`
- [ ] BibTeX 编译通过

### P2 — 投稿打磨
- [ ] 编译检查版式 / 无严重报错
- [ ] checklist / 须知
- [ ] 可选：删模板残留图 `mcr3b.eps`、`MultimediaFigure.jpg`

---

## 2. 已完成

| 模块 | 状态 |
|------|------|
| Intro / Related Work / Method 3.1–3.4 | 已写 |
| Experiments Setup / Results+Gradient+Qual / Ablation | 已写 |
| Conclusion | 已写 |
| Tables 1–3 | 已从 `latex/` 迁入（数据+彩色） |
| `tables/table_style.tex` | 颜色定义就绪 |
| Fig.dvr | 已插入 |
| 术语词典 / 贡献点 `notes/contributions.md` | 已同步 |

### sections 一览
| 文件 | 状态 |
|------|------|
| `01_introduction.tex` | 齐 |
| `02_related_work.tex` | 齐（cite 占位） |
| `method/01`–`04` | 齐（除 framework/vggt 图仍注释） |
| `experiments/01,02,05` | 齐（gradient/qual 图仍注释） |
| `05_conclusion.tex` | 齐 |

---

## 3. 建议下一步

1. 填 `references.bib` 并映射 `refN`
2. `pdflatex main && bibtex main && pdflatex main && pdflatex main`
3. 可选：Acknowledgments 资助信息
