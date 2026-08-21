---
title: "NDX CVD — Agregacja Delty Wolumenu Indeksu Kasowego"
date: 2026-08-21
draft: false
tags: ["atlas", "NDX CVD", "order flow", "agregacja", "mikrostruktura"]
---

# NDX CVD — Agregacja Delty Wolumenu Indeksu

**W kosmologii Antigravity:** Paliwo Gwiazdy Centralnej (NDX).
**W języku klasycznym:** Agregowana, ważona skumulowana delta wolumenu (CVD) dla 100 spółek wchodzących w skład indeksu NASDAQ-100.

## Jak powstaje NDX CVD

Indeks NASDAQ-100 sam w sobie jest koszykiem papierów wartościowych, a nie pojedynczą akcją. Wskaźnik **NDX CVD** w telemetrii Henia obliczany jest w następujący sposób:

1. **Feed transakcyjny:** Ciągły odczyt transakcji z giełd dla każdego ze 100 komponentów indeksu.
2. **Klasyfikacja transakcji:** Zlecenia realizowane po cenie Ask (agresywny popyt) dodają wolumen; zlecenia po cenie Bid (agresywna podaż) odejmują wolumen.
3. **Agregacja i ważenie:** Wolumeny są sumowane w czasie rzeczywistym z uwzględnieniem wag komponentów w indeksie, tworząc jedną syntetyczną linię przepływu energii dla całego rynku kasowego.
4. **Reset sesyjny:** Linia CVD jest zerowana na otwarciu sesji kasowej o 9:30 ET (15:30 czasu polskiego), co pozwala mierzyć czysty bilans walki popytu i podaży dla bieżącego dnia.

## Interpretacja jednostek

Wartości podawane w raportach (np. `+162,49M` lub `-175,43M`) oznaczają sumaryczną liczbę akcji netto kupionych/sprzedanych agresywnie w trakcie trwania danej sesji.

* **Dywergencja NDX / CVD:** Jeżeli cena indeksu spada, a NDX CVD rośnie, wskazuje to na pasywną absorpcję podaży przez zlecenia z limitem. Jeżeli cena rośnie przy ujemnym CVD, wskazuje to na pasywną dystrybucję podaży w popyt rynkowy.

---

*Karta Atlasu. Zero sygnałów — tylko fizyka Układu.*
