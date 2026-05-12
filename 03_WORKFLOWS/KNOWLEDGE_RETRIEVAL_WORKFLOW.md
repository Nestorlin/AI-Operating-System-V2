# KNOWLEDGE_RETRIEVAL_WORKFLOW

## Purpose

定義 AI Retrieval（AI 檢索）的工作流，讓 AI 能從 Obsidian 與 GitHub 友善 Markdown 文件中取得可靠上下文。

## Scope

適用於知識庫查詢、專案上下文查詢、會議查詢、風險查詢、簡報資料收集與 AI Memory 檢索。

## Input

- 查詢問題
- 查詢範圍
- 文件路徑
- Schema 類型
- 時間範圍
- 關鍵字

## Output

- 相關文件清單
- 摘要
- 來源引用
- 缺口清單
- 後續建議

## Workflow

1. 確認查詢目的。
2. 限定查詢範圍。
3. 搜尋相關文件。
4. 讀取高相關內容。
5. 摘要並保留來源。
6. 分離事實、推論與缺口。
7. 輸出可追蹤結果。

## Validation

- 回答必須可追蹤來源。
- 不可把推論當成事實。
- 不可引用不存在文件。
- 查詢結果不足時必須說明缺口。
- 檢索結果必須優先使用系統內文件。

## Failure Handling

- 找不到資料：輸出 `NO_SOURCE_FOUND`。
- 來源衝突：列出衝突文件與日期。
- 查詢範圍過大：要求縮小或分批查詢。
- 文件格式不一致：標記待整理。

## Future Expansion

- 可接 Embedding Index。
- 可接 Ollama Retrieval。
- 可接 Local Vector Database。
- 可接 Python Retriever。
- 可接來源可信度評分。

## Examples

```markdown
# Retrieval Result

## Query
AI OS V2 的命名規範是什麼？

## Sources
- 00_SYSTEM_CORE/FILE_NAMING_STANDARD.md
- 01_SYSTEM_RULES/OUTPUT_RULES.md

## Answer
系統文件使用 UPPER_SNAKE_CASE.md 命名。
```
