# PRESENTATION_VALIDATION

## Purpose

建立工程提案、技術簡報、客戶展示與高階摘要的穩定產出標準。 本文件聚焦於 PRESENTATION VALIDATION。

## System Role

P7 簡報智能層文件，定義從會議紀錄與知識分析到簡報結構與 Canva Prompt 的轉換規則。

## Input

- 使用者需求
- 既有治理文件
- 相關 Schema
- 相關 Workflow
- 本地 Markdown 文件

## Output

- 標準化設計規則
- 可人工執行步驟
- 未來 Python 相容接口
- 驗證與失敗處理規則

## Workflow

1. 確認此文件對應的系統層級。
2. 讀取既有治理、Schema 與 Workflow。
3. 定義人工優先的穩定流程。
4. 保留未來 Python 或 Ollama 介接點。
5. 輸出可被 Obsidian 與 GitHub 讀取的 Markdown。
6. 標記尚未實作能力為 Future Expansion。

## Validation

- 必須使用 Markdown 作為主要格式。
- 必須保持人類可讀與 AI 可讀。
- 不可宣稱尚未實作的功能已經可用。
- 不可依賴 SaaS 或外部 API 作為核心流程。
- 命名必須符合 UPPER_SNAKE_CASE.md。

## Failure Handling

- 資料不足時，輸出缺口清單。
- 來源衝突時，保留來源並標記衝突。
- 格式不一致時，先標記待整理，不直接覆蓋。
- 流程無法完成時，輸出可人工執行的替代步驟。

## Future Expansion

- 接 PPT Workflow。
- 接 Canva Prompt 生成。
- 接簡報驗證器。
- 接客戶風格記憶。

## Examples

``markdown
# PRESENTATION_VALIDATION
Status: Draft
Mode: Manual + Semi-Auto
Dependency: Local Markdown first
``
