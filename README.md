# AI Operating System V2

AI Operating System V2（AI 作業系統 V2）是一套以：

- AI Workflow（AI 工作流）
- Knowledge Management（知識管理）
- Retrieval System（檢索系統）
- Automation（自動化）
- Local LLM（本地大型語言模型）
- PM System（專案管理系統）

為核心的個人 AI 協作架構。

本系統的目標不是單一 AI 工具，而是：

建立一套：

「可長期維護、可擴展、可驗證、可移植」

的 AI Operating Layer（AI 作業層）。

---

# Current Status（目前狀態）

目前狀態：

```text
Architecture Documentation Skeleton Completed
```

代表：

- 系統架構文件已大量建立
- 主系統層級已完成規劃
- Workflow（工作流）與 System Boundaries（系統邊界）已定義

但：

```text
Runtime Implementation NOT Completed
```

目前尚未代表：

- Python Runtime（Python 執行系統）完成
- Ollama Integration（Ollama 整合）完成
- Vector Database（向量資料庫）完成
- RAG Pipeline（檢索增強生成管線）完成
- PPT Automation（簡報自動化）完成

---

# System Philosophy（系統理念）

本系統核心理念：

1. AI 必須可控
2. AI 必須可驗證
3. AI 必須可維護
4. AI 必須有上下文邊界
5. AI 必須避免 Context Pollution（上下文污染）
6. AI 必須與人類協作，而非完全取代

---

# Folder Structure（資料夾結構）

## 00_SYSTEM_CORE

系統核心定義。

包含：

- 系統定位
- 系統狀態
- 啟動規則
- AI Bootstrap（AI 啟動）規則

---

## 01_SYSTEM_RULES

AI 全域規則層。

包含：

- AI Runtime Constraints（AI 執行限制）
- Output Rules（輸出規則）
- Validation Rules（驗證規則）
- Memory Rules（記憶規則）

---

## 02_SCHEMAS

資料結構層。

包含：

- Meeting Schema（會議資料結構）
- Project Schema（專案資料結構）
- Task Schema（任務資料結構）

---

## 03_WORKFLOWS

工作流層。

包含：

- PM Workflow（PM 工作流）
- Meeting Workflow（會議工作流）
- PPT Workflow（簡報工作流）
- Retrieval Workflow（檢索工作流）

---

## 04_RETRIEVAL_SYSTEM

Knowledge Retrieval（知識檢索）架構。

包含：

- Obsidian Structure
- Retrieval Rules
- RAG Architecture
- Local Retrieval Strategy

---

## 05_AUTOMATION_CORE

Automation（自動化）核心。

包含：

- Python Automation
- Export Pipeline
- Prompt Pipeline
- Semi-Automation Rules

---

## 06_AI_MEMORY_SYSTEM

AI 記憶系統。

包含：

- Short-term Memory（短期記憶）
- Long-term Memory（長期記憶）
- Memory Validation（記憶驗證）
- Memory Priority（記憶優先級）

---

## 07_PRESENTATION_INTELLIGENCE

Presentation Intelligence（簡報智能）層。

包含：

- PPT Generation
- Canva Prompt Design
- Technical Presentation Rules

---

## 08_LOCAL_LLM_SYSTEM

Local LLM（本地大型語言模型）層。

包含：

- Ollama Architecture
- Embedding Strategy
- Vector Strategy
- Local RAG Pipeline

---

## 09_SYSTEM_VALIDATION

系統驗證層。

包含：

- Hallucination Prevention（幻覺防護）
- Workflow Validation（工作流驗證）
- Failure Recovery（失敗恢復）

---

## 10_EXPANSION_SYSTEM

未來擴展層。

包含：

- Multi-AI Collaboration（多 AI 協作）
- Plugin Architecture（插件架構）
- Future Agent Design（未來 Agent 設計）

---

## 11_SYSTEM_FINALIZATION

系統治理與維護層。

包含：

- Backup Strategy（備份策略）
- Deployment Guide（部署指南）
- Versioning Strategy（版本策略）
- Maintenance Rules（維護規則）

---

# Important Warning（重要警告）

本系統目前：

```text
是 Architecture Layer（架構層）
不是 Production Runtime（正式執行系統）
```

請勿誤判：

「文件存在」＝「功能已完成」。

---

# Recommended Reading Order（建議閱讀順序）

AI 或新協作者：

請依序閱讀：

1. README.md
2. 00_SYSTEM_CORE/AI_BOOTSTRAP_PROMPT.md
3. 00_SYSTEM_CORE/CURRENT_SYSTEM_STATUS.md
4. 01_SYSTEM_RULES/
5. 03_WORKFLOWS/
6. 04_RETRIEVAL_SYSTEM/
7. 05_AUTOMATION_CORE/

再開始實作或生成內容。

---

# Future Direction（未來方向）

下一階段：

```text
P12 — Alignment & Freeze
P13 — Real Runtime Implementation
```

重點：

- Python Runtime
- Obsidian Integration
- Ollama Integration
- Local RAG
- AI Memory Runtime
- PPT Automation Pipeline