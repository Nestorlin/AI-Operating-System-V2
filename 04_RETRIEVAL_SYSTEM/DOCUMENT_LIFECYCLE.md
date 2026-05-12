# DOCUMENT_LIFECYCLE

## Purpose

避免文件長期累積後失效、重複、衝突或污染 AI Context。

## System Role

定義文件從建立、使用、更新、驗證到封存的生命週期。

## Input

- 新文件
- 更新請求
- 驗證結果
- 使用紀錄
- 過期條件

## Output

- 文件狀態
- 更新紀錄
- 封存決策
- 檢索可用性

## Workflow

1. 建立文件並指定狀態。
2. 依規則更新內容。
3. 定期驗證必要區塊。
4. 標記過期或衝突文件。
5. 封存不再使用的版本。
6. 保留可追蹤歷史。

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

- 接 Python Validator。
- 接 Lifecycle Scanner。
- 接 GitHub 版本檢查。
- 接自動封存建議。

## Examples

``markdown
Status: Active`nReview Date: 2026-06-12`nArchive Reason: Replaced by newer governance document
``
