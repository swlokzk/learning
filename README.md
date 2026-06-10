# Learning

這是一個學習用的 monorepo，收錄並保留多個來源（GitHub Skills、個人筆記、課程練習）的原始 commit 歷史，便於集中管理、展示與備份。

## 專案結構

- `github/`
	- `github/github-skills/`：GitHub Skills 類型的專案集合，使用 `git subtree` 保留來源 repo 的歷史並放在此目錄下。
- `coursera/`：課程筆記與練習（例如 `coursera/genai-with-llm/`）。
- `cpttm/`：CPTTM 的各項練習或實作子專案。

## 使用與貢獻要點

- 保留來源歷史：對於外部 repo（例如 GitHub Skills、個人筆記庫），採用 `git subtree` 或 `git subtree split` 將來源匯入到對應子目錄，以保留原始 commit 歷史。
- 新內容維護：匯入後的內容請直接在本 `learning` repo 中維護與更新；不再回寫到來源 repo（若需同步請事先規劃）。
- 命名原則：來源類專案統一放到 `github/github-skills/`，課程相關放到 `coursera/`，若為特定專案請使用短而具辨識度的資料夾名。
