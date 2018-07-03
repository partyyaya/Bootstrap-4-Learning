## 欄位排序

<pre>
  常見的例子是三欄式畫面（左側邊+主內容+右側邊），
  在手機觀看，變成單欄式時，希望變成：（主內容→左側邊→右側邊）的順序。
</pre>

- 用 .order 調整：
```html
<div class="container">
  <div class="row">
    <div class="col-sm-7 order-sm-2">
      在中間的主內容區
    </div>
    <div class="col-sm order-sm-1">
      在左邊的側邊欄
    </div>
    <div class="col-sm order-sm-3">
      在右邊的側邊欄
    </div>
  </div>
</div>
```

<pre>
  請依照在單欄式情況下，希望呈現的先後順序來寫，然後再利用 order 來調整位置。
  在三欄式時（未自適應前），會按照 order 的順序來排，
  在單欄式時，就會忽略 order，依照語法順序來排。
</pre>