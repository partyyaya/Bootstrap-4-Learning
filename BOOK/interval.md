##　間隔工具

- 間隔工具的組成為「屬性邊緣-尺寸」: ml-3
- 屬性設定
    - m - 這個 class 會設定 margin
    - p - 這個 class 會設定 padding
- 邊緣設定
    - t - 這個 class 會設定 margin-top 或 padding-top
    - b - 這個 class 會設定 margin-bottom 或 padding-bottom
    - l - 這個 class 會設定 margin-left 或 padding-left
    - r - 這個 class 會設定 margin-right 或 padding-right
    - x - 這個 class 會設定 *-left 和 *-right
    - y - 這個 class 會設定 *-top 和 *-bottom
    - 空白 - 如果邊緣 class 未加入則會設定 margin 或 padding 在元素的四個邊緣
- 尺寸設定
    - 0 - 這個 class 會設定 margin 或 padding 的樣式值為 0
    - 1 - (預設時) 這個 class 會設定 margin 或 padding 於 $spacer * .25
    - 2 - (預設時) 這個 class 會設定 margin 或 padding 於 $spacer * .5
    - 3 - (預設時) 這個 class 會設定 margin 或 padding 於 $spacer
    - 4 - (預設時) 這個 class 會設定 margin 或 padding 於 $spacer * 1.5
    - 5 - (預設時) 這個 class 會設定 margin 或 padding 於 $spacer * 3
- 使用範例：
```html
<div class="container">
    <div class="row">
        <div class="col-2">col 等寬 1/3</div>
        <div class="col-2 pl-5">col 等寬 2/3</div>
        <div class="col-2">col 等寬 3/3</div>
    </div>
</div>    
```