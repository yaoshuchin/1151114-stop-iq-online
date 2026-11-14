# STOP麥擱騙! 我智商在線 · 研習數位典藏鏡像站

本專案為「**STOP麥擱騙! 我智商在線**」研習看板之高保真、離線本機典藏平台，提供完整的教材鏡像、活動歷程、查核遊戲及學員作品典藏。

---

## 📌 專案特點與架構

1. **檔案與圖片完整實體複製 (100% 離線可用，絕無外部圖床依賴)**
   - 全看板所有卡片附加圖片與照片，全數抓取**高解析原始大圖（Full Resolution）**實體典藏於 `./assets/images/`，徹底擺脫外部 Padlet 縮圖快取與過期權杖限制。
   - 包含學員上傳之認知實驗推論截圖、成績單認證圖、課程封面與高解析背景畫布。
   - 李宜玲老師精闢講義完整離線鏡像（HTML 網頁版 + Markdown 原始文檔）。
   - 包含講義內嵌之 14 份教學圖表實體檔案（`./assets/lectures/images/`）。
   - 包含第 4 節課堂實作操作影片（`assets/lectures/SS練習.mp4` · 1.68 MB 完整收錄）。
   - 提供「下載本機檔案 (已完整典藏)」抽屜，可一鍵下載：
     - `assets/exports/padlet_data_export.xlsx`（官方看板全量試算表，含檔案大小與路徑）
     - `assets/exports/padlet_document_export.pdf`（高解析向量式全板備份文檔）
     - `assets/exports/padlet_screenshot_export.png`（全景畫布備份截圖）
     - 講義 HTML / Markdown 與影片離線包

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
├── index.html                               # 典藏看板主網頁介面
├── data.js                                  # 看板完整結構化本機資料庫 (高解析實體路徑)
├── .nojekyll                                # GitHub Pages 靜態發布配置
├── .gitignore                               # Git 忽略清單
├── README.md                                # 專案說明文件
└── assets/                                  # 實體離線資源庫
    ├── exports/                             # 官方全板備份輸出
    │   ├── padlet_data_export.xlsx          # 全看板 Excel 試算表
    │   ├── padlet_document_export.pdf       # 高解析全板 PDF 檔案
    │   └── padlet_screenshot_export.png     # 全景畫布截圖
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
