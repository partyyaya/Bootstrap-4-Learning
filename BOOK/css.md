## CSS 基礎知識

### 一、關於CSS
- Bootstrap是一套CSS框架，簡單了解CSS用法是必要的
- CSS：Cascading Style Sheets，簡稱CSS，中文通常稱為層疊樣式表或串接樣式表
- 可用來替網頁上的各種元件設定其外觀
- 套用樣式的三種方法：

|  | 行內樣式 | 內部頁面樣式 | 外部連結樣式 |
| -- | -- | -- | -- |
| 範圍 | 最小 | 頁中 | 許多頁 |
| 優先 | 最優先 |  |  |
| 用法 | ```<標籤 style="CSS;">``` | ```<style type='text/css'>```<br/>``` CSS; ```<br/>```</style>``` | ```<link href="CSS檔.css" rel="stylesheet">```|

- 頁面可同時套用數個css檔或設定，重複的以最後讀到的為主
- 並可以用import來引入其他的CSS檔：如：@import url("my.css");

|  | 標籤挑選器 | ID挑選器 | 類別挑選器 |
| -- | -- | -- | -- |
| 樣式表 | p {CSS屬性: 值;} | #home{CSS屬性: 值;} | .row{CSS屬性: 值;} |
| 網頁 | `<p></p>` | `<div id="home"></div>` | `<div class="row"></div>` |

- 基本上，BootStrap就是一堆類別挑選器的組合
