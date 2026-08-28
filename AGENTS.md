# Hatsuon 產品規則

- 本 repo 是 Hatsuon 的 Product git
- 產品為日文假名讀音對應熟練 App
- 技術基礎為 React Native Expo

## 多層 git 結構

- Product git 承載提案與規劃層
- Spec git 位於 `no3_product_specs/no1_pronunciation_app/`
- Impl git 位於 `no5_product_development/no1_pronunciation_app/`
- Design git 尚未建立
- Module 配對以 `decision_framework_router` 的註冊表為準

---

## 目錄責任

- `no1_product_initiation/`
  - 承載產品定義
- `no2_product_planning/`
  - 承載需求與 Product Map
- `no3_product_specs/`
  - 承載獨立 Module Spec git
- `no4_product_designs/`
  - 預留 Module Design git
- `no5_product_development/`
  - 承載獨立 Module Impl git

---

## 原生工作規則

- 任何改動先使用 `decision_framework_router`
- Markdown 改動使用 `universal_writing_linter`
- Spec 文件改動先使用 `spec_writer`
- 跨層改動使用同名 feat branch
- 配對 commit 使用相同 subject 與 body
- 上游需求與 Product Map 已建立
- 變更前需確認上游對應仍成立

---

## 歷史脈絡

- 本 repo 由 HatsuonSpec 與 HatsuonApp 重構而來
- 舊 content spec 對應 Model 層
- 舊 screen specs 對應 View 層
- 舊 module specs 對應 Logic 層
- 專案管理已移至工作區根層
- 現行層編號自 2026-07-21 生效

---

## 相容與漂移控制

- `AGENTS.md` 是本目錄的規則真相
- `CLAUDE.md` 只保留 Claude Code 入口
- 產品規則不得複製回相容入口
- 漂移檢查確認相容入口只含導向規則
