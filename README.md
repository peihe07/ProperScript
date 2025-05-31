# 中規中矩體── 沒有好看，沒有難看，中規中矩

![中規中矩體](https://github.com/user-attachments/assets/6ff75585-7356-426b-bbef-402a21f7dd99)

我喜歡寫字，想了好幾年終於動手自己做，會叫「中規中矩體」是因為我認為自己的字跡在沒有很好看也沒有很難看的範圍內，我想就真的是中規中矩吧。

第一次嘗試自己做字體，自己寫自己學會修字及如何利用工具處理大量的字體，還是有很多不太滿意的字，以及想要調整的地方，後續會慢慢調整更新，我相信會繼續更新版本吧XD。

## 下載

### [點此下載 v1.0](https://github.com/peiyuhsu/ProperScript/raw/main/ProperScript-Regular.ttf)

## 🛠️ 製作輔助工具

為了有效製作這套字體，我開發了一系列前端工具與腳本來進行字符排版與預覽，協助字型切割與字符對位。

### 字集模板生成器（通用分頁 HTML）
- 功能：將字集文字檔自動排版成 A4 字網格模板，可選擇每頁字數、分割檔案、位置樣式（左上 / 居中）
- 技術：JavaScript + HTML5 前端工具
- 特色程式碼：
```js
function getUnicodeFromName(name) {
    if (name.startsWith('uni')) {
        const hex = name.substring(3);
        return String.fromCodePoint(parseInt(hex, 16));
    }
    // ...
}
```

### 特殊符號模板生成器
- 功能：支援手動輸入 U+XXXX 編碼或上傳 txt，快速生成特殊符號網格
- 用途：測試標點與符號集的對齊情形

### 台語拼音模板生成器
- 功能：針對台羅拼音常用字元提供快速預覽與排版下載功能
- 使用場景：台語拼音支援測試

### 日文垂直變體模板生成器
- 功能：比較日文字元在水平與垂直模式下的顯示差異，支援垂直模式切換
- 程式碼片段：
```js
.writing-mode: vertical-rl;
.text-orientation: upright;
```
### Python 切割字符腳本
- 功能：將命名後的 .png 字符圖自動對應為 Unicode 檔名
- 檔案：`切割字符.py`
```python
from fontTools.pens.boundsPen import ControlBoundsPen
pen = ControlBoundsPen(font.getGlyphSet())
```

這些工具讓我能更有效率地規劃、臨摹與切割超過 7000 個字元，實現個人字體專案的自動化與結構化。

### 更新紀錄
- 2025/05/24 中規中矩體v1.0正式釋出。

## 應用範例

![GrrgO_OXIAAFYEO](https://github.com/user-attachments/assets/a98d77a5-221b-4844-827d-18956417cb94)
![GrrlkVgXkAE9r5L](https://github.com/user-attachments/assets/625f9a35-7647-447e-b68e-6a6b650b7ede)
![GrrlkVlXYAAMvCN](https://github.com/user-attachments/assets/8ba69206-5fe9-4569-bf5d-dd3ae22917c1)


## **製作故事**

寫字做字體的期間，我看了大量的電影、影集以及紀錄片，需要詳細列出可以私訊我（咦？），本來因為看很多的恐怖片，想把字體名稱叫做「懼體」，總之推薦《安道爾》（？？）。

![安道爾](https://github.com/user-attachments/assets/b85fdab9-0156-43c1-b42d-4f5375f57f2b)

## 授權

採用 OFL 1.1 授權開源釋出，詳細規定可以參考 Open Font License：[http://scripts.sil.org/OFL](http://scripts.sil.org/OFL)

### 特別感謝

我的手、我的眼睛、我的睡眠 ΩДΩ。
