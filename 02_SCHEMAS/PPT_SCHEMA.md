# PPT_SCHEMA

## Purpose

定義 PPT Generation（簡報生成）的標準資料結構，支援從知識庫、專案與會議資料產生簡報內容。

## Scope

適用於專案簡報、會議簡報、客戶簡報、策略簡報與知識摘要簡報。

## Input

- Presentation Title
- Audience
- Objective
- Source Materials
- Slide Outline
- Key Messages
- Data References
- Visual Requirements

## Output

- 標準化簡報需求文件
- Slide Outline
- Slide Content Draft
- 資料來源清單
- 可供未來 PPT Automation 使用的輸入

## Workflow

1. 定義簡報目的。
2. 定義受眾。
3. 收集來源資料。
4. 建立大綱。
5. 定義每頁重點訊息。
6. 標記資料來源。
7. 產出草稿並驗證一致性。

## Validation

- Title 不可空白。
- Audience 必須明確。
- 每張投影片必須有 Key Message。
- 引用資料必須可追蹤來源。
- 不可產生未經來源支持的數據或結論。

## Failure Handling

- 缺少資料來源：標記 `SOURCE_REQUIRED`。
- 受眾不明：標記 `AUDIENCE_UNCLEAR`。
- Slide 目的不明：合併或移除該 Slide 草稿。
- 結論無依據：標記 `EVIDENCE_MISSING`。

## Future Expansion

- 可接 PowerPoint 產生器。
- 可接 Project Schema。
- 可接 Knowledge Retrieval Workflow。
- 可接圖表與資料驗證流程。

## Examples

```markdown
# AI_OS_V2_INTRO_PPT

## Audience
System Owner

## Objective
說明 AI OS V2 架構、治理規則與下一步建置計畫。

## Slides
- 1: System Purpose
- 2: Architecture
- 3: Governance Rules
- 4: Roadmap
```
