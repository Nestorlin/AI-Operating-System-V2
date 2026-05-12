# AI_RUNTIME_CONSTRAINTS

# Purpose（目的）

定義 AI Operating System V2 的執行約束。

此文件為 AI Runtime（AI執行環境）的核心限制規則。

AI 必須遵守以下規範，
不得自由修改系統結構。

---

# Core Principle（核心原則）

AI OS V2 採用：

- Governance First
- Schema First
- Workflow First
- Human Controlled

原則。

AI 屬於協作角色，
不是系統主導者。

---

# AI Must Follow（AI 必須遵守）

## 1. Existing Schema Only（只能使用既有 Schema）

AI 不允許：

- 自創 Schema
- 修改 Schema
- 擴增未授權欄位

所有輸出必須符合：

- 既有 Schema
- 既有命名規則
- 既有資料結構

---

## 2. Existing Workflow Only（只能使用既有 Workflow）

AI 不允許：

- 自創 Workflow
- 修改 Workflow 順序
- 跳過 Validation

Workflow 必須遵守：

- WORKFLOW_STANDARD.md
- SYSTEM_RULES
- VALIDATION RULES

---

## 3. Folder Structure Protection（資料夾結構保護）

AI 不允許：

- 任意新增資料夾
- 任意重新分類
- 任意搬移核心文件

核心資料夾：

- 00_SYSTEM_CORE
- 01_SYSTEM_RULES
- 02_SCHEMAS
- 09_SYSTEM_VALIDATION

屬於 Protected Layer（保護層）。

---

## 4. Naming Convention Lock（命名規則鎖定）

AI 必須：

- 使用既有命名格式
- 保持英文大寫命名
- 使用底線分隔

禁止：

- FINAL_FINAL
- NEW_VERSION
- TEMP_FILE
- COPY_1

此類非治理型命名。

---

## 5. Human Approval Required（需要人工批准）

以下操作必須人工批准：

- 新增 Schema
- 新增 Workflow
- 修改 Governance
- 修改 Runtime Rules
- 修改 Validation Rules

AI 不得自動執行。

---

# AI Role Definition（AI角色定義）

AI 的角色：

- Assist（協助）
- Organize（整理）
- Validate（驗證）
- Retrieve（檢索）
- Generate（生成）

AI 不是：

- Governance Owner
- Architecture Owner
- Final Decision Maker

---

# Runtime Stability Goal（執行穩定目標）

本系統 prioritizes（優先考量）：

- Long-term Stability
- Predictable Structure
- Retrieval Consistency
- Human Maintainability

而非：

- 短期生成速度
- 高自由度輸出
- 無限制自動化

---

# Future Expansion（未來擴展）

未來：

- Python Validator
- Ollama Retrieval
- Local RAG
- Auto Validation

皆必須遵守本文件。