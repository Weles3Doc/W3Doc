---
title: Przykład RK - alg. pełen koszt
---

# Przykład RK - alg. pełen koszt

W niniejszej instrukcji przedstawimy Państwu przykładowe rozliczenie składnika opłat, dla którego jako wartość do rozliczenia podamy kwotę poniesionego kosztu w rozliczanym okresie. Warto nadmienić, że rozliczenia pełnym kosztem nie stosujemy dla składników opłat powiązanych z licznikami. 

#### Opis przykładu

Założenia:

- Przeprowadzimy rozliczenie Centralnego ogrzewania - opłaty stałej.
- Okres rozliczenia to pół roku.

#### Wstęp

Przed przystąpieniem do rozliczenia sprawdzamy:

- Czy wartość Danej (powierzchni użytkowej) wg, której będziemy rozliczać składnik, jest stała i prawidłowa w okresie rozliczenia lub jeśli występują jej zmiany, to są one zamierzone? (menu `Widok` > `Struktura danych w lokalach`)
- Czy wartość zaliczki za centralne ogrzewanie jest prawidłowa we wszystkich miesiącach, sprawdzamy też konto 700 przychodów składnika w zakładce Konta FK. (menu `Widok` > `Struktura naliczeń w lokalach` i zakładka `Konta FK`)
- Czy na koncie 400 składnika są zaksięgowane wszystkie koszty? (zakładka `Konta FK`)

![Przykład RK1](przykladRK1.gif)

#### Terminy rozliczeń

Po sprawdzeniu określamy okres rozliczenia składnika, w naszym przypadku jest to od 01-2021 do 06-2021.

Menu `Elementy` > `Terminy rozliczeń kosztów`

![Przykład RK2](przykladRK2.gif)

#### Określanie sposobu rozliczenia

Przechodzimy do ustawienia sposobu rozliczenia kosztów. Dla przyjętych wcześniej założeń ustawiamy:
- Zakładka `Administracja` > `Naliczenia` > `K.bieżąca`
- Menu `Obciążenia` > `Rozliczenia kosztów`.
- Pole `Typ` > `Algorytm - pełen koszt`.
- Pole `Sposób` > `Łącznie`.
- Pole `Algorytm` > wybieramy `Daną`, na przykład: `Powierzchnia użytkowa`.
- Pole `Wartość` > wpisujemy lub wybieramy z podpowiedzi kwotę kosztu CO stałej.
- Klikamy `Dodaj`.
- Klikamy `Zatwierdź`.

Następnie przeliczamy rozliczenie w korekcie bieżącej i sprawdzamy.

Menu `Obciążenia` > `Nalicz korekty RL + RK`.

![Przykład RK3](przykladRK3.gif)

#### Sprawdzenie

Sprawdzamy rozliczenie kosztów jeszcze przed zaksięgowaniem. Właściciele nie widzą w swoim podglądzie internetowym niezaksięgowanych rozliczeń. Opis kolumn:

- `Było Wartość` > jest to kwota poprzednich obciążeń (zaliczek, korekt, rozliczeń). do których odnosi się bieżące rozliczenie.
- `Ma być Wartość` > jest to kwota kosztu przypadająca na lokal, wynika z iloczynu kolumn Ilość oraz Stawka.
- `Wartość` > to różnica pomiędzy kolumnami `Było` i `Ma być`.
- `Stawka` > to kwota kosztu do rozliczenia.
- `Ilość` > to udział (ułamek) wyliczony z ilorazu: pow. lokalu / pow. całkowita, przedstawiając to w uproszczeniu.

![Przykład RK4](przykladRK4.gif)

#### Księgowanie

Po sprawdzeniu rozliczenia kosztów można przystąpić do jego księgowania. Rozliczenia zazwyczaj księgujemy na koniec okresu rozliczeniowego, dzięki temu nie wchodzą w przychody przyszłych okresów. Zarówno przed i po zaksięgowaniu można zrobić wydruk kontrolny od strony księgowej. Znajdziemy go w:

- Menu `Funkcje` > `Wydruki` > zakładka `Zasób` > Wydruk: `Rozliczenie` (lub `Sprawozdanie finansowe`).

Saldo dla rozliczanego składnika powinno być jak najbardziej zbliżone do zera. Księgowanie odbywa się za pomocą:

- Menu `Funkcje` > `Księguj należności`.

![Przykład RK5](przykladRK5.gif)

#### Przykład w arkuszu

Na koniec przedstawimy Państwu omawiane rozliczenie w arkuszu kalkulacyjnym.

**[Przykład RK Tabela](PrzykladRKtabela.xlsx)**