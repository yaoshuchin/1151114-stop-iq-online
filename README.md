# STOP麥擱騙! 我智商在線 · 研習數位典藏鏡像站

本專案為「**STOP麥擱騙! 我智商在線**」研習看板之高保真、離線本機典藏平台，提供完整的教材鏡像、活動歷程、查核遊戲及學員作品典藏。

---

## 📌 專案特點與架構

1. **圖片與檔案直接下載複製 (100% 離線可用，絕無外部 Padlet 依賴)**
   - **全面剔除外部 Padlet 轉址**：移除所有跳轉回 Padlet 的作者個版連結與 Wish 網址，全部改為本地資源直接讀取與下載。
   - **卡片直覺下載**：每張看板卡片與詳情彈窗均具備「📥 下載原圖」、「🔍 檢視」按鈕，學員可一鍵將 28 份高解析實體原檔儲存至本機。
   - **3 套互動測驗與遊戲免聯網本機執行**：
     - `assets/games/246game.html`（2-4-6 認知實驗系統，含本機截圖庫）
     - `assets/games/mygopen-test.html`（防詐查核線上測驗題庫版 · 4.03 MB）
     - `assets/games/case072.html`（情境模擬查核解謎系統 · 4.68 MB）
   - **李宜玲老師精闢講義離線雙格式**：HTML 網頁版 + Markdown 原始文檔 + 14 份教學圖表（`./assets/lectures/images/`）。
   - **第 4 節課堂實作操作影片**：`assets/lectures/SS練習.mp4`（1.68 MB，MP4 視訊實體收錄）。
   - **兩大全量一鍵打包禮包**：
     - `assets/exports/padlet_full_offline_bundle.zip`（24.35 MB，全站離線旗艦大禮包）
     - `assets/exports/padlet_images_all.zip`（12.28 MB，全板高解析圖片包）

2. **門禁防護安全規範**
   - 採用瀏覽器原生 **Web Crypto API** (`crypto.subtle.digest('SHA-256')`) 進行研習專屬內部驗證。
   - 前端程式碼與文檔中零明文儲存，嚴格保護教學智慧財產權與研習學員成果。
   - 驗證成功後自動記住授權狀態，並於頁面右上角提供「重新上鎖」按鈕方便隨時切換。

3. **現代化互動體驗**
   - 支援即時關鍵字過濾搜尋（即時高亮標題、作者、內文）。
   - 支援分區快速跳轉下拉選單。
   - 支援滑鼠滾輪水平畫布捲動與單欄垂直滑動。
   - 卡片互動式詳細資訊 Modal 視窗、高畫質縮放燈箱與一鍵複製內容。

---

## 📂 檔案目錄結構

```text
├── index.html                               # 典藏看板主網頁介面 (直接下載與本機執行)
├── data.js                                  # 看板完整結構化本機資料庫 (零 Padlet 依賴)
├── .nojekyll                                # GitHub Pages 靜態發布配置
├── .gitignore                               # Git 忽略清單
├── README.md                                # 專案說明文件
└── assets/                                  # 實體離線資源庫
    ├── exports/                             # 官方全板備份與打包專區
    │   ├── padlet_full_offline_bundle.zip   # 全站全量離線旗艦大禮包 (24.35 MB)
    │   ├── padlet_images_all.zip            # 全板高解析圖片懶人包 (12.28 MB)
    │   ├── padlet_data_export.xlsx          # 全看板 Excel 試算表 (含實體路徑/大小)
    │   ├── padlet_document_export.pdf       # 高解析全板 PDF 檔案
    │   └── padlet_screenshot_export.png     # 全景畫布長截圖
    ├── games/                               # 3 套獨立離線互動遊戲系統
    │   ├── 246game.html                     # 2-4-6 認知實驗系統
    │   ├── mygopen-test.html                # 防詐查核線上測驗 (4.03 MB)
    │   ├── case072.html                     # 情境模擬查核遊戲 (4.68 MB)
    │   └── html2canvas.min.js               # 本地截圖支援庫
    ├── lectures/                            # 研習講義與影音離線鏡像
    │   ├── lecture_1_3.html                 # 第1~3節 講義離線 HTML
    │   ├── lecture_1_3_offline.md           # 第1~3節 講義 Markdown 源碼
    │   ├── lecture_4.html                   # 第4節 講義離線 HTML
    │   ├── lecture_4_offline.md             # 第4節 講義 Markdown 源碼
    │   ├── SS練習.mp4                       # 第4節 實作影音 (1.68 MB)
    │   └── images/                          # 講義內嵌 14 份教學圖表
    └── images/                              # 全板 28 份高解析實體圖檔與背景畫布
```

---

## 🌐 研習課程主題

- **主講講師**：李宜玲 老師（台中市資訊教育議題分團輔導員、教育部中央輔導團科技領域輔導員）
- **研習單元**：
  1. 講師區：講師個人資歷與 1~4 節精華講義
  2. 2-4-6 遊戲歷程：Wason 2-4-6 認知實驗與假設檢定探究
  3. 查核成績單：反詐騙與事實查核成果評量
  4. 給講師的話：學員回饋與心得
  5. 查核遊戲：情境模擬查核遊戲、消失的學生實時線上互動解謎
