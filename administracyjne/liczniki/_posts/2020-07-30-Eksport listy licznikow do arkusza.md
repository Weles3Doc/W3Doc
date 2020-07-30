---
title: Eksport listy liczników do arkusza
---
# Eksport listy liczników do arkusza

Z systemu można wygenerować arkusz z danymi liczników, który jest bardzo pomocny przy imporcie odczytów oraz prognoz lub wprowadzaniu wymiany liczników. Aby to zrobić, należy przejść do:

- Zakładka `Administracja` > menu `Funkcje` > `Wydruki`.
- Zakładka `Zasób`.
- Dodajemy wydruk `Lista odczytywania liczników`.
- Pole `Typ` > `Lista importu`.
- Pole `Bez grup liczników` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Bez typów właścicieli` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Sortowanie` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Format` > `CSV (;) - Excel`.
- Klikamy: Podgląd wydruku.

Pobieramy plik i otwieramy go w arkuszu kalkulacyjnym. Znajdują się w nim następujące kolumny:

- `MIE` > numer lokalu w systemie.
- `NR` > numer licznika w systemie.
- `TYP` > typ licznika.
- `LOKALIZACJA` > lokalizacja uzupełniona w systemie.
- `OB_WAR` > obecna wartość odczytu.
- `OB_PROG` > obecna wartość prognozy.
- `DT_OB_WAR` > data obecnej wartości odczytu.
- `DT_OB_PROG` > data, od której obowiązuje prognoza na liczniku.
- `OB_ODC_PROG` > odczyt prognozowany.
- `DATA` > miejsce na uzupełnienie daty nowego odczytu.
- `WAR` > miejsce na nowy odczyt.

Formatując i pozostawiając tylko kolumny: `MIE NR TYP DATA WAR` można w szybki sposób stworzyć tabelkę do importu odczytów.

![Lista liczników](listalicznikow.gif)