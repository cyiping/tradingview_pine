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

# 移動平均クロスオーバー戦略 (Moving Average Crossover Strategy)

## 戦略説明

### 1. 買い条件
月移動平均線が四半期移動平均線を上回ったとき、1単位の資金を購入します。

### 2. 売り条件
月移動平均線が四半期移動平均線を下回ったとき、1単位の資金を売却します。

### 3. テスト期間
過去2年間 (2022年1月1日から2023年12月31日まで)。

---

## Pine Script ロジック構造

### 1. 入力パラメータ
- 月移動平均期間: デフォルトは20日間。
- 四半期移動平均期間: デフォルトは60日間。

### 2. 指標の計算
- 月移動平均: 終値を使用して計算された単純移動平均 (SMA)。
- 四半期移動平均: 終値を使用して計算された単純移動平均 (SMA)。

### 3. シグナルの判定
- **買いシグナル**: 月移動平均線が四半期移動平均線を上抜けたときに発生します。
- **売りシグナル**: 月移動平均線が四半期移動平均線を下抜けたときに発生します。

### 4. トレード条件
- **エントリー**: 買いシグナルが発生した場合、1単位の資金でロングポジションに入ります。
- **エグジット**: 売りシグナルが発生した場合、すべてのポジションをクローズします。

### 5. 時間範囲の制限
- 戦略はテスト期間内 (2022年1月1日から2023年12月31日まで) のみ実行されます。

### 6. 可視化
- 月移動平均線 (青) をプロット。
- 四半期移動平均線 (赤) をプロット。

---

## 拡張戦略の提案

1. 短期移動平均線を10日に調整して感度を高める。
2. 取引量フィルターを追加して、流動性の低い環境を回避する。
3. RSIを売買シグナルの確認に加える。
4. 利益を保護するためにトレーリングストップを追加する。
5. テスト期間を5年間に拡大して、戦略の安定性を検証する。

---

# Moving Average Crossover Strategy

## Strategy Description

### 1. Buy Condition
When the monthly MA crosses above the quarterly MA, buy 1 unit of capital.

### 2. Sell Condition
When the monthly MA crosses below the quarterly MA, sell 1 unit of capital.

### 3. Test Time Range
Last two years (from January 1, 2022, to December 31, 2023).

---

## Pine Script Logic Structure

### 1. Input Parameters
- Monthly MA Period: Default 20 days.
- Quarterly MA Period: Default 60 days.

### 2. Indicator Calculation
- Monthly MA: Simple moving average (SMA) calculated from closing prices.
- Quarterly MA: Simple moving average (SMA) calculated from closing prices.

### 3. Signal Detection
- **Buy Signal**: Triggered when the monthly MA crosses above the quarterly MA.
- **Sell Signal**: Triggered when the monthly MA crosses below the quarterly MA.

### 4. Trading Conditions
- **Entry**: Enter a long position with 1 unit of capital when the buy signal triggers.
- **Exit**: Close all positions when the sell signal triggers.

### 5. Time Range Limitation
- The strategy operates only within the test time range (from January 1, 2022, to December 31, 2023).

### 6. Visualization
- Plot the monthly MA (blue).
- Plot the quarterly MA (red).

---

## Extended Strategy Suggestions

1. Adjust the short-term MA to 10 days for increased sensitivity.
2. Add a volume filter to avoid low-liquidity environments.
3. Include RSI confirmation for buy and sell signals.
4. Add a trailing stop to protect gains.
5. Extend the test period to 5 years for strategy stability validation.

---

# Gleitender Durchschnitt Kreuzungsstrategie (Moving Average Crossover Strategy)

## Strategie-Beschreibung

### 1. Kaufbedingungen
Wenn der monatliche GD den vierteljährlichen GD nach oben durchkreuzt, kaufe 1 Einheit Kapital.

### 2. Verkaufsbedingungen
Wenn der monatliche GD den vierteljährlichen GD nach unten durchkreuzt, verkaufe 1 Einheit Kapital.

### 3. Testzeitraum
Letzte zwei Jahre (vom 1. Januar 2022 bis zum 31. Dezember 2023).

---

## Pine Script Logikstruktur

### 1. Eingabeparameter
- Monatlicher GD-Zeitraum: Standardmäßig 20 Tage.
- Vierteljährlicher GD-Zeitraum: Standardmäßig 60 Tage.

### 2. Indikatorenberechnung
- Monatlicher GD: Einfacher gleitender Durchschnitt (SMA), berechnet aus Schlusskursen.
- Vierteljährlicher GD: Einfacher gleitender Durchschnitt (SMA), berechnet aus Schlusskursen.

### 3. Signalbestimmung
- **Kaufsignal**: Ausgelöst, wenn der monatliche GD den vierteljährlichen GD nach oben durchkreuzt.
- **Verkaufssignal**: Ausgelöst, wenn der monatliche GD den vierteljährlichen GD nach unten durchkreuzt.

### 4. Handelsbedingungen
- **Einstieg**: Eröffnung einer Long-Position mit 1 Einheit Kapital bei einem Kaufsignal.
- **Ausstieg**: Schließen aller Positionen bei einem Verkaufssignal.

### 5. Zeitbeschränkung
- Die Strategie operiert nur im Testzeitraum (vom 1. Januar 2022 bis zum 31. Dezember 2023).

### 6. Visualisierung
- Zeichnen Sie den monatlichen GD (blau).
- Zeichnen Sie den vierteljährlichen GD (rot).

---

## Erweiterte Strategie-Vorschläge

1. Passen Sie den kurzfristigen GD auf 10 Tage an, um die Empfindlichkeit zu erhöhen.
2. Fügen Sie einen Volumenfilter hinzu, um Umgebungen mit geringer Liquidität zu vermeiden.
3. Integrieren Sie den RSI-Indikator, um Kauf- und Verkaufssignale zu bestätigen.
4. Fügen Sie einen Trailing-Stop hinzu, um Gewinne zu schützen.
5. Erweitern Sie den Testzeitraum auf 5 Jahre, um die Stabilität der Strategie zu überprüfen.
