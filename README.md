# Vue Azure OpenAI ChatGPT AccuHit

## demo
https://donaldtsaoaccu.github.io/vue_Chatbot_accuhit/

### 使用方法

1. 將vue_uniChatbot直接下載到你的專案裡 (vue_uniChatbot檔名可自取，ex.accu)
2. 將accu**解壓縮至此**會有一個`vue_Chatbot_accuhit-main`的資料夾，將其重新命名(直接使用該名稱也行)
3. 打開自己專案的入口頁面(以html為例)，在`<body></body>`標籤中新增 
    
        <div id="app"></div>

    然後繼續新增兩行`<script></script>` ，如下 --

        <script src="accu/js/app.js"></script>
        <script src="accu/js/chunk-vendors.js"></script>
    
    最後在`<head>`標籤中新增
       
        <link rel="stylesheet" href="accu/css/app.css">

## 圖片位址問題

 有兩張圖片位址需自行修正，請照以下步驟操作

 1. 懸浮icon的圖，在***accu/css/app.css***裡，有段`background:url(/vue_uniChatbot/img/uni_logo.png) `
 請改成 --> 

         background:url(../img/uni_logo.png) 

 2. 對話機器人的圖，在***accu/js/app.js***裡，有段`{class:"img-circle",src:"cow.png",alt:"image"}` 就在第二行一開始，請改成 -->
       
        {class:"img-circle",src:"accu/cow.png",alt:"image"}

## 如果想看本地index.html

直接刪除前綴路徑()，開頭直接`js/app.js` 跟 `css/app.css` ，還有`href="accuhit.ico"`



## !!注意事項


 - css樣式可能會被原生css影響到，可能導致單向影響或雙向影響
 - 圖檔位置可依資料夾位置自行更動
 - 此為大致定檔版本，如需自行修改圖檔及專案，請用 ***vue_Chatbot_picChange*** 或原始檔 ***vue_uniChatbot***
   


