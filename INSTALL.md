# 安裝 Monokai Pro (CE) for Typora

## 安裝

1. 下載本專案的 [`monokai-pro.css`](monokai-pro.css)。如果從 GitHub 檔案頁下載，請使用 **Download raw file**，避免將網頁存成 CSS。
2. 開啟 Typora 的 **偏好設定／設定 → 外觀 → 開啟主題資料夾**。
3. 將 CSS 檔案放入主題資料夾，不需要複製整個專案。
4. 重新啟動 Typora。
5. 在 **Themes／主題 → Monokai Pro** 選用。

選單名稱來自 `monokai-pro.css` 的檔名。專案完整名稱為 **Monokai Pro (CE) for Typora**。

## 查看效果

使用 Typora 開啟 [`monokai-pro-specimen.md`](monokai-pro-specimen.md)。數學公式、圖表與部分擴充語法的呈現，取決於 Typora 的版本及 Markdown 偏好設定。

## 更新

備份自行修改的 CSS，然後以新版 `monokai-pro.css` 取代主題資料夾中的同名檔案。重新啟動 Typora 以確保載入新版本。

建議將個人調整放在 `monokai-pro.user.css`，以便更新時保留。

## PDF 與列印

若 PDF 外觀與編輯器不同，檢查 **偏好設定 → 匯出 → PDF → 主題** 是否指定了另一套主題。選擇目前主題或 Monokai Pro，才能使用本主題的列印 CSS。

白底列印規則已進行樣式檢查；原生 PDF 分頁尚未完成驗證，匯出後請檢查長程式碼、表格和圖表。

## 移除

先切換至其他主題，再移除主題資料夾中的 `monokai-pro.css`。如有建立 `monokai-pro.user.css`，可一併移除或自行保留。重新啟動 Typora 更新主題選單。

官方參考：[Typora — About Themes](https://support.typora.io/About-Themes/)。
