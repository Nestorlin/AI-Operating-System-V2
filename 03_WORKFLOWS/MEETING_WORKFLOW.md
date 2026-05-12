# MEETING_WORKFLOW

## Purpose

定義會議從準備、紀錄、整理、追蹤到記憶更新的工作流。

## Scope

適用於內部會議、客戶會議、專案同步、需求討論與決策會議。

## Input

- `MEETING_SCHEMA.md`
- 會議目的
- 會議資料
- 參與者
- 待討論問題

## Output

- 會議紀錄
- 決策清單
- Action Items
- 風險清單
- AI Memory 更新候選

## Workflow

1. 會前建立議題與資料來源。
2. 會中記錄討論、決策與待辦。
3. 會後依 `MEETING_SCHEMA.md` 整理。
4. 將任務同步至 PM 管理。
5. 將風險同步至風險管理。
6. 將長期有效資訊整理為 AI Memory 候選。

## Validation

- 會議紀錄必須有日期。
- 決策與討論必須分離。
- Action Item 必須可追蹤。
- 風險不可混入一般討論。
- AI Memory 只保存已確認資訊。

## Failure Handling

- 會議資訊不足：建立待補清單。
- 討論與決策混雜：拆分區塊。
- Action Item 無 Owner：標記 `UNASSIGNED`。
- 來源不明：不寫入永久記憶。

## Future Expansion

- 可接語音轉文字。
- 可接會議摘要 Automation。
- 可接 Calendar。
- 可接任務追蹤與提醒。

## Examples

```markdown
# Meeting Workflow Result

## Decisions
- 採用 UPPER_SNAKE_CASE.md 命名。

## Action Items
- 建立治理文件。
- 建立 Schema 文件。
- 建立 Workflow 文件。
```
