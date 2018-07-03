## grid(網格) 系統應用

### 一、使用網格的注意事項
- 網格系統以 flexbox（CSS3）為基礎，可以做到自動等寬等高的欄位 、自動平均欄位、垂直置中等以往很難做的功能。
- 同時也代表對 IE9（以下）不再支援，至少要用IE10才行。
- 網格系統必須在容器（.container）中才有作用

### 二、指定欄寬用法
- 使用範例：
```html
<div class="container">
    <div class="row">
        <div class="col-sm-5">左邊五欄</div>
        <div class="col-sm-7">右邊七欄</div>
    </div>
</div>
```
- .row 代表一個橫列，確保裡面的欄位對齊、排序。
- .col-sm 是斷點前綴詞，後面接的是欄位寬度設定，預設滿版為12欄
- 若超過12欄，自動新增一個 .row

### 三、自動等寬用法
- 使用等寬欄位
```html
<div class="container">
    <div class="row">
        <div class="col">col 等寬 1/5</div>
        <div class="col">col 等寬 2/5</div>
        <div class="col">col 等寬 3/5</div>
        <div class="col">col 等寬 4/5</div>
        <div class="col">col 等寬 5/5</div>
    </div>
    <div class="row">
        <div class="col-sm">col-sm 等寬 1/5</div>
        <div class="col-sm">col-sm 等寬 2/5</div>
        <div class="col-sm">col-sm 等寬 3/5</div>
        <div class="col-sm">col-sm 等寬 4/5</div>
        <div class="col-sm">col-sm 等寬 5/5</div>
    </div>
</div>
```
- 上方是不管螢幕多大，都分成五欄
- 下方是當螢幕在 576 以上時，才分五欄，576 以下的時候，自動調成單欄式。

### 四、指定欄寬+自動欄寬
- 可以指定某幾欄的欄寬，其餘的自行自動平均
```html
<div class="container">
    <div class="row">
        <div class="col-sm">自動平均分配</div>
        <div class="col-sm-7">指定佔 7 欄</div>
        <div class="col-sm">自動平均分配</div>
    </div>
</div>
```

### 五、根據內容多寡自動調整欄寬
- 不確定該站多少欄寬，讓電腦自行根據內容多寡來判斷：
```html
<div class="container">
    <div class="row">
        <div class="col-sm">自動平均分配</div>
        <div class="col-sm-auto">根據中間內容多多寡來判斷欄寬</div>
        <div class="col-sm">自動平均分配</div>
    </div>
</div>
```

### 六、不同斷點的欄寬搭配
- 在同一個欄位根據不同斷點給予不同大小
```html
<div class="container">
    <div class="row">
        <div class="col">自動平均分配</div>
        <div class="col-sm-6 col-md-7 col-lg-8">根據不同螢幕大小來指定中間欄位欄寬</div>
        <div class="col">自動平均分配</div>
    </div>
</div>
```