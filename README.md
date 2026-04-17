# Sentai Travel

這是一個純前端的靜態旅遊行程頁面，用來整理「2026 仙台馬拉松・東北之旅」的每日安排、航班資訊與天氣提醒。

目前專案以單一 `index.html` 組成，不需要安裝套件，也不需要建置流程，直接開啟即可使用。

## 功能特色

- 單頁式旅遊行程表
- 置頂日期切換 tab
- 航班資訊分組顯示
- 每日行程卡片整理
- Google Maps 導航連結
- 依日期切換的天氣預報提示
- 支援手機與桌機瀏覽

## 如何使用

1. 下載或 clone 這個專案
2. 直接用瀏覽器開啟 [index.html](/C:/Users/lillian.lo/PycharmProjects/sentai_travel/index.html)

也可以在專案資料夾中用任何靜態伺服器啟動，例如：

```powershell
# Python
python -m http.server 8000

# Node.js
npx serve .
```

啟動後，打開 `http://localhost:8000`

## 專案結構

```text
sentai_travel/
├─ index.html   # 主頁面，包含 HTML / CSS / JavaScript
└─ README.md    # 專案說明
```

## 可調整內容

如果你想修改內容，主要都在 `index.html`：

- 航班資訊：搜尋 `pane-flight`
- 每日行程：搜尋 `pane-day1` 到 `pane-day5`
- 天氣預報：搜尋 `weather-item`
- 主選單切換：搜尋 `switchMainTab`
- 天氣同步邏輯：搜尋 `syncWeather`

## 技術說明

- HTML5
- CSS3
- Vanilla JavaScript
- 無框架、無額外相依套件

## 適合部署方式

這個專案很適合部署到任何靜態網站服務，例如：

- GitHub Pages
- Netlify
- Vercel
- 任意可託管靜態檔案的空間

## 備註

目前天氣內容是整理後的旅遊參考資訊，不是即時 API 資料。如果之後要改成即時天氣，也可以再擴充。
