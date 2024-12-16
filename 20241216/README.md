# Pine Script : BBand 波段突破策略

---

## 1. 條件說明

- **買入條件**
  - 前一根 K 線的收盤價低於 Bollinger Bands 的下緣。
  - 當前 K 線的收盤價也低於 Bollinger Bands 的下緣。
  - 符合以上條件時觸發買入信號。

- **賣出條件**
  - 前一根 K 線的收盤價高於 Bollinger Bands 的上緣。
  - 當前 K 線的收盤價也高於 Bollinger Bands 的上緣。
  - 符合以上條件時觸發賣出信號。

- **測試時間範圍**
  - 從 **2021/12/15** 到 **2024/12/15**。
  - 超出此時間範圍的資料將被忽略，並在範圍外關閉所有持倉。

---

## 2. Pine Script 邏輯架構

### **輸入參數**
- 使用者可調整的 Bollinger Bands 長度（`length`）與倍數（`mult`）。

### **計算指標**
- 利用移動平均線與標準差計算 Bollinger Bands 的中軌、上軌及下軌。

### **信號判斷**
- 判斷前一根 K 線是否在上軌或下軌之外。
- 判斷當前 K 線是否也在上軌或下軌之外。

### **交易條件**
- 若滿足買入條件則進場做多。
- 若滿足賣出條件則進場放空。

### **限制時間範圍**
- 透過 `timestamp` 限制回測的日期範圍。

### **視覺化**
- 在圖表上標記買入與賣出的信號，以方便觀察。

---

# Pine Script : BBand ブレイクアウト戦略


![2330 TSMC](/20241216/2330.png)

---

## 1. 条件説明

- **買い条件**
  - 前のローソク足の終値がボリンジャーバンドの下限を下回っている。
  - 現在のローソク足の終値もボリンジャーバンドの下限を下回っている。
  - 上記の条件を満たした場合、買いシグナルを発生させる。

- **売り条件**
  - 前のローソク足の終値がボリンジャーバンドの上限を上回っている。
  - 現在のローソク足の終値もボリンジャーバンドの上限を上回っている。
  - 上記の条件を満たした場合、売りシグナルを発生させる。

- **テスト期間**
  - **2021/12/15** から **2024/12/15** まで。
  - この期間外のデータは無視され、ポジションは自動的にクローズされる。

---

## 2. Pine Script ロジック構造

### **入力パラメータ**
- ボリンジャーバンドの長さ（`length`）と倍率（`mult`）を調整可能。

### **指標計算**
- 移動平均線と標準偏差を使用してボリンジャーバンドの中央線、上限、下限を計算。

### **シグナル判定**
- 前のローソク足が上限または下限を超えたかを判定。
- 現在のローソク足も上限または下限を超えているかを判定。

### **取引条件**
- 買い条件を満たす場合、ロングポジションを開始する。
- 売り条件を満たす場合、ショートポジションを開始する。

### **期間制限**
- `timestamp` を使用してテスト期間を制限。

### **視覚化**
- チャート上に買いと売りのシグナルを表示し、確認しやすくする。

---

# Pine Script: BBand Ausbruchsstrategie

---

## 1. Bedingungsbeschreibung

- **Kaufbedingungen**
  - Der Schlusskurs der vorherigen Kerze liegt unterhalb der unteren Bollinger-Band-Grenze.
  - Der Schlusskurs der aktuellen Kerze liegt ebenfalls unterhalb der unteren Bollinger-Band-Grenze.
  - Wenn diese Bedingungen erfüllt sind, wird ein Kaufsignal ausgelöst.

- **Verkaufsbedingungen**
  - Der Schlusskurs der vorherigen Kerze liegt oberhalb der oberen Bollinger-Band-Grenze.
  - Der Schlusskurs der aktuellen Kerze liegt ebenfalls oberhalb der oberen Bollinger-Band-Grenze.
  - Wenn diese Bedingungen erfüllt sind, wird ein Verkaufssignal ausgelöst.

- **Testzeitraum**
  - Vom **15.12.2021** bis **15.12.2024**.
  - Daten außerhalb dieses Zeitraums werden ignoriert, und alle Positionen werden außerhalb des Zeitraums geschlossen.

---

## 2. Pine Script Logikstruktur

### **Eingabeparameter**
- Benutzerdefinierte Einstellung für die Länge der Bollinger-Bänder (`length`) und den Multiplikator (`mult`).

### **Indikatorberechnung**
- Berechnung der mittleren Linie sowie der oberen und unteren Bollinger-Band-Grenzen mithilfe von gleitenden Durchschnitten und Standardabweichungen.

### **Signalerkennung**
- Überprüfung, ob der Schlusskurs der vorherigen Kerze außerhalb der oberen oder unteren Grenzen liegt.
- Überprüfung, ob der Schlusskurs der aktuellen Kerze ebenfalls außerhalb der oberen oder unteren Grenzen liegt.

### **Handelsbedingungen**
- Wenn die Kaufbedingungen erfüllt sind, wird eine Long-Position eröffnet.
- Wenn die Verkaufsbedingungen erfüllt sind, wird eine Short-Position eröffnet.

### **Zeitbegrenzung**
- Einschränkung des Testzeitraums mithilfe von `timestamp`.

### **Visualisierung**
- Markierung von Kauf- und Verkaufssignalen auf dem Diagramm, um die Analyse zu erleichtern.

---

# Pine Script: BBand Breakout Strategy

---

## 1. Conditions Description

- **Buy Condition**
  - The closing price of the previous candlestick is below the lower Bollinger Band.
  - The closing price of the current candlestick is also below the lower Bollinger Band.
  - When these conditions are met, a buy signal is triggered.

- **Sell Condition**
  - The closing price of the previous candlestick is above the upper Bollinger Band.
  - The closing price of the current candlestick is also above the upper Bollinger Band.
  - When these conditions are met, a sell signal is triggered.

- **Backtesting Time Range**
  - From **2021/12/15** to **2024/12/15**.
  - Data outside this time range will be ignored, and all positions will be closed outside this range.

---

## 2. Pine Script Logic Framework

### **Input Parameters**
- Adjustable Bollinger Band length (`length`) and multiplier (`mult`) by the user.

### **Indicator Calculation**
- Calculate the middle, upper, and lower Bollinger Bands using moving averages and standard deviation.

### **Signal Detection**
- Check if the previous candlestick closes outside the upper or lower band.
- Check if the current candlestick also closes outside the upper or lower band.

### **Trading Conditions**
- Enter a long position if the buy condition is satisfied.
- Enter a short position if the sell condition is satisfied.

### **Time Range Restriction**
- Use `timestamp` to restrict the backtesting date range.

### **Visualization**
- Mark buy and sell signals on the chart for better observation.

---

