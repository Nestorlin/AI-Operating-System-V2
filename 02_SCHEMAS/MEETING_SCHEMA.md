# MEETING_SCHEMA

## Purpose

定義 Meeting Management（會議管理）的標準資料結構，支援會議紀錄、決策追蹤、Action Item 與 AI 檢索。

## Scope

適用於所有會議紀錄、會議摘要、客戶討論、內部討論與專案同步。

## Input

- Meeting ID
- Date
- Topic
- Participants
- Context
- Discussion Notes
- Decisions
- Action Items
- Risks

## Output

- 標準化會議紀錄
- 決策清單
- Action Item 清單
- 可檢索摘要
- 可轉入專案管理與 AI Memory 的資料

## Workflow

1. 建立符合命名規範的會議文件。
2. 填寫基本資訊。
3. 記錄討論重點。
4. 分離決策、待辦、風險。
5. 標記後續追蹤人與日期。
6. 將長期有效資訊同步至 AI Memory 候選資料。

## Validation

- 必須包含日期與主題。
- 必須區分討論、決策與待辦。
- Action Item 必須有 owner（負責人）或標記 `UNASSIGNED`。
- 未確認事項不得寫成決策。
- 文件命名建議使用 `YYYY-MM-DD_TOPIC.md`。

## Failure Handling

- 缺少參與者：標記 `UNKNOWN_PARTICIPANT`。
- 缺少決策：標記 `NO_DECISION_RECORDED`。
- 缺少負責人：標記 `UNASSIGNED`。
- 會議內容不完整：標記待補並保留原始紀錄。

## Future Expansion

- 可接 Calendar Automation。
- 可接 Action Item Tracker。
- 可接 Project Schema。
- 可接 AI Retrieval 與 Meeting Summarizer。

## Examples

```markdown
# 2026-05-12_AI_OS_V2_PLANNING

## Meeting Info
- Meeting ID: MEETING-2026-05-12-001
- Date: 2026-05-12
- Topic: AI OS V2 Planning
- Participants: User, AI

## Decisions
- 文件必須使用 UPPER_SNAKE_CASE.md。

## Action Items
- Owner: AI
- Task: 建立第一到第三批工程文件。
- Status: In Progress
```
