# AI_CONTEXT_LOADING_RULES

## Purpose

防止 Context 過載、來源混亂與記憶污染，讓 AI 使用最小且足夠的上下文。

## System Role

定義 AI 在回答或產出前如何選擇、載入與限制上下文。

## Input

- 使用者問題
- 相關文件
- AI Memory
- Schema
- Workflow

## Output

- Context Pack
- 來源清單
- 缺口清單
- 排除清單

## Workflow

1. 確認任務目的。
2. 搜尋必要文件。
3. 優先載入治理、Schema、Workflow。
4. 只加入與任務直接相關的內容。
5. 標記推論與事實。
6. 輸出前檢查來源。

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

- 接 Context Compressor。
- 接 Ollama 初步摘要。
- 接 Python Context Builder。
- 接上下文污染檢測。

## Examples

``markdown
Context Pack:`n- OUTPUT_RULES.md`n- MEETING_SCHEMA.md`nExcluded: unrelated archive files
``
