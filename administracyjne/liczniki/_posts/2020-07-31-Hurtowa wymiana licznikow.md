---
title: Hurtowa wymiana liczników
---

# Hurtowa wymiana liczników

Wymiana liczników polega na zamknięciu starych i otwarciu nowych oraz ewentualnym przeniesieniu. Czynność tą można sprawnie wykonać, tworząc odpowiednie tabelki w arkuszu kalkulacyjnym. Wymianę więc zaczynamy od pobrania z systemu arkusza z danymi obecnych liczników. Aby to zrobić, należy przejść do:

- Zakładka `Administracja` > menu `Funkcje` > `Wydruki`.
- Zakładka `Zasób`.
- Dodajemy wydruk `Lista odczytywania liczników`.
- Pole `Typ` > `Lista importu`.
- Pole `Bez grup liczników` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Bez typów właścicieli` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Sortowanie` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Format` > `CSV (;) - Excel`.
- Klikamy: `Podgląd wydruku`.

Pobieramy plik i otwieramy go w arkuszu kalkulacyjnym, wybierając odpowiednie kodowanie znaków i separator. Przykładowy [>>ARKUSZ<<](listaodczytywanialicznikow.xls) kliknij, aby pobrać.

![Wymiana liczników](listalicznikow.gif)

![Lista liczników](wymlistalicznikow.png)

Pobrany arkusz formatujemy do postaci trzech oddzielnych tabelek, tak jak to jest pokazane na obrazku poniżej. Kolumny `MIE NR TYP OB_PROG` ułatwiają tworzenie tabelek do wymiany. Jeśli liczniki nie mają prognoz, to tabelkę do ich przenoszenia można pominąć. Przykładowy [>>ARKUSZ<<](tabelkidowymiany.xls) kliknij, aby pobrać.

![Przykładowe tabelki](tabelkiwymiany.png)

Opis tabelek:

- Tabelka zamykająca stare liczniki składa się z kolumn:
  - `MIE` > numer lokalu.
  - `NR` > numer starego licznika
  - `TYP` > typ licznika.
  - `DATA` > data wymiany licznika.
  - `WAR` > odczyt końcowy.
  - `FIN` > dodajemy ją jako ostatnią, odpowiada za zamknięcie licznika, w jej komórkach wpisujemy 1.

- Tabelka dodająca nowe liczniki:
  - `MIE` > numer lokalu.
  - `NR` > numer nowego licznika.
  - `TYP` > typ licznika.
  - `DATA` > data wymiany licznika **musi być taka sama** jak w tabelce zamykającej licznik.
  - `WAR` > odczyt początkowy.
  - `NEW` > dodajemy ją jako ostatnią, odpowiada za dodanie licznika, w jej komórkach wpisujemy 1.

- Tabelka przenosząca prognozy na nowe liczniki:
  - `MIE` > numer lokalu.
  - `NR` > numer nowego licznika.
  - `TYP` > typ licznika.
  - `DATA` > data bieżąca, nie data wymiany. Data bieżąca to **pierwszy dzień miesiąca, za który nie są jeszcze zaksięgowane naliczenia** w systemie, bardzo ważne.
  - `PROG` > wartość prognozy. W pierwszym arkuszu to kolumna `OB_PROG` zachowujemy ją. Jeśli licznik nie ma prognozy, to wpisujemy słowo `PUSTY`.

Tak przygotowaną tabelki zaznaczamy pojedynczo w arkuszu, wraz z tytułami kolumn. Kopiujemy. Wklejamy do:

- Menu `Funkcje` > `Import danych` > Pole `Dane`.
- Następnie wpisujemy hasło i zatwierdzamy. 

Okno zamknie się, po czym można sprawdzić zaimportowane wartości odczytów i liczników. Czasami potrzeba też odświeżyć system: menu `Funkcje` > `Odśwież`.

![Import wymiany liczników](importwymianylicznikow.gif)

### Uwagi:

- Datę wpisujemy w formacie RRRR-MM-DD.
- Numery liczników sugerujemy podawać bez zer wiodących.
- W kolumnie WAR musi być podany odczyt licznika, bez tego system nie przyjmie tabelki.
- Liczniki, które nie zostały wymienione, usuwamy z tabelek.
- Tabelki importujemy tylko raz. Pojedynczo.
- Importujemy w kolejności: zamykająca stare liczniki > dodająca nowe liczniki > przenosząca prognozy.
- Taką wymianę liczników prosimy najpierw przeprowadzić w bazie testowej.
- Przed przystąpieniem do wymiany jest konieczne ustalenie terminu rozliczenia liczników.