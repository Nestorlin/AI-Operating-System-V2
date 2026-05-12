# LOCAL_LLM_STRATEGY

## Purpose

規劃未來 Ollama 或其他本地模型的使用邊界，支援隱私、檢索、摘要與輔助分析。

## System Role

定義 Local LLM 在 AI OS V2 中的定位，避免把本地模型當成不可控核心依賴。

## Input

- 本地 Markdown 文件
- 使用者查詢
- 可用模型
- 硬體限制
- Context 限制

## Output

- Local LLM 使用策略
- 模型選擇原則
- 任務分工
- 限制清單

## Workflow

1. 判斷任務是否適合本地模型。
2. 本地模型先做檢索、摘要或分類。
3. 高風險決策交由 GPT 或人工確認。
4. 保留來源與不確定性。
5. 避免把模型輸出直接寫入核心文件。

## Validation

- 必須使用 Markdown 作為主要格式。
- 必須保持人類可讀與 AI 可讀。
- 不可宣稱尚未實作的功能已經可用。
- 不可依賴 SaaS 或外部 API 作為核心流程。
- 命名必須符合 UPPER_SNAKE_CASE.md。

## Failure Handling

- 資料不足時，輸出缺口清單。
- 來源衝突時，保留來源並標記衝突。
- 格式不一致時，先標記待整理，不直接覆蓋。
- 流程無法完成時，輸出可人工執行的替代步驟。

## Future Expansion

- 接 Ollama。
- 接本地 Embedding。
- 接混合式 AI 架構。
- 接模型效能評估。

## Examples

``markdown
Local LLM Task: 摘要 20 份會議紀錄`nGPT Task: 根據摘要做高階推理與文件產出
``
