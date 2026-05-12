# PROJECT_SCHEMA

## Purpose

定義 PM Management（專案管理）的標準資料結構，支援單人與 AI 協作的專案追蹤。

## Scope

適用於專案目標、里程碑、任務、狀態、依賴、風險、決策與交付物管理。

## Input

- Project ID
- Project Name
- Objective
- Scope
- Milestones
- Tasks
- Owners
- Status
- Risks
- Deliverables

## Output

- 標準化專案文件
- 任務清單
- 里程碑狀態
- 風險連結
- 可供 AI 檢索與 Automation 使用的專案上下文

## Workflow

1. 建立專案基本資料。
2. 定義專案目標與範圍。
3. 拆分里程碑。
4. 拆分任務。
5. 連結風險與依賴。
6. 更新狀態與版本紀錄。

## Validation

- Project ID 不可空白。
- Objective 必須清楚。
- 任務必須有狀態。
- 里程碑必須可驗證。
- 風險必須連結至 `RISK_SCHEMA.md` 格式。

## Failure Handling

- 目標不清：標記 `OBJECTIVE_UNCLEAR`。
- 任務無負責人：標記 `UNASSIGNED`。
- 依賴不明：標記 `DEPENDENCY_UNKNOWN`。
- 狀態衝突：以最新日期紀錄為準，保留歷史。

## Future Expansion

- 可接 GitHub Issues。
- 可接 Automation 排程檢查。
- 可接 Risk Management。
- 可接 PPT Generation 產出專案簡報。

## Examples

```markdown
# PROJECT_AI_OS_V2

## Objective
建立長期可維護的 AI PM 與知識系統。

## Status
Active

## Milestones
- M1: Governance Documents
- M2: Schemas
- M3: Workflows
```
