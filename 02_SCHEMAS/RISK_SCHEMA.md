# RISK_SCHEMA

## Purpose

定義 Risk Management（風險管理）的標準資料結構，支援風險辨識、評估、處理與追蹤。

## Scope

適用於技術風險、架構風險、資料風險、流程風險、交付風險與維護風險。

## Input

- Risk ID
- Risk Title
- Description
- Category
- Probability
- Impact
- Severity
- Owner
- Mitigation
- Status

## Output

- 標準化風險紀錄
- 風險等級
- 緩解方案
- 追蹤狀態
- 專案與會議可引用的風險資料

## Workflow

1. 記錄風險來源。
2. 分類風險。
3. 評估發生機率。
4. 評估影響程度。
5. 指定處理方式。
6. 定期更新狀態。

## Validation

- Risk ID 不可重複。
- Probability 必須為 `Low`、`Medium`、`High`。
- Impact 必須為 `Low`、`Medium`、`High`。
- Status 必須為 `Open`、`Monitoring`、`Mitigated`、`Closed`。
- Mitigation 不可空白，除非 Status 為 `Closed`。

## Failure Handling

- 缺少風險描述：標記 `DESCRIPTION_REQUIRED`。
- 無法評估等級：標記 `ASSESSMENT_PENDING`。
- 無 Owner：標記 `UNASSIGNED`。
- 風險已失效：標記 `Closed` 並保留紀錄。

## Future Expansion

- 可接 Project Schema。
- 可接 Meeting Schema。
- 可接 Automation 定期提醒。
- 可接 Validator 檢查風險欄位完整性。

## Examples

```markdown
# RISK_SCHEMA_CONFLICT

## Category
Architecture

## Probability
Medium

## Impact
High

## Mitigation
所有新增文件必須先檢查既有架構與命名規範。
```
