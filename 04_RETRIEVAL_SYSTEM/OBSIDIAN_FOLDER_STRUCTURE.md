# OBSIDIAN_FOLDER_STRUCTURE

## Purpose

建立可雙向連結、可搜尋、可長期維護的 Obsidian 資料夾結構。

## System Role

定義 Obsidian 知識庫的資料夾語義，避免文件成長後失控。

## Input

- 系統層級
- 文件類型
- 知識分類
- 使用者工作流程

## Output

- 資料夾用途表
- 文件放置規則
- 連結與索引原則

## Workflow

1. 依系統層級建立資料夾。
2. 依文件用途放置內容。
3. 核心治理文件放在固定位置。
4. 知識文件保持可擴展。
5. Archive 僅保存過期或衝突內容。

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

- 接 File Router。
- 接 Metadata Scanner。
- 接 Obsidian Dataview。
- 接本地知識圖譜。

## Examples

``markdown
11_RETRIEVAL_SYSTEM/RETRIEVAL_ARCHITECTURE.md`n13_AI_MEMORY_SYSTEM/MEMORY_ARCHITECTURE.md`n10_ARCHIVE/過期或衝突文件
``
