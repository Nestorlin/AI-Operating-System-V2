# AI_MEMORY_RULES

## Purpose

定義 AI Memory（AI 記憶）的使用規則，確保記憶內容可追蹤、可更新、可驗證，且不污染核心系統。

## Scope

適用於會議摘要、決策紀錄、專案脈絡、使用者偏好、長期知識與 AI 協作紀錄。

## Input

- 使用者明確提供的資訊
- 已確認的決策
- 會議輸出
- 專案狀態
- 風險與後續行動

## Output

- 結構化 AI Memory 條目
- 可檢索摘要
- 可追蹤來源
- 可更新狀態

## Workflow

1. 判斷資訊是否值得長期保存。
2. 確認資訊來源。
3. 分類為決策、偏好、背景、風險或待辦。
4. 寫入對應知識或記憶區。
5. 保留日期與來源。
6. 未確認資訊不得寫入永久記憶。

## Validation

- AI Memory 必須有來源。
- AI Memory 必須可被更新或撤銷。
- 不可保存未確認推測為事實。
- 不可把暫時任務狀態當成長期規則。
- 不可覆蓋核心架構文件。

## Failure Handling

- 資訊來源不明：標記為待確認。
- 記憶與新決策衝突：保留歷史，新增更新紀錄。
- 記憶過期：移入 Archive 或標記失效。
- 記憶不足：回到原始文件重新檢索。

## Future Expansion

- 可建立 Memory Schema。
- 可接 AI Retrieval。
- 可接 Local LLM Context Builder。
- 可接 Automation 定期整理記憶。

## Examples

```markdown
# 2026-05-12_AI_OS_V2_DECISION

## Type
Decision

## Source
User instruction on 2026-05-12

## Content
AI OS V2 文件命名必須使用 UPPER_SNAKE_CASE.md。

## Status
Active
```
