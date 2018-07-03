 ## 欄位推移

- Bootstrap 4 裡面已經沒辦法用 .col-offset-x 或者 .offset-sm-x 來跳過幾欄
- 可利用下表將剩下的空位謄出來。

| .mr-auto | .mx-auto | .ml-auto |
| -- | -- | -- |
| 將右邊剩下的空位謄出 | 空位平均分散到左右兩邊 | 空位放到左邊 |

- 使用範例：
```html
<div class="container">
    <div class="row">
        <div class="col-2">col 等寬 1/3</div>
        <div class="col-2 ml-auto">col 等寬 2/3</div>
        <div class="col-2">col 等寬 3/3</div>
    </div>
</div>
```

<img src="../img/offset.png" width="100%" height="100%">
