---
title: "MOC — nierównowaga na zamknięcie, czyli Anomalia MOC"
date: 2026-08-10
draft: false
tags: ["atlas", "MOC", "order flow", "mikrostruktura"]
---

# MOC — Market-On-Close Imbalance

**W kosmologii Antigravity:** Anomalia MOC / Młot MOC — grawitacyjne uderzenie w ostatnich minutach cyklu.
**W języku klasycznym:** nierównowaga zleceń na zamknięcie — nadwyżka popytu albo podaży, którą giełda musi sparować do godziny 16:00 czasu nowojorskiego.

## Czym MOC jest naprawdę

Ogromna część kapitału na rynku — fundusze indeksowe, ETF-y — z definicji rozlicza się po **cenie zamknięcia**. Ich zlecenia trafiają do specjalnej aukcji zamykającej, a giełda od 15:50 ET publikuje **nierównowagę (NOII - Net Order Imbalance Indicator)**: o ile więcej jest wolumenu do kupienia niż do sprzedania (albo odwrotnie). To jedno z najczystszych publicznych okien na jawnie zadeklarowany wolumen aukcji zamknięcia (Nasdaq Closing Cross) — przepływ w księdze aukcyjnej jest zadeklarowany, a nie domyślany.

Dlatego okno MOC bywa najgęstszą grawitacyjnie chwilą sesji: dziesiątki lub setki milionów akcji szukają drugiej strony w kilka minut. Cena zamknięcia, która z tego wynika, jest punktem odniesienia dla całego następnego dnia.

## Jak to mierzymy na mostku

Heniu odczytuje wartość netto nierównowagi w oknie MOC i traktuje ją progowo — progi są zapisane w konfiguracji na sztywno: przewaga rzędu ±50 mln to silny sygnał kierunkowej presji zamknięcia, a ±150 mln to zjawisko klasy osobliwości („Młot MOC"). Odczyt wpływa na opis wektora układu od ~15:50 czasu giełdy aż w noc — dokumentując stan bilansu zleceń na zamknięciu sesji (closing order interest).

## Czego MOC nie robi

Nie przepowiada jutrzejszej sesji — mierzy dzisiejszą presję rozliczenia. Bywa, że gigantyczny Młot MOC zostaje wchłonięty bez śladu; bywa, że mała nierównowaga kończy się dużym ruchem. Na tym blogu MOC jest opisem siły obecnej w aukcji — niczym więcej.

---

*Karta Atlasu. Zero sygnałów — tylko fizyka Układu.*
