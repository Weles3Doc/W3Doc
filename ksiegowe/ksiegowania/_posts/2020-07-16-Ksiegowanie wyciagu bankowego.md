---
title: Księgowanie wyciągu bankowego
---

# Księgowanie wyciągu bankowego

Wprowadzanie wyciągu bankowego jest robione przez dedykowaną, uproszczoną formatkę do wprowadzania dekretów. Aby zaksięgować operacje bankowe, należy przejść do:

- Zakładka `Dekrety` > menu `Dokumenty` > `Dodaj wyciąg bankowy`.

W nagłówku okna uzupełniamy podstawowe pola dotyczace dekretu:

- Pole `Konto` > wybieramy rachunek bankowy, dla którego będziemy wprowadzać wpłaty.
- Pole `Data księgowania` > określamy datę księgowania dekretu.
- Pole `Opis dokumentu` > można zastosować wzór: `WB MM-RRRR`.
- Pole `Domykanie konta` > można wybrać, czy wprowadzone pozycje mają być zbilansowane jedną pozycją na koncie 131-xx (`Zbiorczo`) lub czy każda pozycja ma być bilansowana osobno (`Indywidualnie`), zostało to dokładniej wytłumaczone na końcu instrukcji.

Następnie przechodzimy do wprowadzania pozycji:

- Pole `LP` > będzie się powiększało automatycznie.
- Pole `Data pozycji` > ustawiamy datę operacji bankowej.
- Pole `Operacja` > określamy czy wprowadzana pozycja jest operacją przychodzącą (uznaniem), czy wychodzącą (obciążeniem).
- Pola `Konto Wn` lub `Konto Ma` > w zależności od wybranego typu operacji, określamy konto:
  - `Wpłata` — Wpłata właściciela — `Konto Ma` — 201-1-0000001-1.
  - `Wpłata` — Odsetki — `Konto Ma` — 760-xx Przychody finansowe.
  - `Wypłata` — Zapata kontrahentowi — `Konto Wn` — 202-xxxxxxxxx.
  - `Wypłata` — Prowizje bankowe — `Konto Wn` — 400-2-001-xxx Koszty bankowe lub 761-xx Koszty finansowe.
- Pole `Treść` > opisujemy operację.
- Pole `Wartość` > podajemy kwotę operacji.
- Klikamy: `Dodaj`.

Wprowadzamy wszystkie następne operacje. Gdy wszystkie pozycje będą dodane na koniec:

- Klikamy: `Zatwierdź`.

Do wprowadzania operacji bankowych można w każdej chwili powrócić, zaznaczając dokument > menu `Dokumenty` > `Edytuj dokument`.

![Księgowanie WB](ksiegowaniewb.gif)

#### Wyciągi z różnych rachunków

W jednym dekrecie wprowadzamy tylko i wyłącznie obroty jednego rachunku bankowego, w związku z tym, na każde księgowanie operacji innego rachunku, tworzymy osobny dekret WB. Przepływy pieniężne pomiędzy różnymi rachunkami bankowymi, księgujemy przez konto `149-01 Środki pieniężne w drodze`.

![Księgowanie WB](ksieg_wb_wiele_rach.png)

#### Prowadzenie wyciągów

Zdecydowanie większość użytkowników prowadzi operacje bankowe zasobu w jednym dekrecie w miesiącu (na rachunek). Ten dekret zazwyczaj jest tworzony z ostatnim dniem miesiąca. Gdy wpłyną nowe operacje bankowe do zaksięgowania, są one dodawane przez `Edytuj dokument`. Poniżej przykład:

![Księgowanie WB](ksieg_wb_jed_dekret.png)

Wyciągi można też rejestrować pojedynczo, na każdy dzień, w którym są do zaksięgowania pozycje. Przykład poniżej:

![Księgowanie WB](ksieg_wb_wiele_dekret.png)

#### Domykanie konta

Pole `Domykanie konta` odpowiada za to w jaki sposób pozycje wprowadzone w dekrecie są reprezentowane po stronie konta `13x`. Jeśli wybierzemy:

- `Zbiorczo` > system będzie agregował pozycje na dzień oraz dla każdej strony Wn/Ma.

![Księgowanie WB](ksieg_wb_domyk_zbiroczo.png)

- `Indywidualnie` > każda pozycja będzie osobno wyszczególniona na koncie `13x`.

![Księgowanie WB](ksieg_wb_domyk_ind.png)