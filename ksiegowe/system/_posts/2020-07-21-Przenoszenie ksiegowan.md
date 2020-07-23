---
title: Przenoszenie księgowań
---
# Przenoszenie księgowań

Funkcja służy do przenoszenia księgowań pomiędzy kontami. Nie jest tworzony nowy dokument, nie pojawiają się też dodatkowe storna, w pozycjach są poprawiane tylko i wyłącznie konta wybrane w polach Konto Wn i Ma. Funkcja ta przenosi wszystkie wybrane pozycje i umieszcza je na koncie docelowym. Jeśli na docelowym koncie są już jakieś księgowania, to obroty tego konta zostaną powiększone o wartość przenoszonych pozycji. Trzeba koniecznie sprawdzić, czy takie przeksięgowanie jest poprawne merytorycznie (np. czy nie połączymy wyciągów bankowych z przychodami na jednym koncie). Późniejsza poprawa lub cofnięcie tego działania może okazać się poważnie utrudniona, lub wręcz niemożliwa do przeprowadzenia i wszystkie dokumenty, w których dokonano zmiany, trzeba będzie poprawić ręcznie! Za pomocą tej funkcji nie przenosimy przychodów z kont 700, które zaksięgował system. Przenosi się je za pomocą korekt naliczeń lub przez ich cofnięcie i zmianę algorytmów.

### Przeksięgowania

- Wybieramy wspólnotę i przechodzimy do zakładki Konta FK.

![Przenoszenie księgowań](przenoszksieg1.png)

- Wybieramy menu Funkcje i Przeksięgowania. Po chwili otworzy się nowe okno dialogowe.

![Przenoszenie księgowań](przenoszksieg2.png)

- W tym momencie określamy Filtry dla naszego wyszukiwania: Pole Z konta — Wybieramy konto źródłowe.

![Przenoszenie księgowań](przenoszksieg3.png)

- Pole Okres od — Określamy datę początkową, domyślnie podpowiada bilans otwarcia, można to zmienić (naciskając Spację) na konkretną datę.

![Przenoszenie księgowań](przenoszksieg4.png)

- Pole Okres do — Określamy datę końcową.

![Przenoszenie księgowań](przenoszksieg5.png)

- Pole Strona — W tym polu wybieramy czy przeksięgowanie ma wyświetlić obroty z obydwu stron konta lub tylko z jednej, konkretnej Wn lub Ma.

![Przenoszenie księgowań](przenoszksieg6.png)

- Pole Typy dekretów — Pozwala na przeksięgowanie tylko wybranych typów dokumentów. Domyślnie wyświetlane i poprawiane jest wszystko, jeśli zostanie zaznaczony jeden lub więcej typów, to zostaną wyświetlone i poprawione tylko one.

![Przenoszenie księgowań](przenoszksieg7.png)

- Pole Na konto — opcjonalnie określamy konto docelowe (TYLKO CIĄG CYFR BEZ MYŚLNIKÓW) - możemy wpisać numer konta, na który system przeksięguje obroty. 

![Przenoszenie księgowań](przenoszksieg8.png)

- Po kliknięciu przycisku Wyszukaj, pozycje załadują się do dolnej części okna (do edycji).

![Przenoszenie księgowań](przenoszksieg9.png)

- Pole Pozycja — uaktywnia się po załadowaniu pozycji w dolnej części okna, pozwala wybrać konkretną pozycję.

![Przenoszenie księgowań](przenoszksieg10.png)

- Pole Konto docelowe — Pozwala na zmianę konta docelowego wybranej wcześniej pozycji.

![Przenoszenie księgowań](przenoszksieg11.png)

- Po kliknięciu klawisza Dodaj system ustawi konto docelowe w pozycji do przeksięgowania. Możemy teraz uzupełnić pozostałe pozycje (jedno przeksięgowanie może się odbywać na różne konta dla różnych pozycji).

![Przenoszenie księgowań](przenoszksieg12.png)

- Całość zatwierdzamy Hasłem.

![Przenoszenie księgowań](przenoszksieg13.png)

- W podglądzie dokumentu widać naszą przeksięgowaną pozycję.

![Przenoszenie księgowań](przenoszksieg14.png)

### Funkcje specjalne

W polu Na konto można wpisać formułę, która pozwoli na uzupełnienie konta docelowego automatycznie, czyli bez konieczności ręcznej edycji każdej z pozycji. W pole możemy wpisać konkretny numer konta albo formułę, która będzie takie konto podstawiała. Poniżej kilka przykładów dla lepszego zobrazowania.

- Pole Na konto jest puste — system nie przypisze konta docelowego, dla każdej widocznej pozycji trzeba takie konto wprowadzić osobno.

![Przenoszenie księgowań](przenoszksieg15.png)

- W pole Na konto jest wprowadzony konkretny numer konta z planu kont — wszystkie pozycje będą miały domyślnie wpisany ten numer konta.

![Przenoszenie księgowań](przenoszksieg16.png)

- W pole Na konto wprowadzamy formułę zaawansowaną tj. {X;Y} oznaczające podciąg numeru oryginalnego konta od znaku X o długości Y np. przy koncie 400123 specyfikacja 401{3;3} da nam 401123.

- Poniżej przykłady przeksięgowania z konta 400-1-100 na 400-1-200 w różnych wariantach.

![Przenoszenie księgowań](przenoszksieg17.png)

![Przenoszenie księgowań](przenoszksieg18.png)

![Przenoszenie księgowań](przenoszksieg19.png)