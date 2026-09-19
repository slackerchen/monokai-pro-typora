# Monokai Pro (CE) for Typora

以 [Monokai Pro](https://monokai.pro/) 預設配色為基礎、由本專案貢獻者獨立維護的 Typora Community Edition。採用暖灰底色、柔白文字與六色語法高亮，適合中文、英文及程式碼混合的筆記。

本專案並非 Monokai 官方產品，也不代表已獲官方收錄或認證。

[安裝說明](INSTALL.md) · [示範 Markdown](monokai-pro-specimen.md) · [MIT 授權](LICENSE.md) · [來源與發布範圍](NOTICE.md)

## 特色

- **單檔安裝、離線使用**：不載入網路字型、JavaScript 或其他外部資源。
- **中英混排**：預設 16px 正文、1.8 倍行高，搭配系統字型與繁體中文 fallback。
- **一致的編輯配色**：包含程式碼區塊、Markdown 原始碼模式、大綱側欄、搜尋與選取狀態。
- **常用 Markdown 元素**：表格、引述、工作清單、註腳、目錄與五種提示類型。
- **公式與圖表**：長公式可在區塊內水平捲動；Mermaid 採用深色主題並保留作者指定的色彩。
- **響應式留白**：依視窗寬度調整邊距，保持正文可讀性。
- **列印樣式**：提供白底與深色語法配色；原生 PDF 分頁尚待驗證。

## 快速開始

1. 下載 [monokai-pro.css](monokai-pro.css)。
2. 在 Typora 的 **偏好設定／設定 → 外觀 → 開啟主題資料夾**，放入該 CSS。
3. 重新啟動 Typora，選擇 **Themes → Monokai Pro**。
4. 開啟 [monokai-pro-specimen.md](monokai-pro-specimen.md) 查看各種 Markdown 元素。

專案公開名稱為 **Monokai Pro (CE) for Typora**；為維持安裝相容性，CSS 檔名仍為 `monokai-pro.css`，因此 Typora 選單會顯示 **Monokai Pro**。

## 相容性與已知限制

目前的驗證基準是 **macOS / Typora 1.14.10**（2026-09-13），涵蓋正文、中英混排、大綱、程式碼、原始碼模式、表格、工作清單、提示、公式及 Mermaid。HTML 輸出曾以 320px 與 390px 寬度檢查。

- Windows 與 Linux 尚未實機驗證。
- 列印 CSS 已檢查，但尚未完成本主題的原生 PDF 分頁驗證。Typora 若指定其他 PDF 匯出主題，會使用該主題的樣式。
- macOS 原生分頁、選單及系統對話框不受主題 CSS 完整控制。
- CodeMirror 的語法分類依各語言模式而異，不等同於 VS Code 的語意高亮。
- Mermaid 使用 Typora 提供的深色渲染；明確指定的 `classDef` 或作者配色會保留。

## 自訂

在主題資料夾建立 `monokai-pro.user.css`，例如：

```css
:root {
    --mp-page-width: 960px;
    --mp-code-font: "JetBrains Mono", Menlo, Consolas, monospace;
}

html { font-size: 17px; }
```

指定字型需自行安裝。Typora 的字型與字級偏好設定可能覆蓋主題預設。

## 專案內容

| 檔案 | 用途 |
| --- | --- |
| `monokai-pro.css` | 主題樣式 |
| `monokai-pro-specimen.md` | 示範與手動檢查文件 |
| `INSTALL.md` | 安裝、更新與移除說明 |
| `LICENSE.md` | 依官方 CE 模板保留的 MIT 授權 |
| `NOTICE.md` | 來源、CE 發布規則與第三方內容範圍 |
| `CONTRIBUTING.md` | 問題回報、修改與 CE 提交流程 |

發布內容不包含其他作者的參考主題、舊版 CSS、開發紀錄或產生的 HTML/PDF。HTML 匯出包含額外的第三方樣式及渲染內容，其再散布授權仍待另行核對。

## 授權與致謝

本專案依 [Monokai Pro Community Edition 官方模板](https://github.com/monokai-pro/community-edition) 整理，採用模板的 [MIT 授權](LICENSE.md)，並保留原有著作權聲明。

Monokai Pro 原始配色及品牌歸 Monokai 所有。CE 的命名、適用平台、預設 filter、免費非商業發布及套件接手等規則，請參閱 [官方 CE 說明](https://monokai.pro/contribute) 與 [NOTICE.md](NOTICE.md)。本專案僅包含預設配色的 Typora 實作，未包含官方付費擴充套件或圖示包。

更多支援的應用程式：[Monokai Pro](https://monokai.pro/)。
