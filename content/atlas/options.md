---
title: "Opcje QQQ i Sfera Dysona — IV, Put/Call Ratio i Zasięg Oczekiwany"
date: 2026-08-21
draft: false
tags: ["atlas", "opcje", "QQQ", "IV", "Put/Call", "Expected Move", "Sfera Dysona"]
---

# Opcje QQQ i Sfera Dysona (Options Surface)

**W kosmologii Antigravity:** Sfera Dysona / Tarcze Grawitacyjne i Pole Zmienności.
**W języku klasycznym:** Parametry powierzchni zmienności implikowanej (IV), struktury wolumenu opcji oraz wycenianego przez rynek zasięgu wahań (Expected Move) na funduszu ETF QQQ.

## Czym jest Sfera Dysona

Fundusz ETF Invesco QQQ Trust (QQQ) jest głównym wehikułem płynnościowym i zabezpieczającym dla indeksu NASDAQ-100. Rynek opcji na QQQ stanowi ogromny bufor hedgingowy, w którym animatorzy rynku (dealerzy) i inwestorzy instytucjonalni handlują ryzykiem zmienności.

## Kluczowe metryki publikowane w telemetrii

### 1. Zmienność Implikowana (Implied Volatility — IV)
* **Co mierzy:** Roczna zmienność implikowana (30-day IV composite / at-the-money) wyliczana z bieżących cen rynkowych opcji.
* **Znaczenie:** Wyższa IV oznacza droższe premie opcyjne i rynkowe oczekiwanie gwałtowniejszych wahań cenowych; niska IV oznacza kompresję zmienności i względny spokój w wycenach opcji.

### 2. Put/Call Volume Ratio (Stosunek Wolumenu Put do Call)
* **Definicja:** Stosunek liczby zrealizowanych kontraktów opcyjnych typu Put do Call na danym instrumencie w trakcie sesji:
  $$ \text{P/C Ratio} = \frac{\text{Wolumen Put}}{\text{Wolumen Call}} $$
* **Rygor interpretacyjny:** Wartość `P/C = 1.32` oznacza wyłącznie, że wolumen zawartych putów był 1,32-krotnie wyższy niż calli. **Wskaźnik ten NIE dowodzi jednoznacznie kierunku ani intencji:**
  - Może oznaczać kupowanie putów (hedging / zabezpieczenie portfeli lub spekulacja na spadek),
  - Może oznaczać sprzedaż putów (inkasowanie premii / zlecenia bycze ze strony dealerów),
  - Może wynikać ze złożonych strategii spreadowych lub arbitrażu.
  Dlatego na mostku Henia P/C traktowany jest jako **surowa asymetria wolumenowa**, a nie wyrocznia nastrojów.

### 3. Zasięg Oczekiwany (Expected Move)
* **Definicja:** Statystyczne pasmo wahań cenowych implikowane przez ceny opcji na dany horyzont czasowy:
  $$ \text{Expected Move} \approx \text{Cena} \times \text{IV} \times \sqrt{\frac{\text{DTE}}{365}} $$
* **W logach:** Publikowane pasmo (np. `Zasięg 703,27 – 718,59`) reprezentuje obszar standardowego odchylenia ($\pm 1\sigma$), w którym rynek opcyjny wycenia ~68% prawdopodobieństwa zamknięcia ceny do daty wygaśnięcia.

## Czego Opcje nie robią

Struktura opcyjna nie jest twardą barierą nie do przebicia. Wybicia poza Zasięg Oczekiwany (tzw. zdarzenia gamma) zdarzają się regularnie przy nagłych impulsach makroekonomicznych.

---

*Karta Atlasu. Zero sygnałów — tylko fizyka Układu.*
