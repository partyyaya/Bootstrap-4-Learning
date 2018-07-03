## 安裝與開始

### 一、安裝資源
- 新建專案資料夾
- 下載最新版 Bootstrap 4：<a href="https://github.com/twbs/bootstrap/releases/download/v4.0.0/bootstrap-4.0.0-dist.zip">Bootstrap 4下載</a>
- 將下載的 js , css 資料夾拉出 放到 專案資料夾 下
- BootStrap 4拿掉了圖示，可到 <a href="https://use.fontawesome.com/releases/v5.1.0/fontawesome-free-5.1.0-web.zip">fontawesome下載</a> 
- 解壓後，將 fonts 及 css 複製到 專案資料夾 裡面
- 下載 jquery：<a href="https://jquery.com/download/">jquery下載</a>，並存入 js 資料夾中
- 下載 popper.js ：<a href="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.11.0/umd/popper.min.js">popper下載</a>，存入 js 資料夾中

### 二、引入index.html內
- 可以使用網址引入
- css :　

```html
<link rel="stylesheet"  
href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"  
integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm"  
crossorigin="anonymous">
```
- js : 

```html
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"  
crossorigin="anonymous">
</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"  
crossorigin="anonymous">
</script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
crossorigin="anonymous">
</script>
```

- 建立index.html
```html
<html lang="zh-Hant-TW">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>Doc</title>
        <!-- Bootstrap CSS -->
        <link rel="stylesheet" href="css/bootstrap.min.css">
        <link rel="stylesheet" href="css/fontawesome.css">
        <link rel="stylesheet" href="css/my.css">
        <!-- JavaScript -->
        <script src="js/jquery-3.2.1.min.js"></script>
        <script src="js/popper.min.js"></script>
        <script src="js/bootstrap.min.js"></script>
    </head>
    <body>
        <h1>Hello, world!</h1>       
    </body>
</html>
```
- 引入順序請勿隨便調整
- width=device-width ：表示寬度是設備螢幕的寬度
- initial-scale=1：表示初始的縮放比例， 可以讓網頁的寬度自動適應手機螢幕的寬度
- 在iOS9更新中更改了initial-scale 的用途，故使用shrink-to-fit=no 來替代
- 其中的 css/my.css 是用來放置自定義的CSS 內容，例如想要讓頁面用微軟正黑體，加入字型設定即可：
```css
body{
    font-family: '微軟正黑體';
}
```


