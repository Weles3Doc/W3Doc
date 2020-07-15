# Rozliczenie wyniku finansowego

Właściciele po zakończeniu roku finansowego mogą podjąć uchwałę o rozliczeniu wyniku finansowego. Takie rozliczenie można łatwo wykonać w systemie. Pierwszym etapem jest dodanie konta syntetycznego: 820 Rozliczenie wyniku finansowego, w tym celu przechodzimy do:

- Zakładka Zasoby > Menu Plan kont > Konta syntetyczne.
- Pole Numer > 820.
- Pole Nazwa > Rozliczenie wyniku finansowego.
- Pole Analityka > 2.
- Pole Konto > Wynikowe.
- Pole Typ > Zwykłe.
- Klikamy: Dodaj.
- Wpisujemy hasło i zatwierdzamy.

Jeśli konto jest już dodane, to ta czynność możne zostać pominięta.

![Rozliczenie WF](rkwf1.gif)

Po dodaniu konta syntetycznego trzeba dodać konto analityczne, w tym celu przechodzimy do:

- Zakładka Zasoby > Menu Plan kont > Edytuj konta.
- Pole Konto nadrzędne > 820.
- Pole Numer > 1 lub kolejny wolny numer.
- Pole Nazwa > Rozliczenie wyniku finansowego.
- Pole Usuwanie > Pozostaw.
- Klikamy: Dodaj.
- Wpisujemy hasło i zatwierdzamy.

Jeśli konto jest już dodane, to ta czynność możne zostać pominięta.

![Rozliczenie WF](rkwf2.gif)

Gdy konta są gotowe, można dodać algorytm, którym rozliczymy wynik, przechodzimy do:

- Zakładka Zasoby > Menu Elementy > Nazwy algorytmów.
- Pole ID > wpisujemy numer algorytmu, będzie on pochodną numeru konta: 820xx. Gdzie xx to numer konta analitycznego, w tym przypadku 01. Czyli wpisujemy 82001.
- Pole Nazwa > wpisujemy nazwę opłaty, którą zobaczą właściciele na wydrukach.
- Pole Grupa należności > wybieramy grupę należności, z której pochodzi rozliczany wynik.
- Pole Konto przychodów > wpisujemy 820010000000. (Ważne!)
- Pole Konto kosztów > wpisujemy 820010000000. (Ważne!)
- Pole Stawka VAT > ustawiamy stawkę, ew. może pozostać ND.
- Pole PKWiU > uzupełniamy numer, ew. może pozostać puste.
- Klikamy: Dodaj.
- Wpisujemy hasło i zatwierdzamy.

Jeśli algorytm jest już dodany, to ta czynność możne zostać pominięta.

![Rozliczenie WF](rkwf3.gif)

Gdy powyższe punkty zostały już zrobione, można przejść do zasadniczego rozliczenia. W pierwszej kolejności trzeba przenieść wynik finansowy z 860 na konto 820. Sporządzamy odpowiednie przeksięgowanie w zakładce Dekrety.

![Rozliczenie WF](rkwf4.gif)

Rozliczenie wyniku ustawiamy jak normalne rozliczenie kosztów. 

W terminach rozliczeń kosztów należny wybrać dodany algorytm: Rozliczenie wyniku finansowego 82001.

Jest to dokładnie opisane w ogólnej instrukcji rozliczenia pełnym kosztem.

### Uwagi:

- Rozliczenie wyniku robimy po zamknięciu roku.
- Rozliczenie można zrobić za zamknięty rok i zaksięgować w przyszłym.