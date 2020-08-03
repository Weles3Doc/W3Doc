---
title: Wyliczenie prognoz liczników
---
# Wyliczenie prognoz liczników

W system umożliwia automatyczne wyliczenie nowych prognoz na podstawie zużyć liczników, aby to zrobić, należy przejść do:

- Menu `Funkcje` > `Wylicz prognozy`.
- Pole `Struktura` > wybieramy cały budynek lub konkretny lokal/strukturę.
- Pole `Grupa liczników` > wybieramy grupę liczników.
- Pole `Typ licznika` > wybieramy typ licznika.
- Pole `Operacja` > ustawiamy pożądaną operację:
  - `Ustaw ryczałt` > jeśli wybierzemy tę opcję, system usunie prognozę od danej daty (ustawi pustą, brak).
  - `Ustaw zero` > system doda na liczniki prognozę równą zero do danej daty.
  - `Wycofaj zmianę` > jeśli z daną datą była zmiana prognozy na licznikach, to system przywróci poprzednią prognozę.
  - `Ustaw średnią` > system wyliczy i doda na liczniki średnią prognozę miesięczną na podstawie dalszych ustawień.
- Pole `Okres od` > ustawiamy początkowy okres, na podstawie którego system ma wyliczyć prognozy.
- Pole `Okres do` > ustawiamy końcowy okres, na podstawie którego system ma wyliczyć prognozy.
- Pole `Prognozy ujemne` > określamy systemowi, co ma zrobić w przypadku wyliczenia prognozy ujemnej:
  - `Ustaw ujemną` > wstawi ujemną prognozę.
  - `Ustaw zero` > ustawi prognozę na zero.
  - `Ustaw ryczałt` > usunie prognozę z licznika.
  - `Nie zmieniaj` > nie zmieni prognozy.
- Pole `Wymiana liczników` > ustalamy czy system ma brać pod uwagę zużycie starych liczników, w przypadku ich wymiany, do wyliczenia nowej prognozy.
- Pole `Zmiana od` > ustawiamy datę zmiany/dodania nowych prognoz.
- Klikamy: `Dodaj`.
- Dodajemy kolejną pozycję dla innego typu liczników.
- Wpisujemy hasło i zatwierdzamy.

Po zamknięciu okna, prognozy powinny być od razu widoczne. Można ew. odświeżyć system: menu `Funkcje` > `Odśwież`. Należy przeliczyć też ponownie zaliczki: menu `Obciążenia` > `Nalicz zaliczki`.

![Wyliczenie prognoz](wyliczenieprognoz.gif)

### Uwagi:

- Wyliczonych prognozy nie można dodawać od daty wstecznej.
- Wartości prognoz można wyeksportować za pomocą wydruku: menu `Funkcje` > `Wydruki` > `Zasób` > `Lista odczytywania liczników` > pole `Typ` > `Lista importu`. Ostatnia, obecna prognoza licznika jest w kolumnie OB_PROG.