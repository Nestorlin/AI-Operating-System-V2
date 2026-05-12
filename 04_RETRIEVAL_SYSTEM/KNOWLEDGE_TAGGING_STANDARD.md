# KNOWLEDGE_TAGGING_STANDARD

## Purpose

讓知識文件可被穩定分類、搜尋與載入，避免自由標籤造成污染。

## System Role

定義知識標籤規則，支援 Obsidian Tag、AI Retrieval 與未來 Metadata Scanner。

## Input

- 文件主題
- 系統層級
- 知識類型
- 專案或客戶名稱

## Output

- 標準 Tag
- 檢索分類
- Metadata 建議

## Workflow

1. 判斷文件所屬層級。
2. 指定一個主要類型 Tag。
3. 必要時加入狀態 Tag。
4. 避免同義 Tag 重複。
5. 定期檢查低品質 Tag。

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

- 接 Metadata Scanner。
- 接 Tag Validator。
- 接 AI Memory Loader。
- 接 Obsidian 查詢視圖。

## Examples

``markdown
tags: #ai-os-v2 #retrieval #active`ntype: architecture`nstatus: active
``
