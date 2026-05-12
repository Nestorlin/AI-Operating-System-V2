# ROLE（角色）

定義AI扮演角色。

例如：
- AI PM
- AI System Architect
- AI Documentation Engineer
- AI Validator
- AI Workflow Designer

---

# OBJECTIVE（目標）

定義本次任務目標。

必須：
- 明確
- 可驗證
- 可輸出

避免模糊敘述。

---

# INPUT（輸入資料）

定義：
- 來源資料
- 格式
- 限制
- 上下文

例如：
- Markdown
- Meeting Notes
- JSON
- PDF解析內容

---

# SYSTEM CONTEXT（系統上下文）

定義：
- AI OS規則
- Workflow
- Schema
- Governance
- 命名規範

AI不得脫離系統規則。

---

# CONSTRAINTS（限制條件）

定義：
- 禁止事項
- 輸出限制
- 安全限制
- 格式限制

例如：
- 禁止Markdown外輸出
- 禁止推測不存在資訊
- 禁止破壞Schema

---

# OUTPUT FORMAT（輸出格式）

定義：
- JSON
- Markdown
- YAML
- 表格
- 特定Schema

必須固定格式。

---

# VALIDATION RULES（驗證規則）

AI輸出前必須檢查：

- 是否符合Schema
- 是否缺欄位
- 是否格式錯誤
- 是否有幻覺內容（Hallucination）

---

# FAILURE HANDLING（失敗處理）

當資料不足時：

AI必須：
- 明確指出缺失
- 禁止幻想補全
- 要求補充資料

---

# EXAMPLES（範例）

提供：
- 正確案例
- 錯誤案例

提升模型穩定性。

---

# FINAL CHECKLIST（最終檢查）

AI輸出前檢查：

- Schema正確
- 命名正確
- 格式正確
- 無多餘解釋
- 可直接進入Workflow