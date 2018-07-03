## 按鈕

#### .btn 設計 ```<button>``` 元素使用。 但也可在 ```<a>``` 或 ```<input>``` 元素上使用

<table>
    <tr>
        <td width="10%">標籤</td>
        <td width="90%">使用方法</td>
    </tr>
    <tr>
        <td>a</td>
        <td>&lt;a class="btn btn-primary" href="#" role="button">Link&lt;/a></td>
    </tr>
    <tr>
        <td>button</td>
        <td>&lt;button class="btn btn-primary" type="submit">Button&lt;/button></td>     
    </tr>
    <tr>
        <td>input:button</td>
        <td>&lt;input class="btn btn-primary" type="button" value="Input"></td>     
    </tr>
    <tr>
        <td>input:submit</td>
        <td>&lt;input class="btn btn-primary" type="submit" value="Submit"></td>     
    </tr>
    <tr>
        <td>input:reset</td>
        <td>&lt;input class="btn btn-primary" type="submit" value="reset"></td>     
    </tr>
</table>

#### 按鈕顏色樣式
- 改變按鈕顏色

| 顏色 | 對應的class |
| -- | -- |
| 藍色 | btn-primary |
| 灰色 | btn-secondary |
| 綠色 | btn-success |
| 紅色 | btn-danger |
| 黃色 | btn-warning |
| 淺藍色 | btn-info |
| 白色 | btn-light |
| 黑色 | btn-dark |
| 原生 | btn-link |
- 若要改變外框顏色 : 加上 outline 即可
- 例子 : btn-outline-primary

#### 按鈕大小樣式

| 小 | 大 | 區塊 |
| -- | -- | -- |
| btn-sm | btn-lg | btn-block |
- 範例 ：
```html
<button type="button" class="btn btn-primary btn-block">level button</button>
```

#### 啟用與停用
- 啟用：active
- 停用：disabled

| 狀態 | 標籤 | 用法 | 範例 |
| -- | -- | -- | -- |
| 啟用 | a | class | `<a href="#" class="btn btn-primary btn-lg active" role="button">link</a>` |
| 啟用 | button | class | `<button type="button" class="btn btn-lg btn-primary active">button</button>` |
| 啟用 | input | class | `<input type="button" class="btn btn-secondary btn-lg active" value="input" >` |
| 停用 | a | class | `<a href="#" class="btn btn-primary btn-lg disabled" role="button">link</a>` |
| 停用 | button | 標籤 | `<button type="button" class="btn btn-lg btn-primary" disabled>button</button>` |
| 停用 | input | 標籤 | `<input type="button" class="btn btn-secondary btn-lg active" disabled value="input" >` |

#### 切換狀態
- 增加 data-toggle="button"
- 如預先需要切換按鈕，則須手動將 .active class 和 aria-pressed="true" 添加到 `<button>` 
- 範例 : 
```html
<button type="button" class="btn btn-primary" data-toggle="button" aria-pressed="false" autocomplete="off">
  Single toggle
</button>
```

#### 自行定義顏色管理工具
- 自行定義按鈕工具：http://blog.koalite.com/bbg/
- 定義出來的按鈕可以放在 css/my.css 中
- 若希望底色是透明的，可自行將背景顏色取代為 transparent