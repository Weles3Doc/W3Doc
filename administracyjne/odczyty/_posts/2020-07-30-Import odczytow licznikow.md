---
title: Import odczytów liczników
---

# Import odczytów liczników

Do systemu można wprowadzić odczyty hurtowo, za pomocą tabelki z odpowiednimi kolumnami. Tabelka do importu odczytów powinna zawierać pięć kolumn. Oczywiście, jeśli posiadamy już odczyty liczników w arkuszu, to tabelkę formatujemy do opisanej postaci. Przed importem odczytów trzeba określić termin rozliczeń liczników. Poniżej przykładowa tabelka, którą tworzymy w arkuszu kalkulacyjnym:

![Tabelka importu odczytów](tabelkaimpodc.png)

Tytuły kolumn są bardzo ważne, nazywamy je tak jak na przykładzie. Kolejność kolumn nie ma znaczenia. W kolumnach podajemy:

- `MIE` > numer lokalu z systemu, musi być taki sam.
- `TYP` > podajemy typ licznika tak jak w systemie.
- `NR` > wpisujemy numer licznika.
- `DATA` > podajemy datę w formacie RRRR-MM-DD.
- `WAR` > wpisujemy wartość odczytu na wskazaną datę.

Tak przygotowaną tabelkę zaznaczamy w arkuszu, wraz z tytułami kolumn. Kopiujemy i wklejamy do:

- Zakładka `Administracja`.
- Menu `Funkcje` > `Import danych` > Pole `Dane`.
- Klikamy: `Zatwierdź`.

Okno importu zamykamy, po czym można sprawdzić zaimportowane wartości odczytów. Czasami potrzeba też odświeżyć system: menu `Funkcje` > `Odśwież`. Można pominąć kolumnę `TYP` — wtedy kolumna `NR` powinna mieć unikalne wartości. Można pominąć kolumnę `NR` — wtedy w lokalu może być tylko jeden licznik danego typu. Kolejność kolumn jest dowolna. Do liczników można zaimportować odczyty z typem odczytu: Wcześniejsze rozliczenie, w takim wypadku do tabelki dodajemy kolumnę `FIN`, wartości komórek uzupełniamy na 2. Częstą przyczyną problemów z importem są znaki niepisane (np. spacja) występujące w nazwach kolumn. Częstą przyczyną problemów są też zera wiodące w numerach liczników albo trzeba je dodać w arkuszu, albo usunąć z numerów liczników w systemie.

![Import odczytów](importodczytow.gif)