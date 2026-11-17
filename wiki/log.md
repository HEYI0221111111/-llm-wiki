---
title: 操作紀錄
type: log
---

# 操作紀錄

> 只能往後追加，不可改寫。標題格式：`## [YYYY-MM-DD] 操作類型 | 標題`
> 查看最近紀錄：`grep "^## \[" wiki/log.md | tail -5`

## [2026-11-17] schema | 建立知識庫
- 建立 AGENTS.md、資料夾結構、頁面範本與 tools/lint.py
- 尚未收錄任何資料

## [2026-11-17] ingest | 以人工智慧支援之協作式虛擬實境提升實用英語溝通能力
- 來源：raw/papers/以人工智慧支援之協作式虛擬實境提升實用英語溝通能力.pdf（2026 屏大碩論，60 頁，全文讀畢）
- 新建：[[以人工智慧支援之協作式虛擬實境提升實用英語溝通能力]]、[[Collaborative Virtual Reality]]、[[Self-Determination Theory]]、[[Foreign Language Anxiety]]、[[STT-LLM-TTS Pipeline]]、[[Lag Sequential Analysis]]、[[LLM 作為語言學習對話夥伴]]、[[AI 虛擬面試官的系統與評估設計]]
- 更新：[[index]]、[[overview]]（首次填寫研究焦點與資料缺口）
- 備註：論文的「CVR 累積語言產出較高」換算成人均後不成立（CVR 每人 211 字，VR 每人 239 字），已寫入論文頁的限制段落；文獻回顧中的二手引用已標註待查證

## [2026-11-17] web | 建立瀏覽網站 v1
- 新增 web/AGENTS.md（網站規格書）、web/build.py、web/md.py、web/static/
- 網站輸出到 docs/：首頁、全部條目、分類頁、條目頁、標籤頁、紀錄頁、全文搜尋、反向連結、深淺色模式、手機版面
- 根目錄 AGENTS.md 新增第 12 節「瀏覽網站」
