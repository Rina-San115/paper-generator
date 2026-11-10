# AGENTS.md - National Science Fair & Academic Report Guidelines

本文件為「科展標準作業報告網頁與 Word 自動生成專案」的 AI 協作開發與內容生成規範。
當 AI 被要求協助撰寫新報告、修改網頁內容或處理匯出邏輯時，必須嚴格遵守以下所有規則。

---

## 1. 專案目的 (Project Purpose)
建立一個標準化的學術與科展報告網頁展示與生成系統。使用者提供主題與參考文獻後：
1. 由 AI 依照科展格式與學術筆調生成報告內文。
2. 網頁呈現採用粉淺藍至湛藍的漸層學術美學。
3. 支援一鍵動態匯出符合排版規範的 Word 檔 (.docx)。

---

## 2. 內容與章節結構規範 (Content Architecture)

### A. 大寫數字大綱階層 (Mandatory Chapter Titles)
報告的主要大標題必須嚴格使用「大寫中文數字（壹、貳、參...）」，不得使用小寫數字：
- **壹、 封面與 basic 資訊** (Cover Page)
- **貳、 摘要與目錄** (Abstract & Table of Contents)
- **參、 研究動機與目的** (Motivation & Objectives)
- **肆、 研究過程與方法** (Process & Methodology)
- **伍、 研究結果、討論與心得** (Results, Discussion & Reflection)
- **陸、 參考資料** (References - APA 7th 格式)

### B. 條列與段落縮排規範 (Typography Rules)
- **段落縮排**：正文每一段開頭必須嚴格加上兩個全形空白（`  `）。
- **條列階層順序**：
  一、 大項目（半形/全形數字小寫）
  (一) 中項目
  1. 小項目
  (1) 細項
- **文風與語氣**：採用大學生專業學術筆調，嚴謹、客觀且流暢。**嚴禁使用 AI 罐頭語氣**（如：「總而言之」、「值得注意的是」、「首先...其次...最後」等）。

---

## 3. 多輪修正與文獻消化規則 (Iterative Refinement Rules)
1. **文獻融入**：若使用者提供參考文獻，AI 須深度消化並於內文進行適當引用（In-text citation）。
2. **對話重寫**：當使用者提出修正指令時，AI 僅調整指定章節，且重寫後的版本必須持續維持大寫數字標題（壹、貳...）、全形縮排與無 AI 罐頭感的學術語氣。

---

## 4. UI 視覺與 Word 匯出規範 (UI & Export Specs)

### A. 網頁漸層視覺 (Color Scheme)
- **整體背景**：採用自頂向下的垂直漸層，由柔和粉淺藍 transition 至深邃湛藍（`linear-gradient(180deg, #e0f2fe 0%, #bae6fd 35%, #0284c7 70%, #0369a1 100%)`）。
- **閱讀卡片**：採用高質感半透明白底（`rgba(255, 255, 255, 0.95)`），確保極佳閱讀體驗。

### B. Word 文件匯出功能 (.docx Export)
- 前端與腳本必須包含一鍵匯出 Word 功能。
- 匯出的 Word 文件必須完整保留大寫章節標題（壹、貳、參...）、內文首行縮排 2 字元與 APA 參考資料格式。