# PM_WORKFLOW

## Purpose

定義 PM Management 的工作流，支援單人與 AI 協作的專案規劃、追蹤、風險管理與交付。

## Scope

適用於 AI OS V2 內所有專案、模組、文件批次、功能規劃與交付節點。

## Input

- `PROJECT_SCHEMA.md`
- Roadmap
- Task List
- Meeting Decisions
- Risk Records
- Deliverables

## Output

- 專案狀態更新
- 任務進度
- 里程碑追蹤
- 風險追蹤
- 交付物清單

## Workflow

1. 定義專案目標。
2. 拆分里程碑。
3. 拆分任務。
4. 建立任務狀態。
5. 連結相關會議與風險。
6. 驗證交付物。
7. 更新 Roadmap 與 Change Log。

## Validation

- 每個專案必須有目標。
- 每個任務必須有狀態。
- 每個交付物必須可檢查。
- 重大風險必須連結至 Risk Schema。
- 完成狀態不可在未驗證前標記完成。

## Failure Handling

- 範圍不明：標記 `SCOPE_UNCLEAR`。
- 任務過大：拆分為較小任務。
- 交付物缺失：標記 `DELIVERABLE_MISSING`。
- 進度衝突：以最新文件與決策為準。

## Future Expansion

- 可接 GitHub Issues。
- 可接 Automation 週期更新。
- 可接 Validator 檢查交付物。
- 可接 PPT Workflow 生成專案簡報。

## Examples

```markdown
# PM Status

## Milestone
M1 Governance Documents

## Status
In Progress

## Deliverables
- PROMPT_ENGINEERING_STANDARD.md
- OUTPUT_RULES.md
- VALIDATION_RULES.md
- AI_MEMORY_RULES.md
```
