# 2026 北京 QCon 參會心得網站

單頁靜態網站（`index.html`），分享 2026 北京 QCon 全球軟體開發大會的參會心得。

線上網址：https://mjjackson0414.github.io/2026_QCon_Beijing/

## 專案結構

- `index.html`：整個網站（HTML＋CSS＋JS＋場次資料都在這一個檔案）
- `PDF/`：72 份講師公開講稿（檔名勿改，網站連結依檔名對應）
- `assets/`：心得插畫圖片放這裡（`<img src="assets/xxx.png">`）
- `slide picture/`：段落配圖。放入「與段落標題同名」的 PNG（如 `AI Coding 對企業的影響：流水線的困境.png`），該段右側會自動以圖片取代 SVG 概念圖，無需改程式
- `會議分類整理.md`：77 場次的主題分類與對應表（參考用）
- `會議逐字稿/`：15 場親身參加場次的逐字稿（16 篇，校正版）
- `2026北京QCon心得.txt`：心得原稿

## 在其他電腦接續工作

```bash
git clone https://github.com/MJJackson0414/2026_QCon_Beijing.git
```

直接用瀏覽器開 `index.html` 即可本地預覽（無需伺服器）。

## 維護方式

1. **寫心得**：編輯 `index.html` 的 `<main id="essay">` 區，複製一個
   `<section class="essay-block">` 即可新增段落。
   - `.txt` 放文字（`<br>` 斷行、`<div class="callout">` 為重點縮排卡）
   - `.figside` 的 `<figure>` 放 SVG 概念圖或 `<img src="assets/xxx.png">`
   - `data-refs` 填相關場次 id（如 `s02,s08`），段落底部自動產生連結卡
2. **補 YouTube 連結**：搜尋 `const DATA`，在對應場次的 `"yt": ""` 填入網址（★ 的 15 場）
3. **推版**：commit 後 push 到 `main`，GitHub Pages 會自動重新部署
4. **流量統計**：GoatCounter 儀表板在 https://mjjackson.goatcounter.com/（追蹤碼已嵌在 `index.html` 底部）

## 待辦

- [x] 15 場親身參加場次的 YouTube 連結（已補齊，含上下半場共 24 部）
- [x] 心得全文（四大部分、含五個綜合觀察與結語）
- [ ] 感想類段落的插畫（`assets/`）

---
講稿 PDF 版權屬原講者與 QCon 主辦方，僅供學習交流。
