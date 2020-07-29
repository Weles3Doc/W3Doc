---
title: Import danych z arkusza
---
# Import danych z arkusza

Do systemu można wprowadzić dane hurtowo, za pomocą tabelki z odpowiednimi kolumnami. Tabelka do importu danych powinna zawierać co najmniej trzy kolumny. Poniżej przykładowa tabelka, którą tworzymy w arkuszu kalkulacyjnym:

MIE | DATA | Dxx | Dyy |
--- | ---- | --- | --- |
M01 | 2021-06-01 | 35,23 | 2 |
M02 | 2021-06-01 | 43,12 | 1 |
M03 | 2021-06-01 | 76,14 | 4 |
M04 | 2021-06-01 | 61,89 | 3 |

---

Gdzie w kolumnach podajemy:

- `MIE` > numer lokalu z systemu, musi być taki sam.
- `DATA` > podajemy datę w formacie RRRR-MM-DD.
- `Dxx` > literka D i zaraz po niej `ID` danej, którą importujemy, np. D1.
- `Dyy` > można importować wiele danych naraz. W kolejnych kolumnach dostawiamy kolejne dane do importu. 

Tak przygotowaną tabelkę zaznaczamy w arkuszu, wraz z tytułami kolumn. Kopiujemy. Wklejamy do:

- Menu `Funkcje` > `Import danych` > Pole `Dane`.

Następnie pisujemy hasło i zatwierdzamy. Okno zamknie się, po czym można sprawdzić zaimportowane wartości danych. Czasami potrzeba też odświeżyć system: menu `Funkcje` > `Odśwież`.

![Import danych](importdanych.gif)

Powyższy import działa dla miesięcy, za które **nie są jeszcze zaksięgowane zaliczki**. Gdy trzeba zaimportować dane wstecz, to trzeba do importowanej tabelki dodać dodatkowe kolumny.

- `DWxx` > literki DW i zaraz po nich `ID` danej importowanej wstecz. W komórkach tej kolumny wpisujemy 1.
- `DWyy` > kolumnę DW dodajemy dla każdej danej importowanej wstecz.

Przykład tabelki i przykład importu:

MIE | DATA | Dxx | Dyy | DWxx | DWyy |
--- | ---- | --- | --- | ---- | ---- |
M01 | 2021-06-01 | 35,23 | 2 | 1 | 1 |
M02 | 2021-06-01 | 43,12 | 1 | 1 | 1 |
M03 | 2021-06-01 | 76,14 | 4 | 1 | 1 |
M04 | 2021-06-01 | 61,89 | 3 | 1 | 1 |

---

![Import danych wstecz](importdanychwstecz.gif)

### Uwagi:

- Przy imporcie udziałów prosimy w arkuszu używać funkcji zaokr, zaokrąglić wartość danej do maksymalnie sześciu miejsc po przecinku. W przeciwnym wypadku udział może się nie równać 1 lub 100 procent.
- W kolumnie Dxx wartość danej może pozostać nieuzupełniona (pusta komórka), wtedy nie zostanie ona zaimportowana lub zmieniona.
- `ID` danych są różne — można je sprawdzić w menu `Zasoby` > `Edytuj dane`.
