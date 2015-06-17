# Openpush framework 手機訊息推送平台 #

## Openpush研發動機 ##
手機訊息推送應用目前當紅, 不管是單純的送文字簡訊, 或圖文並茂的多媒體簡訊, 以及可以連到手機網站的WAP Push, 各種應用都有. 但身為程式設計師的我們, 卻沒辦法免費取得相關資源, 即使是個人或學生身份, 只想實驗一下自己的IDEA, 就必須找系統業者拿API簽約, 才能開始Coding實驗發送訊息到手機, 就算不怕麻煩的去申請了, 超貴的訊息發送費用, 也讓人吃不消.

除了費用問題, 各家大哥大業者的API格式不統一, 且訊息欄位編碼非常複雜, 只是簡單的送個文字簡訊, 要填的欄位多得驚人, 甚至必須用Socket才能發送, 其實只要一個簡單的HTTP API就能解決的事情, 為何要弄得這麼複雜? Openpush簡化各種程式語言發送手機訊息的複雜度, 純文字簡訊SMS的發送參數只要手機號與內容即可. 圖文並茂的MMS與WAP Push也不需額外學習特殊格式, HTTP POST就能發送.

## 特色 ##
  * Open Source 開放原始碼, 並提供 Java, C#, Python, PHP 等程式語言的範例
  * 開放式的 Target Adapter 設計, 允許開發者輕易銜接各家系統業者訊息API, 甚至各商業公司的訊息API, 任意隨時切換
  * 無論是 SMS, MMS, WAP Push 發送, 都可透過Email模擬發送, 開發各種應用完全免費
  * 統一採用HTTP API (HTTP POST), 就能發送各種訊息, 參數極簡, 容易使用
  * 未來將支援 J2ME MIDP Push Registry, 利用簡訊啟動手機Java程式, 背景執行各種應用

## Target Adapter目前已經有下面實作 ##
  * TargetAdapterSmtp: 將各種訊息發到電子郵件信箱模擬實驗, 完全免費
  * TargetAdapterChtExpressMail: 限發中華電信手機門號, SMS/MMS/WAP Push不論訊息種類與大小一律0.5元, 最多480吃到飽無限發送
  * TargetAdapterTaiwan: 限發中華電信,台灣大哥大,遠傳, 每則SMS或WAP Push 1.0元, 每則 MMS 2.0元

## 最新消息請看部落格 ##
您可以到Openpush部落格留言, 並參與開發過程喔
http://openpush.blogspot.com/
