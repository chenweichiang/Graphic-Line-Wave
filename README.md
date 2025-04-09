# 波浪線動畫 (Graphic Line Wave)

Version 1.1.0

一個使用 HTML Canvas 實現的簡單優雅的波浪線動畫。波浪線會隨機生成，並自然地從右向左流動，呈現出平滑、連續的波動效果。

## 功能特點

- 全屏顯示的波浪線動畫
- 波浪線會自然、平滑地從右向左流動
- 每次載入頁面時，波浪線都會以隨機的振幅、頻率和位置生成
- 無抖動的平滑動畫效果
- 波浪線延伸到畫面外，視覺上更加連續
- 輕量級實現，僅使用原生 JavaScript，無需第三方庫
- 極細的線條寬度（0.5px）呈現更精緻的視覺效果

## 技術實現

- **HTML5 Canvas**: 使用 Canvas 2D Context 進行繪圖
- **數學模型**: 使用多個不同頻率、振幅和相位的正弦波疊加，創造自然隨機的波形
- **動畫優化**: 
  - 使用 requestAnimationFrame 實現高效流暢的動畫
  - 幀間平滑過渡 (85% 前一幀 + 15% 當前幀)，減少抖動
  - 使用水平偏移量實現從右至左的流動效果
  - 精細的線條寬度控制（0.5px）

## 更新日誌

### Version 1.1.0 (2024-04-20)
- 將線條寬度從 2.5px 減少到 0.5px，實現更精緻的視覺效果
- 優化了波浪線的顯示效果，使其更加細緻優雅

### Version 1.0.0
- 初始版本發布

## 如何使用

1. 克隆此倉庫:
```
git clone https://github.com/chenweichiang/Graphic-Line-Wave.git
```

2. 在瀏覽器中打開 `index.html` 文件

無需安裝其他依賴，打開即可使用。

## 開發過程中使用的 Prompt

以下是開發這個動畫過程中使用的主要提示詞（按時間順序）：

1. "把index改成只顯示全畫面的main.js" - 簡化頁面，只顯示動畫
2. "我想要讓main中的波浪是同一條線自然的隨機波動像波浪一樣" - 優化波浪的自然感
3. "線上面不要再有額外的波浪形狀" - 移除小波浪，保持單一平滑曲線
4. "讓線波動非常滑順" - 改進動畫平滑度
5. "把線上的小波浪刪掉" - 再次優化波浪形狀
6. "為什麼現在的線不是隨機的" - 添加更好的隨機性
7. "現在的線波形不夠大要再大50%" - 調整波浪大小
8. "又開始在抖動了把抖動拿掉" - 修復抖動問題
9. "這條線產生之後就會開始由右至左自然波動" - 添加從右至左的移動效果

## 可能的改進方向

- 添加顏色變化效果
- 允許用戶通過 UI 控制波浪的參數（速度、大小等）
- 添加多條不同顏色和速度的波浪線
- 在移動設備上優化性能
- 添加聲音效果，與波浪運動同步

## 授權

MIT 授權。

## 貢獻

歡迎提交問題和改進建議。