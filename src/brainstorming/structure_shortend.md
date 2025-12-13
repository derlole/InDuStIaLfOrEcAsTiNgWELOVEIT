# 📘 Aufbau des Jupyter Notebooks – Vorhersage klassischer vs. moderner Modelle

## 1. Einleitung
- Kurze Beschreibung des Problems (z. B. Energieverbrauch / Durchsatz / Ausfallraten)
- Was ist Forecasting?
- Motivation: Warum kurz- bis mittelfristige Vorhersagen wichtig sind
- Ziel des Notebooks: Vergleich klassischer Modelle (ARIMA) mit modernen Modellen (Prophet / LSTM)

---

## 2. Datenbeschreibung
- Woher kommt der Datensatz?
- Welche Variablen enthält er?
- Zeitraum, Auflösung (minütlich / stündlich / täglich)
- Beispielhafte Tabelle/Head anzeigen

---

## 3. Explorative Datenanalyse (EDA)
- Zeitverlauf plotten
- Trend, Saisonalität, Ausreißer untersuchen
- Autokorrelationen (ACF/PACF) anzeigen
- Statistische Kennzahlen: Mittel, Varianz, Min/Max

---

## 4. Datenvorverarbeitung
- Umgang mit fehlenden Werten
- Glättung / Resampling (wenn nötig)
- Erstellung von Train/Test-Split
- Optional: Normalisierung für LSTM

---

## 5. Klassisches Modell: ARIMA
### 5.1 Theoretische Kurzbeschreibung
- Stationarität
- p, d, q Bedeutung
- Stärken / Schwächen

### 5.2 Implementierung
- ACF / PACF basierte Parameterwahl *oder*
- auto_arima, aber mit Erläuterung der gefundenen Parameter

### 5.3 Training & Evaluation
- RMSE, MAE, MAPE
- Residuenanalyse
- Plot: echte Daten vs. ARIMA-Vorhersage

---

## 6. Modernes Modell: Prophet
### 6.1 Kurzbeschreibung
- Automatische Trend- & Saisonalitätserkennung
- additive Komponenten

### 6.2 Implementierung
- Prophet Modell fitten
- Debug/Parameter anzeigen lassen

### 6.3 Evaluation
- Metriken: RMSE, MAE, MAPE
- Plot der Vorhersage und Komponenten

---

## 7. Modernes Modell: LSTM (einfach)
### 7.1 Kurzbeschreibung
- Grundidee von RNNs
- Windowing / Sequencing
- Stärken / Schwächen

### 7.2 Implementierung
- Daten normalisieren
- Fenster erzeugen
- Einfaches LSTM-Netz trainieren

### 7.3 Evaluation
- Fehler-Metriken
- Vorhersage-Plot
- Diskussion Training Time / Overfitting

---

## 8. Vergleich der Modelle
### 8.1 Ergebnisübersicht
- Tabelle mit RMSE / MAE / MAPE / Trainingszeit

### 8.2 Grafischer Vergleich
- Testdaten + alle Modellvorhersagen in einem Plot

### 8.3 Interpretation
- Welches Modell passt sich gut an?
- Wo liegen Stärken / Schwächen?

### 8.4 Bewertung im Praxiskontext
- ARIMA: schnell, gute Baseline
- Prophet: ideal für Trend/Saison
- LSTM: gut bei komplexen Mustern, aber datenhungrig

### 8.5 Finales Urteil
- Welches Modell am sinnvollsten für diesen Datensatz?

---

## 9. Fazit
- Welche Erkenntnisse wurden gewonnen?
- Grenzen der Modelle
- Ausblick (z. B. bessere LSTMs, Hyperparameter-Tuning, Exogene Variablen)

---

## 10. Anhang / Zusatzanalysen
- Code für AC/PCF
- Residuenplots
- Alternate Modelle wie SARIMA
