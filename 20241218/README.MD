# 均線交叉策略 (Moving Average Crossover Strategy)

## 1. 策略條件說明
1.1 **買入條件**: 月線向上穿越季線。
1.2 **賣出條件**: 月線向下穿越季線。
1.3 **測試時間範圍**: 最近兩年。


## 2. Pine Script 邏輯架構
2.1 輸入參數：月線、季線的週期設置。
2.2 計算指標：使用 SMA (Simple Moving Average) 計算月線與季線。
2.3 信號判斷：檢測均線交叉點。
2.4 交易條件：在交叉點時觸發買入/賣出信號。
2.5 限制時間範圍：設定交易日期範圍。
2.6 視覺化要求：在圖表上顯示月線、季線與買賣信號。

---

## 条件説明 (日本語)
1. **買い条件**: 月線が季線を上抜け。
2. **売り条件**: 月線が季線を下抜け。
3. **テスト期間**: 過去2年。

---

## Strategy Conditions (English)
1. **Buy Condition**: Month MA crosses above Quarter MA.
2. **Sell Condition**: Month MA crosses below Quarter MA.
3. **Test Time Range**: Last two years.

---

## Strategiebeschreibung (Deutsch)
1. **Kaufbedingung**: Monat MA kreuzt über Quartal MA.
2. **Verkaufsbedingung**: Monat MA kreuzt unter Quartal MA.
3. **Testzeitraum**: Letzte zwei Jahre.
