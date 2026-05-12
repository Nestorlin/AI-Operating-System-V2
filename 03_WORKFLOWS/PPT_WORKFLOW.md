# PPT_WORKFLOW

## Purpose

定義從資料收集到簡報草稿產出的工作流，確保 PPT 內容有來源、有結構、可驗證。

## Scope

適用於專案簡報、會議簡報、策略簡報、知識庫摘要與客戶簡報。

## Input

- `PPT_SCHEMA.md`
- 簡報目的
- 受眾
- 來源文件
- 專案資料
- 會議紀錄
- 風險紀錄

## Output

- Slide Outline
- Slide Draft
- Key Messages
- Data Source List
- Review Checklist

## Workflow

1. 確認簡報目的與受眾。
2. 收集來源資料。
3. 產生簡報敘事架構。
4. 建立投影片大綱。
5. 為每張投影片指定 Key Message。
6. 標記資料來源。
7. 驗證是否有無根據內容。

## Validation

- 每張投影片必須有明確用途。
- 每張投影片必須有 Key Message。
- 所有數據與結論必須有來源。
- 不可產生幻想案例或未確認能力。
- 輸出必須可回溯到來源文件。

## Failure Handling

- 來源不足：停止產生結論，列出資料缺口。
- 受眾不明：先建立一般版，不做高度客製化。
- 架構鬆散：回到目的與 Key Message 重建。
- 無法驗證資料：標記 `UNVERIFIED`。

## Future Expansion

- 可接 PowerPoint 自動生成。
- 可接 Chart Generator。
- 可接 Knowledge Retrieval。
- 可接簡報品質 Validator。

## Examples

```markdown
# Slide Draft

## Slide 1
Title: AI OS V2 Purpose
Key Message: AI OS V2 是長期可維護的 AI PM 與知識系統。
Source: SYSTEM_VISION.md
```
