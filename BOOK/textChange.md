## 內容(文字，圖案)對齊

- 前面講的是`<div>`容器本身的對齊，這裡講的是`<div>`裡面內容的對齊。
- 例子 : `<div class="col-sm text-right"><img src="images/logo.png" alt="logo"></div>`
- 中間可加 : sm,md,lg,xl => text-sm-left

| 對齊方式 | 用法 |
| -- | -- |
| 靠左對齊 | text-left |
| 置中對齊 | text-center |
| 靠右對齊 | text-right |

- 注意，這種對齊僅對行內元件（inline）有效，如果內容是區塊元件（block），如 `<div>`，那就要用別的方式

#### text-wrap 和 Overflow
- 防止換行可搭配 .text-nowrap

```html
<div class="text-nowrap" style="width: 8rem;">
  This text should overflow the parent.
</div>
```
- 更長的內容，可增加 .text-truncate，截掉多餘內容改用 ...。需要使用 display: inline-block or display: block

```html
<!-- Praeterea iter... -->
<div class="row">
  <div class="col-2 text-truncate">
    Praeterea iter est quasdam res quas ex communi.
  </div>
</div>

<!-- Praeterea iter est q... -->
<span class="d-inline-block text-truncate" style="max-width: 150px;">
  Praeterea iter est quasdam res quas ex communi.
</span>
```

#### 文字字體變換
- 將元件中的文字內容轉變樣式 
- 例子 :

```html
<p class="text-lowercase">Lowercased text.</p>
<p class="text-uppercase">Uppercased text.</p>
<p class="text-capitalize">CapiTaliZed text.</p>

<p class="font-weight-bold">Bold text.</p>
<p class="font-weight-normal">Normal weight text.</p>
<p class="font-weight-light">Light weight text.</p>
<p class="font-italic">Italic text.</p>
```

- 注意 text-capitalize 僅改變第一個字母，其它字母的大小寫不受影響

#### 文字顏色變換
- 下表為文字顏色總表
- 注意，.text-white、.text-muted 沒有連結樣式(focus時不會變色)

| 顏色 | 用法 |
| -- | -- |
| 藍 | .text-primary |
| 灰 | .text-secondary |
| 綠 | .text-success |
| 紅 | .text-danger |
| 黃 | .text-warning |
| 淺藍 | .text-info |
| 亮 | .text-light |
| 黑 | .text-dark |
| 淺灰 | .text-muted |
| 白 | .text-white |

#### 背景顏色
- 下表為背景顏色總表

| 顏色 | 用法 |
| -- | -- |
| 藍 | .bg-primary |
| 灰 | .bg-secondary |
| 綠 | .bg-success |
| 紅 | .bg-danger |
| 黃 | .bg-warning |
| 淺藍 | .bg-info |
| 亮 | .bg-light |
| 黑 | .bg-dark |
| 白 | .bg-white |

#### 背景漸層 : (bg-gradient-後面跟bg一樣)
- 當 $enable-gradients 設置為true時，您將可以使用 .bg-gradient- 的通用類別。<br> 
  預設情況下，$enable-gradients 是停用的<br>
  在您開始使用 Bootstrap 時進行自定義。
<a href="http://bootstrap.hexschool.com/docs/4.0/getting-started/theming/#sass-options">了解我們的 Sass 選項</a>  
