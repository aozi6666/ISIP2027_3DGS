# Writing TODO（会议版总控）

> 更新：2026-10-01 — 仅核清能确认的：D²GS 正式条；CoR-GS pages+DOI；未核清留给你检索。

---

## 0. 已锁定

三模块命名 / DVR / Ablation Visibility Balancing* / VGGT+GT depth / LLFF 360 / LPIPS* / Results 合并 / SynGS(Ours) 彩表 — 同前。

---

## 1. 待办

### P0
- [x] `main.tex` 骨架 + keywords/邮箱
- [x] 图已启用
- [x] Tables 1–3 迁入
- [x] **`references.bib` R1 语义重建（48 条）+ sections `\cite{}` 重挂**
- [x] DVR：补编号公式 `eq:color_loss`（Kerbl: $(1-\lambda)\mathcal{L}_1+\lambda\mathcal{L}_{\mathrm{D-SSIM}}$）；`eq:dvr_loss` / `eq:dropout_ratio` 已有；不加 Bernoulli mask
- [x] **补全 D²GS → `Song26_D2GS`**（ICLR 2026 / arXiv:2510.08566）
- [x] 修 `\cite{ref30}` → `\cite{Wang25_VGGT}`
- [x] Setup 补 baseline + SSIM/LPIPS cites；Related/Results 挂 D²GS
- [x] `Zhang24_CoRGS` 补 pages 335–352 + DOI（已核）
- [ ] **你检索** → 发我：`Song26_D2GS` 页码（可选）；以及任何打算 cite 的 UNVERIFIED（见 `refs_search_todo.md`）
- [ ] 编译：本地执行；日志放 `output/`

### P1
- [ ] Acknowledgments（有资助再写）
- [ ] checklist / 须知
- [ ] 可选删模板残留图

---

## 2. 文献文件

| 文件 | 说明 |
|------|------|
| `references.bib` | 48 条；`Song26_D2GS` 已正式；其余 UNVERIFIED 为库存 |
| `notes/refs_completion_plan.md` | L1/L2/L3 方案（L2 已执行） |
| `notes/refs_search_todo.md` | 可选核对清单（P0 D²GS 已关） |
| `notes/citation_audit.md` | 审计与策略说明 |

---

## 3. 下一步

1. 本地编译；日志放 `output/`
2. 抽查正文 cite ↔ 论文名
3. （可选）L3：删从未 cite 的 UNVERIFIED，bib 瘦身
