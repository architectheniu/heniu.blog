---
title: "NDX CVD — Agregacja Delty Wolumenu Indeksu Kasowego"
date: 2026-08-21
draft: false
tags: ["atlas", "NDX CVD", "order flow", "agregacja", "mikrostruktura"]
---

# NDX CVD — Agregacja Delty Wolumenu Indeksu

**W kosmologii Antigravity:** Paliwo Gwiazdy Centralnej (NDX).
**W języku klasycznym:** Indeksowo ważona skumulowana delta wolumenu (CVD) dla 100 komponentów indeksu NASDAQ-100.

## Jak powstaje NDX CVD

Indeks NASDAQ-100 jest koszykiem papierów wartościowych, a nie pojedynczym instrumentem giełdowym. Wskaźnik **NDX CVD** w telemetrii Henia obliczany jest w następujący sposób:

1. **Feed transakcyjny:** Ciągły odczyt transakcji z giełd dla każdego ze 100 komponentów indeksu.
2. **Klasyfikacja transakcji (Tick Rule / BBO):** Transakcje zawarte po cenie Ask (agresywny popyt rynkowy) dodają wolumen (+); transakcje po cenie Bid (agresywna podaż rynkowa) odejmują wolumen (-).
3. **Ważenie indeksowe i agregacja:** Wolumeny komponentów są sumowane w czasie rzeczywistym z uwzględnieniem wag indeksowych:
   $$ \text{CVD}_{NDX} = \sum_{i=1}^{100} w_i \cdot (\text{Vol}_{\text{Ask}, i} - \text{Vol}_{\text{Bid}, i}) $$
   gdzie $w_i$ to waga spółki w indeksie. Dzięki temu ruchy megacapów (np. Apple, NVIDIA) mają proporcjonalny wpływ na wypadkowy wskaźnik, odzwierciedlając strukturę indeksu.
4. **Reset sesyjny:** Linia CVD jest zerowana na otwarciu sesji kasowej o 9:30 ET (15:30 czasu polskiego), mierząc bilans agresji rynkowej dla bieżącej sesji spot.

## Jednostka i interpretacja semantyczna

* **Jednostka:** Wartości podawane w raportach (np. `+162,49M` lub `-175,43M`) reprezentują **NDX Weighted Flow Units (indeksowo ważone jednostki wolumenu agresywnego)**. Ze względu na ważenie wagami indeksu nie jest to surowa, prosta suma sztuk akcji, lecz znormalizowany wektor presji agresywnej.
* **CVD to NIE „napływ kapitału”:** W każdej transakcji giełdowej następuje symetryczna wymiana gotówki i akcji. CVD nie mierzy salda wpłat do systemu, lecz **signed aggressive order flow** — informuje, która strona rynku (kupujący czy sprzedający) była bardziej zdeterminowana, by płacić spread i uderzać zleceniami rynkowymi w zlecenia oczekujące (limit).
* **Dywergencja NDX / CVD:** 
  - Cena spada, a NDX CVD rośnie: pasywna absorpcja agresywnej sprzedaży przez zlecenia z limitem kupna (akumulacja w dołku).
  - Cena rośnie przy ujemnym CVD: pasywna dystrybucja zleceń sprzedaży w napływający popyt rynkowy.

---

*Karta Atlasu. Zero sygnałów — tylko fizyka Układu.*
