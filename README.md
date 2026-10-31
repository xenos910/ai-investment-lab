# AI 智能投資任務實驗室

以 https://ai-investment-quest-lab-new.vercel.app/ 的可見版面及學習架構為參考，獨立重建的繁體中文互動教材入口。任務細節與完成檢核為本專案撰寫；非原站原始碼複製。

## 功能

- 藍紫漸層首頁與自適應手機版面
- 六項任務地圖、任務切換與可展開教材
- 可複製 Prompt、Google Colab 入口
- 以瀏覽器 localStorage 保存完成檢核
- 五題小測驗、答案解釋、計分與重設
- 無套件、無建置程序、無外部字型依賴

## 本機執行

直接開啟 `index.html`，或在專案目錄執行：

```sh
python -m http.server 8000
```

瀏覽 http://localhost:8000 。剪貼簿複製需 HTTPS 或 localhost；若權限受限可手動複製文字。

## 部署

可將本儲存庫匯入 Vercel，選擇 Other，無需 Build Command，Output Directory 使用根目錄 `.`。也可使用任何靜態網站主機。

如使用 GitHub Pages，請在儲存庫 Settings → Pages 選擇從 `main` 的根目錄發布。私人儲存庫是否支援 Pages 取決於 GitHub 方案；請先確認網站的公開存取設定。

## 檔案

- `index.html`：頁面結構
- `style.css`：視覺與響應式版面
- `app.js`：任務內容與互動功能

## 範圍

本版本是互動教材入口，未串接股價 API、Gemini、Python 回測或交易服務。首頁進度百分比依參考畫面呈現，為示意值；完成檢核獨立保存在本機瀏覽器。

請勿在前端或 GitHub 提交 API 金鑰。後續若擴充實際分析功能，需使用獨立 Python / Streamlit 後端並以 Secrets 管理金鑰。
