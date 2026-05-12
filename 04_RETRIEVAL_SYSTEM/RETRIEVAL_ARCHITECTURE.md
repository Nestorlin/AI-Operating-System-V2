# RETRIEVAL_ARCHITECTURE

## Purpose

建立 AI OS V2 的知識檢索架構，讓文件能被穩定搜尋、載入、摘要與引用。

## System Role

P4 檢索與智能層的總體架構文件，定義 Obsidian、AI Memory、Local LLM 與未來 Python Retriever 的協作邊界。

## Input

- Obsidian Markdown 文件
- Schema 文件
- Workflow 文件
- AI Memory 條目
- 使用者查詢

## Output

- 檢索流程定義
- Context Loading 規則
- 來源引用策略
- 未來 Local LLM 介接邊界

## Workflow

1. 接收查詢目的。
2. 判斷查詢範圍與資料類型。
3. 優先搜尋本地 Markdown 文件。
4. 依相關性選取上下文。
5. 保留來源路徑與標題。
6. 輸出摘要、引用與缺口。

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

- 接 Python Retriever。
- 接 Embedding Index。
- 接 Ollama 本地檢索。
- 接自動化 Context Builder。

## Examples

``markdown
# Retrieval Request`nQuery: 找出 AI OS V2 的命名規範`nSources: 00_SYSTEM_CORE/FILE_NAMING_STANDARD.md`nOutput: 摘要 + 來源
``
