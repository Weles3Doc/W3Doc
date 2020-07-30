---
title: Import prognoz liczników
---
# Import prognoz liczników

Do systemu można wprowadzić prognozy hurtowo, za pomocą tabelki z odpowiednimi kolumnami. Tabelka do importu prognoz powinna zawierać pięć kolumn. Oczywiście, jeśli posiadamy już prognozy liczników w arkuszu, to tabelkę formatujemy do opisanej postaci. Poniżej przykładowa tabelka, którą tworzymy w arkuszu kalkulacyjnym:

![Tabelka importu prognoz](tabelkaimpprog.png)

Gdzie w kolumnach podajemy:

- `MIE` > numer lokalu z systemu musi być taki sam.
- `TYP` > podajemy typ licznika tak jak w systemie.
- `NR` > wpisujemy numer licznika.
- `DATA` > podajemy datę w formacie RRRR-MM-DD.
- `PROG` > wpisujemy wartość prognozy na wskazaną datę.

Tak przygotowaną tabelkę zaznaczamy w arkuszu, wraz z tytułami kolumn. Kopiujemy. Wklejamy do:

- Menu `Funkcje` > `Import danych` > Pole `Dane`.

Następnie wpisujemy hasło i zatwierdzamy. Okno zamknie się, po czym można sprawdzić zaimportowane wartości prognoz. Czasami potrzeba też odświeżyć system: menu `Funkcje` > `Odśwież`.

![Import prognoz](importodczytow.gif)

### Uwagi:

- Można pominąć kolumnę TYP — wtedy kolumna NR powinna mieć unikalne wartości.
- Można pominąć kolumnę NR — wtedy w lokalu może być tylko jeden licznik danego typu.
- Kolejność kolumn jest dowolna.
- Częstą przyczyną problemów z importem są znaki niepisane (np. spacja) występujące w nazwach kolumn.
- Częstą przyczyną problemów są też zera wiodące w numerach liczników albo trzeba je dodać w arkuszu, albo usunąć z numerów liczników w systemie.