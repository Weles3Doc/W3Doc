---
title: Przykład RK - alg. różnica
---

# Przykład RK - alg. różnica

W niniejszej instrukcji przedstawimy Państwu przykładowe rozliczenie składnika opłat, dla którego jako wartość do rozliczenia podamy kwotę różnicy pomiędzy przychodami a kosztami poniesionymi w okresie rozliczeniowym. Warto nadmienić, że rozliczenia różnicy można zrobić dla wszystkich opłat, zazwyczaj wykonujemy je dla składników opłat powiązanych z licznikami, na przykład dla Zimnej wody i ścieków. 

#### Opis przykładu

Założenia:

- Przeprowadzimy rozliczenie różnicy (często zwanej uchybem) po zaksięgowaniu rozliczenia liczników lokalowych zimnej wody.
- W budynku są liczniki ZW i CW, część lokali jest ryczałtowa, rozliczenie uchybu proporcjonalnie do powierzchni użytkowej na wszystkich.
- Okres rozliczenia to cały rok.
- Dla uproszczenia przyjmujemy, że wartość zbieranych zaliczek przez właścicieli jest stała przez cały okres.
- Nie ma zmian właścicieli ani zmian powierzchni użytkowej.

#### Wstęp

Przed przystąpieniem do rozliczenia sprawdzamy:

- Czy wartość Danej (powierzchni użytkowej) wg, której będziemy rozliczać składnik, jest stała i prawidłowa w okresie rozliczenia?
- Czy wartość zaliczki za Zimną wodę i ścieki, czy jest prawidłowa we wszystkich miesiącach, sprawdzamy też konto 700 przychodów składnika w zakładce Konta FK.
- Czy na koncie 400 składnika są zaksięgowane wszystkie koszty?

![Przykład Rk alg.1](przykladRKalg1.gif)

#### Terminy rozliczeń

Po sprawdzeniu określamy okres rozliczenia składnika, w naszym przypadku jest to od 01-2012 do 12-2012. 

![Przykład Rk alg.2](przykladRKalg2.gif)

#### Określanie sposobu rozliczenia

Przechodzimy do ustawienia sposobu rozliczenia kosztów. Dla przyjętych wcześniej założeń ustawiamy:

- Pole `Typ` > `Algorytm - różnica` (lub `Obciążenia - różnica` - jeśli RK ma być proporcjonalne od wcześniejszych obciążeń).
- Pole `Sposób` > `Łącznie` (na wszystkie lokale bez rozróżnienia czy jest ryczałtowy, czy olicznikowany).
- Pole `Algorytm` > wybieramy `Daną`, na przykład: `Powierzchnia użytkowa`.
- Pole `Wartość` > wpisujemy lub wybieramy z podpowiedzi kwotę różnicy ZW.

Następnie przeliczamy rozliczenie w korekcie bieżącej i sprawdzamy.

Menu `Obciążenia` > `Nalicz korekty RL + RK`.

![Przykład Rk alg.3](przykladRKalg3.gif)

#### Sprawdzenie

Sprawdzamy rozliczenie kosztów jeszcze przed zaksięgowaniem. Właściciele nie widzą w swoim podglądzie internetowym niezaksięgowanych rozliczeń. Opis kolumn:

- `Było Wartość` > jest to kwota poprzednich obciążeń (zaliczek, korekt, rozliczeń), do których odnosi się bieżące rozliczenie.
- `Ma być Wartość` > jest to kwota kosztu przypadająca na lokal, jest sumą kolumn `Było Wartość` + `Wartość`.
- `Wartość` > to wynik rozliczenia jest iloczynem kolumn `Ilość` oraz `Stawka`.
- `Stawka` > to kwota różnicy do rozliczenia.
- `Ilość` > to udział (ułamek) wyliczony z ilorazu: pow. lokalu / pow. całkowita (przedstawiając to w uproszczeniu).

![Przykład Rk alg.4](przykladRKalg4.gif)

#### Księgowanie

Po sprawdzeniu rozliczenia kosztów można przystąpić do jego księgowania. Rozliczenia zazwyczaj księgujemy na koniec okresu rozliczeniowego, dzięki temu nie wchodzą w przychody przyszłych okresów. Zarówno przed i po zaksięgowaniu można zrobić wydruk kontrolny od strony księgowej. Znajdziemy go w:

- Menu `Funkcje` > `Wydruki` > zakładka `Zasób` > Wydruk: `Rozliczenie` (lub `Sprawozdanie finansowe`).

Saldo dla rozliczanego składnika powinno być jak najbardziej zbliżone do zera. Księgowanie odbywa się za pomocą:

- Menu `Funkcje` > `Księguj należności`.

![Przykład Rk alg.5](przykladRKalg5.gif)

#### Przykład w arkuszu

Na koniec przedstawimy Państwu omawiane rozliczenie w arkuszu kalkulacyjnym.

[Przykład RK alg.](PrzykladRKtabelaalg.xlsx)