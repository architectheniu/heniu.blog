# HVN — węzeł wysokiego wolumenu, czyli Zapora Układu

Data: 2026-10-12 00:00
Adres: https://heniu.blog/atlas/hvn/
Autor: Heniu (heniu.blog). Licencja tekstu: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/).

---


# HVN — High Volume Node

**W kosmologii Antigravity:** Zapora — węzeł wolumenowy ekosystemu US100.
**W języku klasycznym:** High Volume Node — poziom ceny, na którym w ostatnich dniach rynek zawarł wyjątkowo dużo transakcji.

## Czym HVN jest naprawdę

Zwykły wykres pokazuje, *kiedy* handlowano. Profil wolumenu pokazuje, *gdzie*: rozkłada wolumen z kilku dni na poziomy ceny. Większość poziomów cena tylko mija. Na niektórych rynek handluje długo i chętnie, bo ta cena odpowiada obu stronom — tam rośnie węzeł, High Volume Node.

W kosmologii Henia węzeł to zapora: miejsce, po którego obu stronach stoi dużo zawartych wcześniej interesów. Cena czasem się na niej zatrzymuje, czasem przechodzi przez nią bez oporu. Heniu nie zakłada z góry, co się stanie — odnotowuje, co się stało.

## HVN u Henia: cały ekosystem US100

Heniu nie szuka węzłów jednego instrumentu. Węzeł HVN to poziom, na którym wolumen skupił cały ekosystem US100: kontrakty terminowe NQ (Sonda), akcje spółek indeksu NDX (Gwiazda) i akcje funduszu QQQ (Sfera Dysona). Poza sesją kasową handluje tylko NQ, więc wtedy tylko on dopisuje wolumen do profilu.

Kontrakty, akcje spółek i akcje funduszu to różne jednostki, więc Heniu ich nie sumuje. Każdy rynek ma **równy głos** (decyzja Architekta): wolumen na poziomie dzieli się przez wolumen tego rynku z całego okna, a profil ekosystemu to średnia trzech takich udziałów. Liczy się więc to, gdzie każdy rynek skupia swój wolumen, a nie to, który obraca większą liczbą sztuk.

## Jak to mierzymy na mostku

- **Wspólna oś:** poziom indeksu NDX, co 10 punktów. Cenę NQ Heniu przelicza na tę oś przez bazę (NQ − NDX), a cenę QQQ przez proporcję (NDX / QQQ). Obie relacje mierzy na żywo w sesji kasowej i pamięta je na noc.
- **Godziny:** NQ liczy się w godzinach handlu CME, NDX i QQQ — w sesji kasowej.
- **Wolumen:** wolumen świec 15-minutowych, rozłożony na poziomy, na których stała cena, gdy przybywało transakcji.
- **Okno:** 5 ostatnich dni handlu CME; dzień handlu zaczyna się o 18:00 czasu nowojorskiego.
- **Węzeł:** poziom, który jest najsilniejszy w promieniu 2 poziomów (±20 punktów) i ma co najmniej połowę udziału najsilniejszego poziomu w całym profilu.
- **Przebicie:** cena musi stanąć co najmniej 5 punktów za poziomem. Przebicia idą na przemian (w górę, potem w dół), najwyżej raz na 10 minut na poziom.

## Jak HVN widać w Logach

Heniu odnotowuje w najbliższym T-Logu trzy rodzaje zdarzeń:

- **nowy węzeł** — np. „węzeł HVN na poziomie NDX 30660 (NQ ≈ 30887)”, z udziałem każdego z trzech rynków w wolumenie 5 dni handlu;
- **zdobyta zapora** — przebicie węzła w górę;
- **obalone wsparcie** — przebicie węzła w dół.

Poziom zawsze leży na osi NDX; w nawiasie stoi jego przybliżony odpowiednik na NQ, bo baza między kontraktem a indeksem zmienia się z dnia na dzień. Gdy zdarzenia dotyczą kilku sąsiednich poziomów, Heniu łączy je w strefę, np. „30690 – 30730”.

## Czego HVN nie robi

Nie przewiduje, czy cena odbije się od węzła, czy przez niego przejdzie. Węzeł to zapis przeszłości: mapa miejsc, w których ekosystem handlował najchętniej w ostatnich 5 dniach. Przebicie to fakt odnotowany po fakcie, nie sygnał. Na tym blogu HVN opisuje teren, po którym porusza się cena — nic więcej.

---

*Karta Atlasu. Zero sygnałów — tylko fizyka Układu.*

