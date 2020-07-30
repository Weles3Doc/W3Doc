---
title: Import prognoz liczników
---
# Import prognoz liczników

Do systemu można wprowadzić prognozy hurtowo, za pomocą tabelki z odpowiednimi kolumnami. Często taka potrzeba zachodzi przy dodawaniu ręcznie wyliczonych prognoz lub ich powiększaniu np. o 10%. Tabelka do importu prognoz powinna zawierać pięć kolumn. Oczywiście, jeśli posiadamy już prognozy liczników w arkuszu, to tabelkę formatujemy do opisanej postaci. Poniżej przykładowa tabelka, którą tworzymy w arkuszu kalkulacyjnym:

![Tabelka importu prognoz](tabelkaimpprog.png)

Gdzie w kolumnach podajemy:

- `MIE` > numer lokalu z systemu musi być taki sam.
- `TYP` > podajemy typ licznika tak jak w systemie.
- `NR` > wpisujemy numer licznika.
- `DATA` > podajemy datę w formacie RRRR-MM-DD.
- `PROG` > wpisujemy wartość prognozy na wskazaną datę.

Tak przygotowaną tabelkę zaznaczamy w arkuszu, wraz z tytułami kolumn. Kopiujemy. Wklejamy do:

- Menu `Funkcje` > `Import danych` > Pole `Dane`.
- Wpisujemy hasło i zatwierdzamy. 

Okno zamknie się, po czym można sprawdzić zaimportowane wartości prognoz. Czasami potrzeba też odświeżyć system: menu `Funkcje` > `Odśwież`.

Takie zestawienie można też wygenerować z systemu, aby to zrobić, należy przejść do:

- Menu `Funkcje` > `Wydruki` > zakładka `Zasób`.
- Dodajemy wydruk > `Lista odczytywania liczników`.
- Pole `Typ` > `Lista importu`.
- Pole `Format` > `CSV Excel (;)`.
- Klikamy: `Podgląd wydruku`.

Dokument importujemy do arkusza kalkulacyjnego, wybierając odpowiednie kodowanie i separator.

![Import prognoz](importprognoz1.gif)

Takie zestawienie formatujemy do postaci tabelki, w której znajduje się pięć kolumn:

- `MIE` > wpisujemy numer lokalu (taki jak w systemie).
- `NR` > wpisujemy numer licznika.
- `TYP` > wpisujemy typ licznika.
- `PROG` > wpisujemy wartość prognozy.
- `DATA` > wpisujemy datę, od której ma obowiązywać nowa prognoza. W formacie: RRRR-MM-DD.

Formatowanie zestawienia otrzymanego z systemu przedstawiamy poniżej.

![Import prognoz](importprognoz2.gif)

Tak sformatowaną tabelkę kopiujemy (wraz z tytułami kolumn) i wklejamy w:

- Menu `Funkcje` > `Import danych` > `Pole dane`.
- Wpisujemy hasło i zatwierdzamy.

Okno powinno się zamknąć. Nowe prognozy powinny być od razu widoczne na licznikach. Czasami trzeba też odświeżyć system: menu `Funkcje` > `Odśwież`.

![Import prognoz](importprognoz3.gif)


### Uwagi:

- Jeśli wystąpi błąd podczas importu, proszę sprawdzić, czy pomiędzy arkuszem a systemem są zgodne numery lokali i liczników oraz ich typy.
- Można pominąć kolumnę TYP — wtedy kolumna NR powinna mieć unikalne wartości.
- Można pominąć kolumnę NR — wtedy w lokalu może być tylko jeden licznik danego typu.
- Kolejność kolumn jest dowolna.
- Prognozy mogą przyjmować wartości ujemne.
- Gdy wpiszemy w kolumnie PROG, jako wartość prognoz wyraz PUSTY, to prognoza zostanie usunięta z licznika — ustawiona na brak/pusta.
- Prognozy można importować z datami wstecznymi.
- W kolumnie OB_PROG jest wpisana obecna prognoza licznika.
- Częstą przyczyną problemów z importem są znaki niepisane (np. spacja) występujące w nazwach kolumn lub innych komórkach.
- Częstą przyczyną problemów są też zera wiodące w numerach liczników albo trzeba je dodać w arkuszu, albo usunąć z numerów liczników w systemie.