---
title: Rozliczenia ciepła
---

# Rozliczenia ciepła

Instrukcja w przygotowaniu

W związku z wejściem w życie [rozporządzenia Ministra Klimatu i Środowiska z dnia 7 grudnia 2021 roku](https://isap.sejm.gov.pl/isap.nsf/DocDetails.xsp?id=WDU20210002273) zaimplementowaliśmy w systemie możliwość przekazywania użytkownikom lokali dodatkowych informacji dotyczących kosztów zakupu ciepła w zakresie przewidzianym przedmiotowym rozporządzeniem.

### Ustawienia wstępne

Aby określić parametry pozwalające wyliczyć dodatkowe informacje w sprawie rozliczenia, należy przejść do:

- Zakładka `Administracja` > menu `Elementy` > `Rozliczenia ciepła`.
- Zakładka `Edycja`.
- Pole `Grupa liczników` > wybieramy grupę liczników zawierającą liczniki uczestniczące w rozliczeniu ciepła.
- Pole `Struktura` > w większości przypadków wybieramy cały zasób, jeśli chociaż jeden z parametrów ustalanych w dalszych polach jest inny dla danej grupy lokali, należy je rozdzielić, dodając dwie lub więcej pozycji.
- Pole `Od` > ustalamy datę obowiązywania wprowadzonej pozycji. Zazwyczaj będzie to pierwszy dzień okresu rozliczeniowego (na przykład 1 stycznia lub 1 lipca). Pozycję można dodać z datą przeszłą, dzięki temu zyskamy możliwość porównywania obecnych rozliczeń do dużo starszych okresów rozliczeniowych.
- Pole `Typ` > ustawiamy `Ciepłomierze` lub `Podzielniki` w zależności, jakie urządzenie jest zainstalowane w lokalach danej struktury.
- Pole `Koszt GJ` > wybieramy stawkę, w której jest zawarta cena jednostkowa ciepła.
- Pole `Współczynnik struktury` > dotyczy tylko podzielników, wybieramy daną, w której są zawarte współczynniki wyrównawcze.
- Pole `Powierzchnia` > ustawiamy daną, która reprezentuje powierzchnię, która zostanie wykorzystana do wyliczenia średniej ilości jednostek ciepła na jednostkę powierzchni na miesiąc.
- Pole `Minimum GJ/m2` > dotyczy tylko podzielników, minimalny koszt ciepła.
- Pole `Maksimum GJ/m2` > dotyczy tylko podzielników, maksymalny koszt ciepła.
- Pole `Temperatura` > można pozostawić puste lub uzupełnić wartość wynikającą z normy: [https://nowoczesnyzarzadca.pl/2022/09/19/rozliczenia-ciepla](https://nowoczesnyzarzadca.pl/2022/09/19/rozliczenia-ciepla.html)
- Kliknąć `Dodaj`.

Dodajemy więcej pozycji, jeśli chociaż jeden z parametrów ustalanych w polach jest inny dla danej grupy lokali. Pozycje zazwyczaj ustalamy tylko raz, jeśli żaden z parametrów się nie zmienia. Wprowadzone pozycje można dowolnie edytować.

### Sprawdzenie wyników

Po ustawieniu parametrów można od razu sprawdzić wynik działania opisywanej funkcji systemu. Aby zobaczyć dodatkowe informacje w sprawie rozliczenia ciepła, należy przejść do:

- Zakładka `Administracja` > menu `Elementy` > `Rozliczenia ciepła`.
- Zakładka `Rozliczenia ciepła`.
- Pole `Grupa liczników` > wybieramy grupę liczników, dla której zostały określone parametry i dla której chcemy zapoznać się z wynikami funkcji.
- Pole `Okres rozliczenia` > wybieramy porównywany okres rozliczenia.
- Pole `Nazwa algorytmu` > wybieramy algorytm, który jest skojarzony z rozliczeniami ciepła i dla którego chcemy zapoznać się z wynikami funkcji
- Pole `Struktura` > wybieramy strukturę, dla której zostały określone parametry i dla której chcemy zapoznać się z wynikami funkcji.

W środkowej części okna wyświetlą się lokale oraz wyliczone dla nich parametry. Po wybraniu lokalu z listy, w dolnej części okna wyświetli się porównanie parametrów z różnych okresów rozliczeniowych.

### Wydruk dodatkowych informacji

Ady na wydruku rozliczenia dodać tabelkę z dodatkowymi informacjami, należy użyć elementu `Rozliczenia ciepła`:

![Rozliczenia ciepła element](rozl_co_element.png)

Opis ustawień:

- Pole `Miesiąc` > wybieramy rozliczenie, w którym znajduje się rozliczenia liczników lub podzielników.
- Pole `Okres bazowy — przesunięcie` > ustawiany częstotliwość rozliczeń. 1 - rok; 2 - półroczne; 4 - kwartalne. Parametr odpowiada za porównywanie okresów rozliczeniowych.
- Pole `Okres bazowy — liczba` > ustawiamy ilość pokazywanych okresów rozliczeniowych w tabelce, które można porównać (2, 3, 4,).
- Pole `Zużycie właścicieli` > decydujemy, czy w przypadkach zmian właścicieli lokalu, w tabelce ma się wyświetlać zużycie poprzedniego właściciela. 
- Pole `Wykres` > decydujemy czy wykres ma się znaleźć w kolumnie z wartością średnich, czy obok w osobnej kolumnie.
- Pole `Tytuł` > wpisujemy tytuł tabelki.

### Przykłady tabelek:

- Liczniki

![Rozliczenia ciepła wydruk](rozl_co_wydruk1.png)

- Podzielniki

![Rozliczenia ciepła wydruk](rozl_co_wydruk2.png)

- Ryczałt

![Rozliczenia ciepła wydruk](rozl_co_wydruk3.png)
