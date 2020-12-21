---
title: Rozliczenie wyniku finansowego
---

# Rozliczenie wyniku finansowego

Właściciele po zakończeniu roku finansowego mogą podjąć uchwałę o rozliczeniu wyniku finansowego. Takie rozliczenie można łatwo wykonać w systemie. Składa się ono z kilku etapów, które przedstawiamy poniżej.

#### Dodanie konta 820

Jeśli konto jest już dodane, to ten punkt pomijamy.

Pierwszym etapem jest dodanie konta syntetycznego: 820 Rozliczenie wyniku finansowego, w tym celu przechodzimy do:

- Zakładka `Zasoby` > menu `Plan kont` > `Plan kont`.
- Kliknąć: `Dodaj konto syntetyczne`.
- Pole `Numer` > podać numer konta, zazwyczaj jest to 820 (sprawdzić, czy numer jest wolny).
- Pole `Nazwa` > podać nazwę konta.
- Pole `Analityka` > podać analitykę konta np. 2.
- Pole `Konto` > `Wynikowe`.
- Pole `Typ` > `Zwykłe`.
- Kliknąć: `Utwórz`.

![Rozliczenie WF](rkwf1.gif)

#### Dodanie konta analitycznego

Jeśli konto jest już dodane, to ten punkt pomijamy.

Po dodaniu konta syntetycznego trzeba dodać konto analityczne, w tym celu przechodzimy do:

- Zakładka `Zasoby` > menu `Plan kont` > `Plan kont`.
- Na liście po lewej stronie wybieramy konto nadrzędne **820**, pod którym chcemy dodać nowe konto.
- Kliknąć: `Dodaj podkonto`.
- Pole `Numer` > podać numer konta 1 (sprawdzić, czy numer jest wolny).
- Pole `Nazwa` > podać nazwę konta.
- Kliknąć: `Utwórz`.

![Rozliczenie WF](rkwf2.gif)

#### Dodanie algorytmu

Jeśli algorytm jest już dodany, to ta czynność możne zostać pominięta.

Gdy konta są gotowe, można dodać algorytm, którym rozliczymy wynik, przechodzimy do:

- Zakładka `Zasoby` > menu `Elementy` > `Nazwy algorytmów`.
- Kliknąć: `Nowy`.
- Pole `ID` > wpisujemy numer algorytmu, będzie on pochodną numeru konta: 820xx. Gdzie xx to numer konta analitycznego, w tym przypadku 01, czyli wpisujemy `82001`.
- Pole `Nazwa` > wpisujemy nazwę opłaty, którą zobaczą właściciele na wydrukach.
- Pole `Grupa należności` > wybieramy grupę należności, z której pochodzi rozliczany wynik.
- Pole `Konto przychodów` > wpisujemy `820-01`, czyli wcześniej utworzone konto. (Ważne!)
- Pole `Konto kosztów` > wpisujemy `820-01`, czyli wcześniej utworzone konto. (Ważne!)
- Pole `Stawka VAT` > można pozostawić `ND` lub wybrać inną wartość.
- Pole `PKWiU` > może pozostać puste.
- Klikamy: `Dodaj`.
- Klikamy: `Utwórz`.

![Rozliczenie WF](rkwf3.gif)

#### Przeniesienie wyniku

Gdy powyższe punkty zostały już zrobione, można przejść do zasadniczego rozliczenia. W pierwszej kolejności trzeba przenieść wynik finansowy z 860 na konto 820. Sporządzamy odpowiednie przeksięgowanie w zakładce Dekrety.

![Rozliczenie WF](rkwf4.gif)

#### Rozliczenie

Rozliczenie wyniku ustawiamy tak jak normalne rozliczenie kosztów. W menu `Elementy` > `Terminy rozliczeń kosztów` należny wybrać dodany algorytm: Rozliczenie wyniku finansowego 82001. Ustawić sposób rozliczeń w menu `Obciążenia` > `Rozliczenie kosztów`, jest to dokładnie opisane w ogólnej instrukcji: `Przykład RK - alg. pełen koszt`.