# 2026 北京 QCon 參會心得網站

單頁靜態網站（`index.html`），介紹 2026 北京 QCon 全球軟體開發大會的參會心得。

- 收錄 77 場次：15 場親身參與（逐字稿＋YouTube 連結）、62 場官方講稿 PDF
- 互動式知識圖：依 14 個主題分類，點擊節點可連到 YouTube 或下載 PDF
- 心得段落可透過 `data-refs` 標註相關場次，自動產生連結卡片

## 維護方式

1. **補 YouTube 連結**：在 `index.html` 搜尋 `const DATA`，於對應場次的 `"yt": ""` 填入網址。
2. **寫心得**：在 `<main id="essay">` 內複製 `<section class="essay-block">` 範本，`data-refs` 填相關場次 id（如 `s02,s09`）。
3. PDF 檔放在 `PDF/`，檔名勿改。

## GitHub Pages 部署

Repo Settings → Pages → Source 選 `main` branch / root，儲存後網址為
`https://mjjackson0414.github.io/2026_QCon_Beijing/`

---
講稿 PDF 版權屬原講者與 QCon 主辦方，僅供學習交流。
