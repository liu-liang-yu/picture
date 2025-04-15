HTML 結構 (<index.html>)
1.  <!DOCTYPE html>
* 指令： 宣告文件類型為 HTML5。
* 說明： 這是 HTML 文件的第一行，告知瀏覽器以最新的 HTML 標準來解析此文件。
2.  <html lang="zh-Hant">
* 指令： HTML 根元素，指定網頁的主要語言為繁體中文 (zh-Hant)。
* 說明： 包裹了整個 HTML 文件的內容，lang 屬性有助於瀏覽器和搜尋引擎理解網頁的語言。
3.  <head>
* 指令： 包含網頁的元數據（metadata），這些資訊不會直接顯示在網頁內容中。
* 說明： <head> 標籤用於存放關於 HTML 文檔的資訊，例如字符編碼、標題、樣式表連結等。
4.  <meta charset="UTF-8" />
* 指令： 設定網頁的字符編碼為 UTF-8。
* 說明： UTF-8 是一種通用的字符編碼，可以支援顯示多種語言的文字，包括繁體中文。
5.  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
* 指令： 設定網頁在不同裝置上的 viewport，確保響應式設計。
* 說明： 這使得網頁能夠根據裝置的寬度自動調整縮放比例，提供更好的使用者體驗。
6.  <title>圖片展示系統</title>
* 指令： 設定網頁在瀏覽器標籤或視窗標題欄中顯示的文字為「圖片展示系統」。
* 說明： title 標籤對於使用者體驗和搜尋引擎優化都很重要。
7.  <style> ... </style>
* 指令： 在 HTML 文件中嵌入 CSS 樣式規則。
* 說明： 這個標籤包含了用於控制網頁元素外觀的 CSS 程式碼。

* **`body { ... }`**
    * **指令：** 設定 `<body>` 元素（網頁的主要內容區域）的樣式。
    * **說明：** 包括字體 (Arial, sans-serif)、內邊距 (20px) 和文字置中對齊 (`text-align: center`).

* **`.buttons { ... }`**
    * **指令：** 設定 class 為 `buttons` 的 `<div>` 元素的樣式。
    * **說明：** 設定按鈕容器的下邊距 (20px)。

* **`button { ... }`**
    * **指令：** 設定所有 `<button>` 元素的樣式。
    * **說明：** 包括內邊距 (10px 20px)、外邊距 (5px)、文字大小 (16px) 和滑鼠游標樣式 (`cursor: pointer`).

* **`.gallery { ... }`**
    * **指令：** 設定 class 為 `gallery` 的 `<div>` 元素的樣式。
    * **說明：** 使用彈性佈局 (`display: flex`)、允許項目換行 (`flex-wrap: wrap`)、圖片在水平方向置中對齊 (`justify-content: center`) 和設定圖片之間的間距 (15px)。

* **`.gallery img { ... }`**
    * **指令：** 設定 `.gallery` 容器內所有 `<img>` 元素的樣式。
    * **說明：** 設定圖片的預設寬度 (300px)、陰影效果 (`box-shadow`) 和變形及陰影的過渡效果 (`transition`).

* **`.gallery img:hover { ... }`**
    * **指令：** 設定滑鼠移到 `.gallery` 容器內的 `<img>` 元素上時的樣式。
    * **說明：** 設定滑鼠移到圖片上時的放大效果 (`transform: scale(1.05)`) 和移除陰影 (`box-shadow: none`).

* **`@media (max-width: 600px) { ... }`**
    * **指令：** 媒體查詢，當螢幕寬度小於等於 600px 時應用以下樣式。
    * **說明：** 用於響應式設計，針對小螢幕裝置調整佈局。

    * **`.gallery { ... }`**
        * **指令：** 在小螢幕下，設定 class 為 `gallery` 的 `<div>` 元素的樣式。
        * **說明：** 將圖片排列方向改為垂直方向 (`flex-direction: column`).

    * **`.gallery img { ... }`**
        * **指令：** 在小螢幕下，設定 `.gallery` 容器內所有 `<img>` 元素的樣式。
        * **說明：** 將圖片寬度調整為容器的 90% (`width: 90%`).

8.  <body>
* 指令： 包含網頁上所有可見的內容。
* 說明： 這是 HTML 文件的主體部分，包含了所有的文字、圖片、連結、按鈕等元素。
9.  <h1>圖片展示系統</h1>
* 指令： 顯示一個層級一的標題，內容為「圖片展示系統」。
* 說明： 用於呈現網頁的主要標題。
10. <div class="buttons"> ... </div>
* 指令： 建立一個 `div` 元素，其 class 為 `buttons`，用於包含按鈕。
* 說明： 這個 `div` 用於將相關的按鈕組織在一起，方便樣式化和管理。
11. <button onclick="showCategory('all')">全部圖片</button>
* 指令： 建立一個按鈕，當點擊時執行 JavaScript 函式 `showCategory` 並傳入字串 'all' 作為參數。
* 說明： 這個按鈕用於顯示所有類別的圖片。
12. <button onclick="showCategory('nature')">自然風景圖</button>
* 指令： 建立一個按鈕，當點擊時執行 JavaScript 函式 `showCategory` 並傳入字串 'nature' 作為參數。
* 說明： 這個按鈕用於顯示自然風景類別的圖片。
13. <button onclick="showCategory('city')">城市風景圖</button>
* 指令： 建立一個按鈕，當點擊時執行 JavaScript 函式 `showCategory` 並傳入字串 'city' 作為參數。
* 說明： 這個按鈕用於顯示城市風景類別的圖片。
14. <div class="gallery" id="gallery"></div>
* 指令： 建立一個 `div` 元素，其 class 為 `gallery` 和 id 為 `gallery`，用於顯示圖片。
* 說明： JavaScript 將會在這個 `div` 內動態生成圖片元素。
15. <script> ... </script>
* 指令： 包含客戶端的 JavaScript 程式碼。
* 說明： 這個標籤用於存放控制網頁行為的 JavaScript 程式碼。

* **`const images = { ... };`**
    * **指令：** 宣告一個名為 `images` 的常數物件。
    * **說明：** 這個物件用於儲存不同類別的圖片路徑陣列。
        * **`all: [...]`**: 包含所有圖片的路徑。
        * **`nature: [...]`**: 包含自然風景圖片的路徑。
        * **`city: [...]`**: 包含城市風景圖片的路徑。

* **`function showCategory(category) { ... }`**
    * **指令：** 定義一個名為 `showCategory` 的函式，它接受一個 `category` 參數。
    * **說明：** 這個函式用於根據選擇的類別顯示圖片。
        * **`const gallery = document.getElementById("gallery");`**: 取得 `id` 為 "gallery" 的 DOM 元素。
        * **`gallery.innerHTML = images[category].map(img => \`<img src="${img}" />\`).join('');`**: 根據傳入的 `category`，從 `images` 物件中取得對應的圖片路徑陣列，使用 `map` 方法將每個路徑轉換為一個 `<img>` 標籤的字串，最後使用 `join('')` 將這些字串連接起來，並更新 `gallery` 元素的 `innerHTML`，從而顯示對應的圖片。

* **`showCategory('all');`**
    * **指令：** 在網頁載入時呼叫 `showCategory` 函式並傳入字串 'all'。
    * **說明：** 這使得網頁預設顯示所有類別的圖片。
16. </body>
* 指令： 標示 HTML 文件內容的結束。
* 說明： 所有顯示在網頁上的元素都應該放在 `<body>` 標籤內。
17. </html>
* 指令： 標示 HTML 文件的結束。
* 說明： 這是 HTML 文件的最後一個標籤。
