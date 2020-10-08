---
title: Import danych z arkusza
---

# Import danych z arkusza

Do systemu można wprowadzić dane hurtowo, za pomocą tabelki z odpowiednimi kolumnami. Tabelka do importu danych powinna zawierać co najmniej trzy kolumny. Poniżej przykładowa tabelka, którą tworzymy w arkuszu kalkulacyjnym:

![Przykładowa tabelka](przykladimp1.png)

Gdzie w kolumnach podajemy:

- `MIE` > numer lokalu z systemu, musi być taki sam.
- `DATA` > podajemy datę w formacie RRRR-MM-DD.
- `Dxx` > literka D i zaraz po niej `ID` danej, którą importujemy, np. D1.
- `Dyy` > można importować wiele danych naraz. W kolejnych kolumnach dostawiamy kolejne dane do importu. 

Tak przygotowaną tabelkę zaznaczamy w arkuszu, wraz z tytułami kolumn. Kopiujemy. Wklejamy do:

- Menu `Funkcje` > `Import danych` > Pole `Dane`.

Następnie wpisujemy hasło i zatwierdzamy. Okno zamknie się, po czym można sprawdzić zaimportowane wartości danych. Czasami potrzeba też odświeżyć system: menu `Funkcje` > `Odśwież`.

![Import danych](importdanych.gif)

Powyższy import działa dla miesięcy, za które **nie są jeszcze zaksięgowane zaliczki**. Gdy trzeba zaimportować dane wstecz, to trzeba do importowanej tabelki dodać dodatkowe kolumny.

- `DWxx` > literki DW i zaraz po nich `ID` danej importowanej wstecz. W komórkach tej kolumny wpisujemy 1.
- `DWyy` > kolumnę DW dodajemy dla każdej danej importowanej wstecz.

Przykład tabelki i przykład importu:

![Przykładowa tabelka](przykladimp2.png)

---

![Import danych wstecz](importdanychwstecz.gif)

#### Uwagi:

- Przy imporcie udziałów prosimy w arkuszu używać funkcji zaokr, zaokrąglić wartość danej do maksymalnie sześciu miejsc po przecinku. W przeciwnym wypadku udział może się nie równać 1 lub 100 procent.
- W kolumnie Dxx wartość danej może pozostać nieuzupełniona (pusta komórka), wtedy nie zostanie ona zaimportowana lub zmieniona.
- `ID` danych są różne — można je sprawdzić w menu `Zasoby` > `Edytuj dane`.
