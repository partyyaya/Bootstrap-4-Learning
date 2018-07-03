## 不同的呈現(display)方式

### 一、套用display方法
- xs : .d-{value}
- sm, md, lg, xl : .d-{breakpoint}-{value}
- value 可換成 : 
    - none
    - inline
    - inline-block
    - block
    - table
    - table-cell
    - table-row
    - flex
    - inline-flex
- 範例 : 
```html
<!-- 
    d-inline = display:inline : 在同一行
    p-2 : 對內(padding)四邊距為$spacer * .5
    bg : 背景顏色
    text-white : 文字顏色
 -->
<div class="d-inline p-2 bg-primary text-white">d-inline</div>
<div class="d-inline p-2 bg-dark text-white">d-inline</div>
```
### 隱藏元素
- 例子 : .d-none .d-md-block .d-lg-none 將隱藏所有螢幕尺寸的元素，除了中型(lg)和大型(xl)設備

| 螢幕大小 | class |
| -- | -- |
| Hidden on all | .d-none |
| Hidden only on xs	|.d-none .d-sm-block |
| Hidden only on sm	|.d-sm-none .d-md-block |
| Hidden only on md	|.d-md-none .d-lg-block |
| Hidden only on lg	|.d-lg-none .d-xl-block |
| Hidden only on xl	|.d-xl-none |
| Visible on all |	.d-block |
| Visible only on xs |	.d-block .d-sm-none |
| Visible only on sm |	.d-none .d-sm-block .d-md-none |
| Visible only on md |	.d-none .d-md-block .d-lg-none |
| Visible only on lg |	.d-none .d-lg-block .d-xl-none |
| Visible only on xl |	.d-none .d-xl-block |

### 運用在列印
- 例子 :
```html
<div class="d-print-none">只出現在螢幕,但不印出來</div>
<div class="d-none d-print-block">只有列印才會看到</div>
<div class="d-none d-lg-block d-print-block">只有 lg螢幕以上 和 列印出來 才會顯示</div>
```

| class |
| -- |
| .d-print-none |
| .d-print-inline |
| .d-print-inline-block |
| .d-print-block |
| .d-print-table |
| .d-print-table-row |
| .d-print-table-cell |
| .d-print-flex |
| .d-print-inline-flex |
