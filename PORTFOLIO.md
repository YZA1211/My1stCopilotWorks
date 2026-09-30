![工作坊完成徽章](https://img.shields.io/badge/GitHub_Copilot_實戰工作坊-已完成-1F883D?style=for-the-badge&logo=githubcopilot&logoColor=white)

# 待辦清單 Web App

這是一個在 GitHub Copilot 實戰工作坊中完成的純前端待辦清單應用程式。專案以 HTML、CSS 與原生 JavaScript 實作，支援待辦管理、篩選與深色模式，並以瀏覽器 `localStorage` 保存資料。

## 線上展示

[https://yza1211.github.io/My1stCopilotWorks/](https://yza1211.github.io/My1stCopilotWorks/)

> GitHub Pages 已設定從 `main` 分支的 `/(root)` 發佈。首次部署進行中，請稍後確認上方網址。

## 功能

- 新增待辦事項，並忽略空白內容。
- 勾選完成或取消完成；已完成項目會加上刪除線並淡化。
- 刪除單筆待辦事項。
- 顯示整份清單的未完成數量，不受目前篩選條件影響。
- 依全部、未完成或已完成篩選待辦，並在篩選結果為空時顯示提示。
- 切換淺色與深色模式；手動偏好會保存，未選擇時跟隨作業系統設定。
- 使用 `localStorage` 保存待辦與主題偏好，重新整理後仍可保留。
- 置中卡片版面，支援手機螢幕。

## 技術

- HTML、CSS、原生 JavaScript。
- 不使用框架、套件或外部 CDN；不需要建置流程。
- 使用 CSS 變數管理深淺色配色，使用 `prefers-color-scheme` 讀取系統主題偏好。
- 使用瀏覽器 `localStorage` 保存資料與主題選擇。

## 開發方式

- 使用 GitHub Copilot Agent Mode 根據需求建立並擴充待辦清單介面與功能。
- 在 `.vscode/mcp.json` 設定 Microsoft Learn 與 GitHub MCP Server；伺服器啟動及工具呼叫尚未在本工作階段驗證。
- 建立 `.github/copilot-instructions.md` 專案規範，以及 `.github/prompts/fix-issue.prompt.md` issue 修復劇本。
- 劇本定義了讀取 issue、提出計畫、等待確認、修改、驗證、提交及建立 PR 的流程；目前尚未用它完成 issue 修復或建立 PR。

## 我學到什麼

- 清楚描述需求與限制，有助於 Agent 一次處理多個相關檔案。
- 讓 AI 修改程式後，仍要透過瀏覽器操作與測試確認行為。
- MCP 需要設定、啟動與授權，才能讓 AI 使用外部服務工具。
- 將重複流程寫成 repo 內的 prompt，能讓流程可重複執行與版本管理。
- Git 提交與還原檢查點能保留可回復的工作版本。
