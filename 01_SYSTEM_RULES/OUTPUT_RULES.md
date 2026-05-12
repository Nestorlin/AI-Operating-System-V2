# OUTPUT_RULES

## Purpose

定義 AI OS V2 的輸出規則，確保所有文件與回應具備一致格式、可維護性與可驗證性。

## Scope

適用於工程文件、Schema 文件、Workflow 文件、AI 回應、Automation 輸出與知識庫條目。

## Input

- 任務指令
- 文件類型
- 既有命名規範
- 既有資料夾架構
- 必要 Schema 或 Workflow

## Output

- Obsidian 友善 Markdown
- GitHub 友善 Markdown
- 結構化工程文件
- 可被 AI 檢索與驗證的內容

## Workflow

1. 判斷輸出文件類型。
2. 使用 `UPPER_SNAKE_CASE.md` 命名。
3. 使用清楚標題與短段落。
4. 必須包含標準九大區塊。
5. 避免 HTML 與複雜巢狀。
6. 優先使用中文。
7. 英文術語如需保留，後方補中文說明。

## Validation

每份正式文件必須包含：

- Purpose
- Scope
- Input
- Output
- Workflow
- Validation
- Failure Handling
- Future Expansion
- Examples

## Failure Handling

- 若缺少必要區塊，文件視為不完整。
- 若命名不符合規範，必須新增正確命名版本，不可刪除舊檔。
- 若輸出與既有架構衝突，必須停止擴張並回到核心架構。

## Future Expansion

- 可建立 Markdown Linter。
- 可建立 Schema-based Output Validator。
- 可由 Automation 檢查文件完整性。
- 可支援多語輸出策略。

## Examples

```text
MEETING_SCHEMA.md
PPT_WORKFLOW.md
VALIDATION_RULES.md
```
