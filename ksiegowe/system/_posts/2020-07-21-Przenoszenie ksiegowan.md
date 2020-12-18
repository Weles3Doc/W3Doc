---
title: Przenoszenie księgowań
---
# Przenoszenie księgowań

Funkcja służy do przenoszenia księgowań pomiędzy kontami. Nie jest tworzony nowy dokument, nie pojawiają się też dodatkowe storna, w pozycjach dekretów są poprawiane tylko i wyłącznie konta Wn i Ma. Funkcja ta przenosi wybrane pozycje i umieszcza je na koncie docelowym. Jeśli na docelowym koncie są już jakieś księgowania, to obroty tego konta zostaną powiększone o wartość przenoszonych pozycji. Trzeba koniecznie sprawdzić, czy takie przeksięgowanie jest poprawne merytorycznie (np. czy nie połączymy wyciągów bankowych z przychodami na jednym koncie). Późniejsza poprawa lub cofnięcie tego działania może okazać się poważnie utrudniona, lub wręcz niemożliwa do przeprowadzenia i wszystkie dokumenty, w których dokonano zmiany, trzeba będzie poprawić ręcznie! Za pomocą tej funkcji nie przenosimy przychodów z kont 700, które zaksięgował system. Przenosi się je za pomocą korekt naliczeń lub przez ich cofnięcie i zmianę algorytmów.

Aby skorzystać z funkcji, należy przejść do:

- Zakładka `Konta FK` > menu `Funkcje` > `Przeksięgowania`.
- Pole `Z konta` > ustawiamy **konto źródłowe**.
- Pole `Analityka 2 3 4 5` > w tych polach podajemy numer konta analitycznego pod kontem źródłowym. Można je pozostawić puste lub wpisać numer na jednym z poziomów.
- Pole `Okres od` > określamy datę początkową pozycji, które będą brane do przeniesienia. Naciśnięcie spacji spowoduje zmianę `BO` na datę.
- Pole `Okres do` > określamy datę końcową pozycji, które będą brane do przeniesienia.
- Pole `Strona` > można tutaj ograniczyć pozycje do przeniesienia tylko ze strony `Ma` lub `Wn` konta.
- Pole `Typ dekretów` > można tutaj ograniczyć pozycje do przeniesienia tylko do specyficznego typu dekretu. Brak wyboru oznacza wszystkie typy.
- Pole `Na konto` > wpisujemy numer konta docelowego (bez myślników) lub pozostawiamy puste, w takim wypadku konto docelowe będzie można określić ręcznie w następnych polach.
- Pole `Liczba pozycji` > określamy limit pozycji branych do przeniesienia. (max. 5000)
- Kliknąć: `Wyszukaj`.

W dolnej części okna powinno się pokazać zestawienie pozycji do przeniesienia, które spełniają wyżej określone kryteria. Najważniejsze są kolumny `Konto`, podane w niej jest konto źródłowe oraz kolumna `Konto docelowe`, w skazanej jest w niej konto, na które zostanie przeniesiona pozycja. Jeśli konto docelowe jest określone jako `-----` oznacza to, że pozycja nie zostanie przeniesiona. Można też ręcznie wskazać lub zmienić konto docelowe pozycji, w tym celu w polach:

- Pole `Pozycja` > wybrać pozycję księgową.
- Pole `Konto docelowe` > ustawić jej konto, na które ma zostać przeniesiona.
- Kliknąć: `Dodaj`.

Gdy ustawienia są w porządku, wystarczy wpisać hasło i kliknąć zatwierdź. Pozycje przeniosą się natychmiast, po zmianie można też odświeżyć system: menu `Funkcje` > `Odśwież`. Z funkcji prosimy korzystać ostrożnie, cofnięcie zmian jest bardzo problematyczne i żmudne.

Na poniższym przykładzie przenosimy źle zaksięgowane koszty. Opłaty pocztowe powinny znaleźć się na koncie dedykowanym `400-2-001-001 Opłaty pocztowe`, a nie w pozostałych opłatach `400-2-099 Pozostałe opłaty`.

![Przenoszenie księgowań](przenoszenieksiegowan.gif)

#### Funkcje specjalne

W polu `Na konto` można wpisać formułę, która pozwoli na uzupełnienie konta docelowego automatycznie, czyli bez konieczności ręcznej edycji każdej z pozycji.

Formuła ma postać:

`{X;Y}`

Pozwala ona na skopiowanie części cyfr z konta źródłowego do konta docelowego. Liczba `X` określa miejsce, od którego numer będzie kopiowany. Liczba `Y` określa ilość skopiowanych cyfr.

- Przykłady użycia:

    W polu `Konto źródłowe` mamy wybrane konto syntetyczne `SSS`, które ma analityki: SSS-aa-bb.

    W polu `Na konto` uzupełnione `ZZZ{3;4}`

    Konto docelowe w pozycjach podpowie się `ZZZaabb`.

    Czyi program do konta syntetycznego `ZZZ` zastosuje taki sam numer konta co z `SSS`.

    `{3;4}` oznacza: zacznij kopiowanie po 3 cyfrze numeru konta, skopiuj 4 kolejne cyfry.

- Przykład użycia:

    W polu `Konto źródłowe` mamy wybrane konto syntetyczne `201`, które ma analityki: 201-y-xxxxxxx-z.

    W polu `Na konto` uzupełnione `{0;11}1`.

    Konto docelowe w pozycjach podpowie się `201-y-xxxxxxx-1`.

    Czyi program skopiuje prawie cały numer konta, jako ostatnie dostawi `1` zamiast `z`.

    `{0;11}` oznacza: zacznij kopiowanie po 0 cyfrze konta, skopiuj 11 kolejnych cyfr.