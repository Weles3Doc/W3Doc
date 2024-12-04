---
title: Edycja mieszkań
---

# Edycja mieszkań

Mieszkania/lokale są elementami systemu, do których można przydzielić właściciela lub innego odbiorcę. To właśnie do nich przydzielamy dane i liczniki oraz definiujemy naliczenia. Do mieszkania/lokalu musi być dodany właściciel/odbiorca, aby wyświetlał się w systemie. Numerację lokali zazwyczaj tworzymy, zaczynając od literki określającej funkcje lokalu np. M — mieszkanie, G — garaż, P — pożytek, LU — lokal użytkowy. Po niej dodajemy numer, z tym że dodajemy też zera przodujące. Przykładowe numery to: 

- `M01 M02 M03` > gdy mieszkań jest mniej niż 99.
- `M001 M002 M003` > gdy mieszkań jest ponad sto.
- `G01 G02` > dla garaży.
- `LU01 LU02` > dla lokali użytkowych.
- `P01 P02 P03` > dla pożytków. 

Numery mieszkań są sortowane alfabetycznie. Jeśli do właściciela są przypisane dwa lub więcej lokali, to przy nazwisku na listach w systemie, wyświetli się jeden numer lokalu — pierwszy alfabetycznie. Numer lokalu w obrębie jednego zasobu musi być unikalny. Informacje podane w polu `Informacja` są dostępne w zakładce `Administracja` po zaznaczeniu lokalu lub w menu `Funkcje` > `Wydruki` > `Zasób` > `Inf. osób/mieszkań`.

#### Dodanie nowego mieszkania/lokalu

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj mieszkania`.
- Klikamy: `Nowy`.
- Pole `Nazwa` > wpisać numer mieszkania/lokalu/elementu.
- Pole `Informacja` > podajemy dodatkowe informacje o lokalu, może też pozostać puste.
- Kliknąć: `Utwórz`.

![Edycja mieszkań](edycjamienowa.gif)

#### Edycja nazwy mieszkania/lokalu

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj mieszkania`.
- Zaznaczamy lokal do edycji.
- Klikamy: `Edycja`.
- Pole `Nazwa` > można wpisać nowy unikalny numer/nazwę.
- Pole `Informacja` > podajemy dodatkowe informacje o lokalu, może też pozostać puste.
- Kliknąć: `Zapisz`.

![Edycja mieszkań](edycjamienazwy.gif)

#### Usunięcie mieszkania/lokalu

Aby usunąć lokal, trzeba najpierw usunąć z niego właściciela/odbiorcę. Dodatkowo warto też przed tym usunąć z niego: dane, liczniki, indywidualne stawki i algorytmy.

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj mieszkania`.
- Na liście po lewej stronie okna zaznaczamy lokal do usunięcia.
- Klikamy: `Usuń`.