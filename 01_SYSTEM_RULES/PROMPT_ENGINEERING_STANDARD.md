# PROMPT_ENGINEERING_STANDARD

## Purpose

定義 AI Operating System V2 的提示工程標準，確保 AI 指令可讀、可追蹤、可驗證、可長期維護。

## Scope

適用於所有交給 AI、Local LLM、Automation、Validator 使用的 Prompt 文件與任務指令。

## Input

- 使用者需求
- 系統目標
- 既有 Schema
- 既有 Workflow
- 專案上下文

## Output

- 結構化 Prompt
- 可驗證任務描述
- 明確輸入與輸出定義
- 可供未來自動化執行的指令格式

## Workflow

1. 確認任務目的。
2. 確認任務範圍。
3. 指定必要輸入。
4. 指定預期輸出。
5. 指定限制條件。
6. 指定驗證方式。
7. 指定失敗處理方式。
8. 保持命名與既有架構一致。

## Validation

- Prompt 必須有明確目的。
- Prompt 必須說明輸入與輸出。
- Prompt 不可要求 AI 假設不存在資料。
- Prompt 不可繞過 Schema。
- Prompt 不可修改核心架構，除非任務明確要求。
- Prompt 必須可被人類與 AI 重新閱讀。

## Failure Handling

- 缺少輸入時，AI 必須列出缺口。
- Schema 不存在時，AI 不可自行幻想欄位。
- 任務範圍衝突時，優先遵守核心原則。
- 無法完成時，必須說明原因與可行替代方案。

## Future Expansion

- 可擴展為 Prompt Template Library。
- 可接 Local LLM 執行。
- 可接 Python Validator 檢查必要區塊。
- 可接 Automation 依任務類型選擇 Prompt。

## Examples

```markdown
# TASK_NAME

## Purpose
說明任務目的。

## Input
列出必要輸入。

## Output
列出預期輸出。

## Validation
列出驗證規則。
```
