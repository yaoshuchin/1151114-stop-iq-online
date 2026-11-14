# 第四節 STOP麥擱騙！我智商在線 (教師版)

:::info
學習目標：
1. 能夠運用「以圖搜圖」功能進行查核
2. 能夠運用GOOGLE智慧鏡頭+「以圖搜圖」功能進行查核
3. 能夠使用AI模式進行查核
4. 能夠使用prompt提升查核的準確度
5. 認識其它查核工具

:::

## 任務一 以圖搜圖
Q1：使用GOOGLE以圖搜圖功能，查看看這個地點在哪裡？
![01.這是哪裡](https://hackmd.io/_uploads/SJuVacslGe.jpg)

## 任務二 GOOGLE 智慧鏡頭+以圖搜圖
Q2：按右鍵，開啟GOOGLE智慧鏡頭搜尋，查看看這個地點在哪裡？
![02.這是哪裡](https://hackmd.io/_uploads/rkz1Rqigzl.jpg)

Q3：查看看這個地點在哪裡？然後打開google map，查看看離這景點最近的國中是哪一間？
![03.我在哪教書](https://hackmd.io/_uploads/BkMkR9ixfx.jpg)

## 任務三 問AI
![AI模式](https://hackmd.io/_uploads/SkmCF6jxGl.jpg)
Q4.開啟瀏覽器的AI模式，問「這張圖片是真的嗎?還是AI生成的?」
![04.這是真的嗎](https://hackmd.io/_uploads/SkeW509ogGx.jpg)

Q5-1.哪一個建築物是AI生圖？
圖A：
![Art Nouveau](https://hackmd.io/_uploads/SkfGiMn2Gg.png)


圖B：
![怪怪屋02](https://hackmd.io/_uploads/BJi0YG22Me.jpg)

Q5-2.哪一張旋轉樓梯是AI生圖？
圖A：
![哪一張是AI生圖(旋轉樓梯)-A](https://hackmd.io/_uploads/BkjnljoeGe.jpg)

圖B：
![哪一張是AI生圖(旋轉樓梯)-B](https://hackmd.io/_uploads/Bkxpliixfg.jpg)

圖C：
![哪一張是AI生圖(旋轉樓梯)-C](https://hackmd.io/_uploads/BySaesogGe.jpg)

## 任務四 STOP查核技巧練習

網傳「只有七個名字的民族」故事內容：
```
雪巴人信仰藏傳佛教，相信一週7天各有不同的守護神，因此都以星期幾出生來命名。
星期天出生就叫太陽，星期二出生就叫月亮。一個村莊裡總共就只有7個名字，如果有一個媽媽叫「太陽啊~回家吃飯啦！」就會有1/7的小孩跑回家去了。
這樣怎麼搞得清楚，倒底是在叫誰啦🤣🤣🤣
星期天「Nyima」，有「太陽」的意思。
星期一「Dawa」，有「月亮」的意思。
星期二「Mingma」，有「火星」的意思。
星期三「Lhakpa」，有「水星」的意思。
星期四「Fura」、「Phurba」、「Furba」，有「木星」的意思。
星期五「Pasang」，有「金星」的意思。
星期六「Pemba」，有「土星」的意思。
```


## 任務五 擅用查核指令，打破AI幻覺
AI幻覺示例
:::spoiler
```
請用 micro:bit MicroPython 的 display.scroll_vertical() 寫一段讓文字由下往上捲動的程式,並說明參數。
```

scroll_vertical() 是我自己編的,目前官方並沒有這個函式,請你先查一下官方文件確認。AI 很容易煞有其事地寫出程式和參數說明。老師貼進編輯器一執行就報錯,查核結果一目了然。

若AI生成了程式碼，請貼在[模擬器](https://python.microbit.org/v/3)上執行看看。
:::

AI可能產生幻覺的場景：冷門、在地、要求精確細節..更容易出錯
:::spoiler
### 例子二:不存在的教材或指引
請摘要國教院《國中生活科技 AI 融入教學手冊(2023)》第二章的教學活動,並列出頁碼。

這份手冊是我虛構的。可以順便讓老師比較「搜尋功能開啟」和「關閉」時,AI 的反應有什麼不同。

### 例子三:錯誤前提
教育部規定國小三年級起必須學會 Python,依據是哪一份公文?

我的理解是課綱並沒有這樣的規定,但請你自行到教育部或國教院網站確認。看 AI 會糾正前提,還是順著編出公文字號。

### 例子四:冷門版本細節
micro:bit V1 和 V2 在 MakeCode 中,哪些積木只有 V2 能用?請完整列出。

要求「完整列出」是關鍵,AI 常常漏列或多列。老師可以對照 MakeCode 官方網站驗證,這個例子比較適合展示「部分正確、部分錯誤」的情況。
:::

### 設定「事實查核員」角色
> 提示詞範例：「你現在是一名專業的事實查核員，請調查以下陳述，列出支持
> 與反對的證據。」


### 要求「按部就班」（Step-by-Step）、列出「參考網站或文件」進行推理
> 提示詞範例：「請依序進行:
> 1. 列出內容中的關鍵事實(人事時地物、數字、函式名稱、文件名稱、法條等)
> 2. 優先搜尋權威來源(政府機關、學術機構、官方文件)
> 3. 比對陳述與來源之間的差異
> 4. 給出結論」


### 其它規則
> 提示詞範例：「規則: 每個陳述請標示結論:「有可靠來源支持」、「與來源不符」或「查無資料」
> - 找不到可靠來源時,請直接寫「查無資料」,不要推測,也不要編造來源或連結
> - 只提供你確實搜尋到的連結,並說明該連結的哪一部分支持或反駁這個陳述
> - 若不同來源說法衝突,請分別說明各方觀點
> - 若涉及程式碼或操作步驟,請標示你無法確定的部分,並指出我應該查哪份官方文件
> - 最後請列出「我應該自己再確認的地方」

:::success
可直接複製以下完整查核指令請AI進行查核：
```
你現在是一名嚴謹的事實查核員。請查核我貼上的內容,並逐句拆成單一陳述,分別查證。

請依序進行:
1. 列出內容中的關鍵事實(人事時地物、數字、函式名稱、文件名稱、法條等)
2. 優先搜尋權威來源(政府機關、學術機構、官方文件)
3. 比對陳述與來源之間的差異
4. 給出結論

規則:
- 每個陳述請標示結論:「有可靠來源支持」、「與來源不符」或「查無資料」
- 找不到可靠來源時,請直接寫「查無資料」,不要推測,也不要編造來源或連結
- 只提供你確實搜尋到的連結,並說明該連結的哪一部分支持或反駁這個陳述
- 若不同來源說法衝突,請分別說明各方觀點
- 若涉及程式碼或操作步驟,請標示你無法確定的部分,並指出我應該查哪份官方文件
- 最後請列出「我應該自己再確認的地方」
```
:::

Q6.訊息查核影片
`傳言：「伊朗襲擊了位於杜拜的美國中央情報局總部,相關畫面已經曝光，阿聯酋正在逮捕那些洩漏影片的人。但他們無法掩蓋這件事。」`
[影片連結](https://drive.google.com/file/d/1ZKmehYpzDrDYaT3lP0a3UCJS81qZVB5g/view?usp=sharing)

## 任務六 模擬情境查核遊戲
[![螢幕擷取畫面 2026-11-14 081326](https://hackmd.io/_uploads/rJ1Aw7H0Ml.png)](https://eurekalea.github.io/html/case072.html)


## 補充資料
- 詐騙網址幫你查 https://check.mygopen.com/ ([教學影片](https://www.instagram.com/reel/Dddgm8yyamk/))
- [LINE 官方機器人](https://line.me/R/ti/p/%40mygopen) ([使用教學](https://www.mygopen.com/p/blog-page_28.html))
- [Google Fact Check Tools](https://toolbox.google.com/factcheck/explorer/search/list:recent;hl=zh)
- [HIVE Moderation](https://hivemoderation.com/ai-generated-content-detection)：上傳圖像、視訊或音頻，進行逐幀 AI 生成和深度偽造檢測，並給出機率評分。
- [公視君竹的媒體白名單](https://andrewintw.github.io/taiwan-media-whitelist/)

:::success
:bulb:不是什麼都要查！想轉傳 + 高風險->必須先查證
:::

![螢幕擷取畫面 2026-06-02 112905](https://hackmd.io/_uploads/SJOS0aixfg.png)



<style>
/* Spoiler 區塊 */
.markdown-body details {
  background-color: #f7f7f8 !important;
  color: #222222 !important;
  border-radius: 8px;
  padding: 8px 12px;
}

/* 文字保持清晰 */
.markdown-body details * {
  opacity: 1 !important;
}

/* Spoiler 標題 */
.markdown-body details summary {
  color: #111111 !important;
  font-weight: 600;
  cursor: pointer;
}

/* 一般內文 */
.markdown-body details p,
.markdown-body details li {
  color: #222222 !important;
}

/* 超連結：藍字 + 底線 */
.markdown-body details a,
.markdown-body details a:link,
.markdown-body details a:visited,
.markdown-body details p a,
.markdown-body details li a {
  color: #0969da !important;
  -webkit-text-fill-color: #0969da !important;
  text-decoration: underline !important;
  text-underline-offset: 2px;
}

/* 滑鼠移過超連結 */
.markdown-body details a:hover {
  color: #0550ae !important;
  -webkit-text-fill-color: #0550ae !important;
  text-decoration: underline !important;
}
</style>

