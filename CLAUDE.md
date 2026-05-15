# CLAUDE.md

本 repo 為 Hatsuon 產品的頂層 **Product git**。Hatsuon 是一款日文發音練習 App，以 React Native Expo 開發。

## 四層 git 結構

Hatsuon 產品採四層 git 拆分。

- **頂層 Product git：**
    - 即本 repo
    - 管理 `no1_product_initiation/`、`no2_product_planning/`、`no5_project_management/`
- **Module Design git：**
    - 位於 `no3_product_designs/<module_id>/`
    - 目前無 Design git；本產品尚未進入設計工件階段
    - 容器目錄已預留
- **Module Spec git：**
    - 位於 `no4_product_specs/<module_id>/`
    - 由頂層 `.gitignore` 排除
- **Module Impl git：**
    - 位於 `no6_product_development/<module_id>/`
    - 由頂層 `.gitignore` 排除

## 當前 module 註冊

- `no1_pronunciation_app`
    - Design git：尚無
    - Spec git：`no4_product_specs/no1_pronunciation_app/`
    - Impl git：`no6_product_development/no1_pronunciation_app/`

完整權威配對表由 `decision_framework_router` skill 的 `products_registry.md` 維護。

---

## 目錄說明

- `no1_product_initiation/` — 提案層：產品定義
- `no2_product_planning/` — 需求與整合層容器，目前為 placeholder，未來擴充需求與 Product Map
- `no3_product_designs/` — Module Design git 容器（目前無 Design git）
- `no4_product_specs/` — Module Spec git 容器
- `no5_project_management/` — 專案管理，含 MVP 規劃
- `no6_product_development/` — Module Impl git 容器

---

## 歷史

本 repo 由原 `HatsuonSpec/` 與 `HatsuonApp/` 兩個兄弟 repo 重構而來。編號結構已對齊 SuSuGiGi 決策框架風格。重構前的檔案命名對應如下。

- 舊 `no2_content_spec/` → 新 `no4_product_specs/no1_pronunciation_app/no1_data_models/`
- 舊 `no3_module_specs/` → 新 `no4_product_specs/no1_pronunciation_app/no3_logics/`
- 舊 `no4_screen_specs/` → 新 `no4_product_specs/no1_pronunciation_app/no2_screens/`
- 舊 `no5_dev_management/` → 新 `no5_project_management/`

2026-05-15 配合四層 git 重構，將原 `no3_product_specs/` 重編為 `no4_product_specs/`、`no4_project_management/` 重編為 `no5_project_management/`、`no5_product_development/` 重編為 `no6_product_development/`，新增 `no3_product_designs/` 容器目錄。

---

## 撰寫規範

所有 .md 文件依循 `universal_writing_linter` skill 的通用政策。任何改動前先 consult `decision_framework_router` skill 的上游 review 四問。
