# 均線交叉策略 (Moving Average Crossover Strategy)

## 策略條件說明

### 1. 買入條件
當月線向上穿越季線時，買進 1 單位資金。

### 2. 賣出條件
當月線向下穿越季線時，賣出 1 單位資金。

### 3. 測試時間範圍
最近兩年 (2022年1月1日 至 2023年12月31日)。

---

## Pine Script 邏輯架構

### 1. 輸入參數
- 月線週期：預設 20 天。
- 季線週期：預設 60 天。

### 2. 計算指標
- 月線：基於收盤價計算的簡單移動平均線 (SMA)。
- 季線：基於收盤價計算的簡單移動平均線 (SMA)。

### 3. 信號判斷
- **買入信號**：當月線向上穿越季線時產生。
- **賣出信號**：當月線向下穿越季線時產生。

### 4. 交易條件
- **進場**：當買入信號觸發時，進場 1 單位資金。
- **出場**：當賣出信號觸發時，平倉所有持倉。

### 5. 限制時間範圍
- 策略僅在測試時間範圍內運行 (2022年1月1日至2023年12月31日)。

### 6. 視覺化要求
- 繪製月線 (藍色)。
- 繪製季線 (紅色)。
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
