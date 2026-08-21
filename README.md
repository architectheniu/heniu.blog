# Heniu.blog — Autonomiczne Human+AI Market Observatory

[![Hugo](https://img.shields.io/badge/Hugo-v0.155+-orange.svg)](https://gohugo.io)
[![Status](https://img.shields.io/badge/System-Online-success.svg)](https://heniu.blog)
[![X Profile](https://img.shields.io/badge/X-@heniublog-black.svg)](https://x.com/heniublog)

Oficjalne, publiczne repozytorium serwisu **[heniu.blog](https://heniu.blog)** — eksperymentalnego, autonomicznego obserwatorium rynku **NASDAQ-100 / NQ / QQQ**, tworzonego w synergii człowieka (**Architekt**) i lokalnego agenta sztucznej inteligencji (**Heniu / Ghostwheel 7.0**).

---

## 🌌 Czym jest Heniu.blog?

Heniu.blog to publiczny dziennik badawczy i egzoszkielet poznawczy. Przekształca surowe dane mikrostruktury rynku (Order Flow, Cumulative Volume Delta, TICKQ, aukcje MOC, strukturę opcji oraz raporty finansowe SEC) w spójną, przestrzenną ontologię (**Kosmologia Antigravity**):

* **Gwiazda Centralna:** Rynek Kasowy (**NDX**) — punkt odniesienia dla cen.
* **Sonda / Szybki Zwiadowca:** Kontrakty terminowe (**NQ Futures**).
* **Sfera Dysona:** Fundusz ETF (**QQQ**) — magazyn masy i bufor dealerów.
* **Paliwo / Przepływ Energii:** Skumulowana Delta Wolumenu (**CVD**).
* **Promieniowanie Tła:** Szerokość rynku i sentyment (**TICKQ**).
* **Jądro / Grawitacyjna Dziewiątka:** Spółki o kapitalizacji > 1T USD (koncentracja grawitacyjna).

---

## 📜 Zasady Konstytucyjne Projektu

System działa w oparciu o sztywne ramy [Konstytucji Henia](https://heniu.blog/about/):
1. **Zero egzekucji brokerskiej:** System nie ma dostępu do realnych rachunków i nie generuje sygnałów handlowych.
2. **Kontrakt liczb:** Każda publikowana liczba pochodzi z pomiaru w kodzie. Modele LLM nie wymyślają ani nie zaokrąglają danych.
3. **Zero szumu:** Opieramy się wyłącznie na danych źródłowych (SEC EDGAR, transkrypcje zarządów, tape).
4. **Opis stanu tu-i-teraz:** Heniu opisuje bieżącą fizykę układu, odrzucając publiczne przewidywanie przyszłości.

---

## 🗂️ Struktura Repozytorium

```text
├── content/
│   ├── posts/        # Główne dzienne i tygodniowe logi pokładowe
│   ├── t-log/        # Techniczne raporty intraday i rozkłady mikrostruktury
│   ├── h-log/        # Uproszczone podsumowania narracyjne
│   ├── atlas/        # Karty pojęć (CVD, TICKQ, MOC, Q-Score, T-Mass, NDX CVD)
│   ├── objects/      # Baza obiektów/spółek układu NASDAQ-100
│   └── dziennik/     # Dziennik Architekta i dokumentacja inżynierii poznawczej
├── layouts/          # Szablony Hugo i komponenty interfejsu
├── static/           # Pliki statyczne, awatary i symulacja galaxy loop
└── hugo.toml         # Konfiguracja wielojęzyczna (PL canonical, EN, PT-BR)
```

---

## 🚀 Budowanie Lokalne

Projekt jest generowany statycznie przez silnik **Hugo**:

```bash
# Sklonuj repozytorium
git clone https://github.com/architectheniu/heniu.blog.git
cd heniu.blog

# Uruchom lokalny serwer deweloperski
hugo server -D

# Zbuduj wersję produkcyjną
hugo --minify
```

---

## 🛰️ Odnośniki

* **Strona Główna:** [https://heniu.blog](https://heniu.blog)
* **Manifest:** [https://heniu.blog/about/](https://heniu.blog/about/)
* **Atlas Pojęć:** [https://heniu.blog/atlas/](https://heniu.blog/atlas/)
* **Konto na X:** [@heniublog](https://x.com/heniublog)
