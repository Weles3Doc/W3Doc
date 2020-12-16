---
title: Łączenie podkont rozrachunkowych
---

# Łączenie podkont rozrachunkowych

W systemie można połączyć konta rozrachunkowe właścicieli. Zazwyczaj rozrachunki są prowadzone na dwóch podkontach:

- `201-y-xxxxxxx-2` Media i eksploatacja
- `201-y-xxxxxxx-3` Fundusz remontowy

Jest to klasyczny sposób prowadzenia rozrachunków z właścicielem. W obecnych czasach administratorzy coraz częściej przechodzą na prowadzenie rozrachunków na jednym podkoncie:

- `201-y-xxxxxxx-1` Rozrachunki

Takie prowadzenie ma swoje zalety. Zarządca dba o poprawność mniejszej ilości kont, nie trzeba dzielić wpłat lub robić przeksięgowań. Właściciel nie musi robić dwóch przelewów, widzi jedno przejrzyste saldo.

Przed przystąpieniem do wykonywania zmiany, mogą Państwo skonsultować się z działem wsparcia Weles 3, podpowiemy jak dokładnie wykonać połączenie podkont.

#### Ustawienie jednego podkonta 201

Aby ustawić jedno konto rozrachunkowe, należy przejść do:

- Zakładka `Administracja` > menu `Elementy` > `Konta należności`.
- Pole `Grupa należności` > ustawiamy grupę należności.
- Pole `Podkonto` > wybrać jedno wspólne konto rozrachunkowe np. Rozrachunki.
- Kliknąć `Dodaj`.
- Przypisujemy tak każdą grupę należności do jednego podkonta.
- Kliknąć: `Zatwierdź`.

Po wykonaniu tej zmiany, obciążenia (zaliczki, korekty, rozliczenia) księgowane przez system, będą się już księgowały na nowym podkoncie. Nie dzieje się to z konkretną datą w systemie, określa to faktyczny moment zmiany sposobu księgowania. Na przykład, przy przechodzeniu na jedno podkonto od sierpnia, połączenie wykonujemy po zaksięgowaniu zaliczek za lipiec, a najlepiej tuż przed zaksięgowaniem zaliczek za sierpień. Warto w tym momencie wspomnieć o tym, aby nie cofać naliczeń po tej zmianie. Obciążenia, które zostały zaksięgowane jeszcze w podziale na MiE oraz FR, po cofnięciu i ponownym zaksięgowaniu zostaną zaksięgowane na nowy sposób.

![Łączenie kont 201](lonczenie2011.gif)

#### Przeniesienie pozycji

Jeśli trzeba, to po stworzeniu jednego konta rozrachunkowego, można przenieść na nie wcześniejsze pozycje księgowe z dotychczasowych podkont właściciela.

- Zakładka `Konta FK` > menu `Funkcje` > `Przeksięgowania`.
- Pole `Z konta` > ustawiamy `201 Właściciele`.
- Pole `Analityka 4` > wpisujemy numer podkonta źródłowego: `2` lub `3`, zazwyczaj będzie to odpowiednio `MiE` lub `FR`. Numery te mogą być różne, trzeba je sprawdzać.
- Pole `Okres od` > określamy datę początkową przeniesienia. Naciśnięcie spacji spowoduje zmianę `BO` na datę.
- Pole `Okres do` > określamy datę końcową przeniesienia.
- Pole `Strona` > `Obie`.
- Pole `Typ dekretów` > nic nie zaznaczamy, przenosimy wszystko.
- Pole `Na konto` > wpisujemy formułkę {0;11}1 spowoduje to automatyczne uzupełnienie konta docelowego, nowym podkontem rozrachunkowym.
- Pole `Liczba pozycji` > uzupełniamy 5000.
- Kliknąć: `Wyszukaj`.

W dolnej części okna powinno się pokazać zestawienie pozycji do przeniesienia, które spełniają wyżej określone kryteria. Najważniejsze są kolumny `Konto`, podane w niej jest konto źródłowe oraz kolumna `Konto docelowe`, w skazanej jest w niej konto, na które zostanie przeniesiona pozycja. Jeśli konto docelowe jest określone jako `-----` oznacza to, że pozycja nie zostanie przeniesiona. Można też ręcznie wskazać lub zmienić konto docelowe pozycji, w tym celu w polach:

- Pole `Pozycja` > wybrać pozycję księgową.
- Pole `Konto docelowe` > ustawić jej konto, na które ma zostać przeniesiona.
- Kliknąć: `Dodaj`.

Gdy ustawienia są w porządku, wystarczy wpisać hasło i kliknąć zatwierdź. Pozycje przeniosą się natychmiast, po zmianie można też odświeżyć system: menu `Funkcje` > `Odśwież`. Z funkcji prosimy korzystać ostrożnie, cofnięcie zmian jest bardzo problematyczne i żmudne.

![Łączenie kont 201](lonczenie2012.gif)

#### Dodatkowe czynności

- Jeśli wspólnota ma uruchomione płatności masowe, to numery przypisane do starych podkont trzeba przenieść na nowe podkonto lub wygenerować nowe numery indywidualne. Prosimy skontaktować się z działem wsparcia.
- Jeśli we wspólnocie importują Państwo wyciągi bankowe przez: menu `Funkcje` > `Import wyciągów bankowych` to trzeba poprawić konta FK przypisane do rachunków w zakładce `Edycja`.