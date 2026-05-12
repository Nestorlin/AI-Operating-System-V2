# FILE_ROUTER_DESIGN

## Purpose

建立不依賴 API 的穩定自動化基礎，讓人類複製貼上、Python 處理與 AI 固定輸出可以協同運作。 本文件聚焦於 FILE ROUTER DESIGN。

## System Role

P5 自動化基礎層文件，定義 GPT、Python、Obsidian、GitHub 與 Ollama 之間的人工加半自動中介規則。

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

- 接 Python 腳本。
- 接 File Router。
- 接本地 Watcher。
- 接半自動匯出與驗證流程。

## Examples

``markdown
# FILE_ROUTER_DESIGN
Status: Draft
Mode: Manual + Semi-Auto
Dependency: Local Markdown first
``
