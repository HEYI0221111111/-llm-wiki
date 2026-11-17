# LLM 研究 Wiki

以 Karpathy 的 LLM Wiki 模式建立的 LLM 研究知識庫：你負責收集資料、提出問題，AI agent 負責把資料整理成互相連結的 Markdown wiki。

## 快速開始

1. 把論文、文章、筆記放進 `raw/` 底下對應的資料夾。
2. 在本資料夾開啟 Claude Code（或其他 agent），它會自動讀 `CLAUDE.md` → `AGENTS.md`。
3. 對 agent 說：
   - `ingest raw/papers/某篇論文.md`：收錄一份資料
   - `query：DPO 和 RLHF 的主要差異是什麼？`：用 wiki 回答問題
   - `lint`：檢查矛盾、斷鏈、孤兒頁
   - `status`：查看 wiki 狀態
4. 用網頁瀏覽：執行 `python web/build.py`，再雙擊 `docs/index.html`。
5. 也可以用 Obsidian 開啟本資料夾，即時瀏覽 wiki 與關聯圖。

## 資料夾

- `raw/`：原始資料（agent 只讀不改）
- `wiki/`：agent 維護的知識庫，入口是 `wiki/index.md` 與 `wiki/overview.md`
- `templates/`：各類頁面範本
- `tools/lint.py`：檢查斷鏈、孤兒頁，並產生 `wiki/_backlinks.json`
- `web/`：瀏覽網站的原始碼與規格書（[web/AGENTS.md](./web/AGENTS.md)）
- `docs/`：產生出來的網站（GitHub Pages 從這裡發布）

完整規則見 [AGENTS.md](./AGENTS.md)。
