# OLLAMA_RETRIEVAL_DESIGN

## Purpose

建立可維護的 Ollama Retrieval 設計，支援本地知識檢索但不依賴外部 API。

## System Role

定義未來 Ollama 參與本地檢索與 Context Injection 的設計邊界。

## Input

- Obsidian Markdown
- 本地索引
- 使用者查詢
- 模型名稱
- Context 限制

## Output

- Retrieval Pipeline
- Context Injection 格式
- 來源引用
- 模型限制說明

## Workflow

1. 掃描本地 Markdown。
2. 建立可搜尋索引。
3. 依查詢取回候選文件。
4. 由 Ollama 進行摘要或重排。
5. 將壓縮上下文交給 GPT 或人工使用。
6. 保留來源與版本。

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

- 接 Embedding Strategy。
- 接 Local Vector Store。
- 接 RAG Pipeline。
- 接 Memory Loader。

## Examples

``markdown
Obsidian -> Local Index -> Ollama Summary -> Context Pack -> GPT Reasoning
``
