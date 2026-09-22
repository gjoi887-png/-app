# 測量案件時間表 App

GitHub Pages-ready 的靜態網頁 App，提供：

- 新增案件：收件日、測量日期、案號、地號、界指點數、案件分類、備註
- 案件清單與月曆檢視
- 鑑界、分割合併、建物案件、法院案件分類
- 測量日前兩天的提醒標示（09:00 台北時間的提醒規則）
- 瀏覽器 localStorage 儲存資料
- CSV 匯出

## GitHub Pages

1. 將本資料夾上傳到 GitHub repository。
2. Repository → **Settings** → **Pages**。
3. Source 選 **Deploy from a branch**，選 `main` / `/root`。
4. 儲存後即可使用 GitHub Pages 網址。

目前版本是前端獨立版，資料儲存在使用者瀏覽器。若要與 Notion 資料庫雙向同步，需要再接 Notion API 的安全後端或 GitHub Actions；不要把 Notion token 直接放在前端。

## PWA

此版本已加入 PWA：可安裝到手機或桌面、支援 standalone 顯示，並快取主要 App 資源以支援離線開啟。GitHub Pages 會自動以 HTTPS 提供 Service Worker 所需的安全環境。
