# UART 通訊問題排查紀錄

## 問題現象
- 使用 CP2102 接至 MCU，minicom 出現大量亂碼
- 嘗試調整 baudrate、flow control 無效

## 解法過程
- 發現缺乏共地，將 GND 端子補齊後即穩定通訊
- 驗證成功 baudrate 為 921600

## 學習心得
- UART 共地為最常見通訊失敗原因之一
- minicom 可做基礎排查，但需實體硬體介面觀察最有效
