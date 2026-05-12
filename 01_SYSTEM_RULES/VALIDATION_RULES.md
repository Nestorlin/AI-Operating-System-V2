# VALIDATION_RULES

## Purpose

定義 AI OS V2 的驗證規則，確保文件、Schema、Workflow 與 AI 輸出可被人工與未來 Validator 檢查。

## Scope

適用於所有系統文件、知識文件、Schema、Workflow、Prompt、AI Memory 與自動化輸出。

## Input

- 待驗證文件
- 文件所在路徑
- 文件命名
- 文件內容區塊
- 對應 Schema 或 Workflow

## Output

- 驗證通過結果
- 驗證失敗清單
- 修正建議
- 可供未來 Python Validator 使用的檢查邏輯

## Workflow

1. 檢查檔名是否為 `UPPER_SNAKE_CASE.md`。
2. 檢查文件是否位於正確資料夾。
3. 檢查是否包含標準九大區塊。
4. 檢查內容是否違反核心原則。
5. 檢查是否引用不存在的系統能力。
6. 檢查是否與既有 Schema 衝突。
7. 輸出驗證結果。

## Validation

- 文件不可為空。
- 文件不可只包含標題。
- 文件不可使用不一致命名。
- 文件不可聲稱已存在尚未實作的 Automation、Validator 或 Local LLM。
- 文件必須保留未來擴展接口，但不可假裝已完成。

## Failure Handling

- 命名錯誤：新增正確命名文件並保留原檔。
- 區塊缺失：補齊缺失區塊。
- Schema 衝突：以現有 Schema 為準，標記衝突。
- 架構不明：停止新增孤立文件，先補充設計文件。

## Future Expansion

- 建立 `VALIDATOR_DESIGN.md`。
- 建立 Python 驗證器。
- 支援 CI 檢查。
- 支援 Obsidian 外掛或命令列檢查。

## Examples

```text
STATUS: FAILED
FILE: OUTPUT_RULES.md
ISSUE: Missing Failure Handling section
ACTION: Add required section
```
