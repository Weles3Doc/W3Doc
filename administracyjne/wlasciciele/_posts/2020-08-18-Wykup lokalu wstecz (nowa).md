---
title: Wykup lokalu wstecz (w przygotowaniu)
---

# Wykup lokalu wstecz

# **Nowa instrukcja — w przygotowaniu.**

Procedura wykupu lokalu wstecz potrzebna jest w sytuacji, gdy przykładowo w połowie roku otrzymujemy informację o zmianie właściciela lokalu, która nastąpiła na jego początku (np. w lutym). Z reguły w tym momencie mamy już zaksięgowane zaliczki oraz porozsyłane dokumenty do właścicieli. W tym rozdziale została przedstawiona procedura, która ma za zadanie rozwiązać problem związany z zaistniałą sytuacją w możliwie najlepszy sposób. Umożliwia ona korektę niezgodności za okres, który nie został jeszcze rozliczony przez rozliczenie kosztów. Procedurę tą wykonujemy **tylko i wyłącznie, jeśli mamy zaksięgowane już dokumenty zaliczki/korekty w miesiącu, w którym nastąpiła zmiana właściciela**. Jeśli nie mamy jeszcze zaksięgowanych naliczeń za miesiąc, w którym nastąpiła zmiana właściciela, to robimy Zwykły wykup.

Wykup wstecz lokalu składa się z dwóch zasadniczych czynności:

- Doprowadzenie do zwrotu (korekty) naliczonych należności staremu właścicielowi.
- Dodanie nowego lokalu i właściciela od daty wykupu, naliczenie należności (korekty) za lokal.

Następnie te dwa etapy można podzielić na:

- 1.0 Były właściciel:
  - 1.1 Edycja numeru lokalu.
  - 1.2 Wyzerowanie danych w lokalu.
  - 1.3 Wyzerowanie prognoz licznikom.
  - 1.4 Dodanie odczytów końcowych licznikom w lokalu.
- 2.0 Nowy właściciel:
  - 2.1 Dodanie nowego lokalu.
  - 2.2 Dodanie nowego właściciela.
  - 2.3 Dodanie danych.
  - 2.4 Wprowadzenie liczników.
  - 2.5 Dodanie prognoz licznikom.
- 3.0 Należności/korekta:
  - 3.1 Naliczenie korekty.
  - 3.2 Sprawdzenie obciążeń.
  - 3.3 Zaksięgowanie.
- 4.0 Usunięcie starego właściciela z lokalu.

Powyższe etapy zostaną dokładnie opisane poniżej.

#### 1.1 Edycja numeru lokalu byłego właściciela

Proces zaczynamy od zmiany numeru lokalu starego właściciela. Dodajemy literę S, ponieważ w nieruchomości nie może być dwóch lokali o takim samym numerze. Aby to zrobić, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj mieszkania`.
- Na liście po lewej stronie okna zaznaczamy **lokal byłego właściciela**.
- Klikamy: `Edycja`.
- Pole `Nazwa` > do numeru lokalu dodajemy literę S, będzie oznaczała starego właściciela.
- Pole `Informacja` > podajemy dodatkowe informacje o lokalu, może też pozostać puste.
- Kliknąć: `Zapisz`.

![Wykup wstecz edycja numeru lokalu.](NwykupwsteczEdycjalok.gif)

#### 1.2 Wyzerowanie danych w lokalu byłego właściciela

Następnym krokiem jest wyzerowanie danych w lokalu, zerujemy je od daty przekazania własności (aktu notarialnego). Przed przystąpieniem do czynności, sprawdzamy jakie dane należy wyzerować, w tym celu klikamy na lokal i następnie przycisk `Dane`. Aby je wyzerować, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj dane`.
- Pole `Lokal` > wybrać **lokal byłego właściciela**.
- Pole `Dana` > wybrać żądaną daną.
- Pole `Data` > wprowadzić **datę wykupu lokalu**.
- Pole `Wartość` > wprowadzamy **wartość = 0**, zerujemy.
- Kliknąć: `Dodaj`.
- Czynności **powtarzamy** dla każdej danej, która jest dodana do lokalu.
- Kliknąć: `Zapisz`.

![Wykup wstecz zerowanie danych lokalu.](NwykupwsteczEdycjadanychstr.gif)

#### 1.3 Wyzerowanie prognoz na licznikach byłego właściciela

Następnym krokiem jest wyzerowanie prognoz w lokalu, zerujemy je od daty przekazania własności (aktu notarialnego). Przed przystąpieniem do czynności, sprawdzamy jakie prognozy należy wyzerować, w tym celu klikamy na lokal i następnie przycisk `Liczniki`. Prosimy zapamiętać wartości prognoz na poszczególnych licznikach. Jeśli licznik nie ma prognozy, to nie trzeba jej zerować. Aby wyzerować prognozy, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj prognozy`.
- Pole `Licznik` > wybieramy licznik **w lokalu byłego właściciela**.
- Pole `Data` > ustawiamy **datę wykupu lokalu**.
- Pole `Wartość` > wpisujemy **prognozę = 0**, zerujemy.
- Klikamy: `Dodaj`.
- Czynności **powtarzamy** dla każdego aktywnego licznika, który jest dodany do lokalu.
- Klikamy: `Zatwierdź`.

![Wykup wstecz zerowanie prognoz lokalu.](NwykupwsteczEdycjaprogstr.gif)

#### 1.4 Zakończenie liczników u byłego właściciela

Następnym krokiem jest zamknięcie liczników w lokalu, zakańczamy je z datą przekazania własności (aktu notarialnego). Wartość odczytu podajemy z protokołu przekazania lokalu. Aby zamknąć liczniki, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj odczyty`.
- Pole `Licznik` > wybieramy licznik **w lokalu byłego właściciela**.
- Pole `Data` > ustawiamy **datę wykupu lokalu**.
- Pole `Wartość` > wpisujemy wartość odczytu z protokołu przekazania.
- Pole `Typ odczytu` > zaznaczamy `Końcowy — demontaż licznika`, powinien się pokazać haczyk przy prawidłowo zaznaczonej pozycji.
- Klikamy: `Dodaj`.
- Czynności **powtarzamy** dla każdego licznika, który jest dodany do lokalu.
- Klikamy: `Zatwierdź`.

![Wykup wstecz zamknięcie liczników w lokalu.](NwykupwsteczZamkliczstr.gif)

#### 2.1 Dodanie nowego lokalu

Przed dodaniem nowego właściciela, należy stworzyć lokal, aby to zrobić trzeba przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj mieszkania`.
- Klikamy: `Nowy`.
- Pole `Nazwa` > wpisać **normalny** numer lokalu taki jak miał stary właściciel.
- Pole `Informacja` > podajemy dodatkowe informacje o lokalu, może też pozostać puste.
- Kliknąć: `Utwórz`.

![Wykup wstecz dodanie nowego lokalu.](NwykupwsteczNowylok.gif)

#### 2.2 Dodanie nowego właściciela

Następnym krokiem jest dodanie nowego właściciela, po tej operacji powinien pojawić się w polu struktury. Przed przystąpieniem do czynności sprawdzamy, jaki dokument ma się wystawiać oraz pod jaką strukturą zlokalizować nowego właściciela. Aby dodać właściciela, należy przejść do:

- Zakładki `Administracja` > menu `Zasoby` > `Edytuj właścicieli`.
- Pole `Lokal` > wybrać lokal, który został stworzony w punkcie 2.1.
- Pole `Data` > ustawiamy **datę wykupu lokalu**.
- Pole `Operacja` > wybrać `Nowy właściciel` (ew. `Istniejący właściciel`, gdy chcemy wykorzystać istniejącą kartotekę właściciela).
- Pole `Udziałowcy` > `Właściciel główny`.
- Pole `Struktura` > wybrać strukturę, pod którą ma się podłączyć lokal (**Ważne!!**).
- Pole `Dokument` > wybrać jeden z dokumentów (**Ważne!!**):
  - `Zawiadomienie` > zwyczajny dokument z opłatami.
  - `Faktura VAT` > wybieramy tylko, gdy chcemy wystawić wszystkie pozycje opłat na FV.
  - `Rachunek` > wybieramy wtedy, gdy chcemy wystawić opłaty na Rachunku lub na Fakturze uproszczonej.
- Pole `Typ` > określamy typ kartoteki, wypieramy jedną z dostępnych, ew. pozostawiamy `Ogólne`.
- Pole `Nazwa` > wpisujemy Imię i nazwisko lub nazwę odbiorcy.
- Pole `Adres` > podajemy pełen adres.
- Pole `Weryfikacja adresu` > `Nie sprawdzaj struktury`.
- Pole `Informacje` > podajemy ew. dodatkowe informacje.
- Klikamy: `Dodaj`.
- Klikamy: `Zatwierdź`.

![Wykup wstecz dodanie nowego właściciela.](NwykupwsteczNowywlas.gif)

#### 2.3 Dodanie danych

Następnym krokiem jest dodanie danych do nowego lokalu, uzupełniamy je od daty przekazania własności (aktu notarialnego). Przed przystąpieniem do czynności, sprawdzamy jakie dane należy przenieść, w tym celu klikamy na lokal i następnie przycisk `Dane`. Aby dodać dane, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj dane`.
- Pole `Lokal` > wybrać **lokal nowego właściciela**.
- Pole `Dana` > wybrać żądaną daną.
- Pole `Data` > wprowadzić **datę wykupu lokalu**.
- Pole `Wartość` > wprowadzamy wartość danej taka jak była w starym lokalu, zazwyczaj dane takie jak powierzchnie, udziały i ilości się nie zmieniają, wyjątkiem są ew. normy lub zmiana liczby osób.
- Kliknąć: `Dodaj`.
- Czynności **powtarzamy** dla każdej danej, która jest dodana do lokalu.
- Kliknąć: `Zapisz`.

![Wykup wstecz dodanie danych nowego właściciela.](NwykupwsteczNowywdanelok.gif)

#### 2.4 Dodanie liczników

Następnym krokiem jest dodanie liczników w nowym lokalu, tworzymy je z datą przekazania własności (aktu notarialnego), numery i typy podajemy takie jak były u starego właściciela. Wartość odczytu podajemy z protokołu przekazania lokalu. Aby dodać liczniki, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj liczniki`.
- Kliknąć: `Nowy`.
- Pole `Lokal` > wybrać **lokal nowego właściciela**.
- Pole `Grupa liczników` > wybrać grupę liczników.
- Pole `Typ licznika` > wybrać typ licznika.
- Pole `Numer` > wpisać numer, maksymalnie 12 znaków, bez zer przodujących.
- Pole `Data założenia` > wprowadzić **datę wykupu lokalu**.
- Pole `Data legalizacji` > ustawić datę przyszłej legalizacji.
- Pole `Odczyt` > wpisujemy wartość odczytu z protokołu przekazania.
- Pole `Prognoza` > wpisać prognozę, może pozostać pusta.
- Pole `Lokalizacja` > wpisać lokalizacje, może pozostać puste.
- Klikamy: `Utwórz`.
- Czynności **powtarzamy** dla każdego aktywnego licznika, który był w lokalu starego właściciela.

![Wykup wstecz dodanie liczników nowego właściciela.](NwykupwsteczNowydodlicz.gif)

#### 2.5 Dodanie prognoz

Następnym krokiem jest dodanie prognoz w lokalu nowego właściciela, dodajemy je od daty przekazania własności (aktu notarialnego). Przed przystąpieniem do czynności, sprawdzamy jakie prognozy należy dodać, w tym celu klikamy na lokal i następnie przycisk `Liczniki`. Aby je dodać, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj prognozy`.
- Pole `Licznik` > wybieramy licznik **w lokalu nowego właściciela**.
- Pole `Data` > ustawiamy **datę wykupu lokalu**.
- Pole `Wartość` > wpisujemy prognozę.
- Klikamy: `Dodaj`.
- Czynności **powtarzamy** dla każdego aktywnego licznika w lokalu, który powinien posiadać prognozę.
- Klikamy: `Zatwierdź`.

![Wykup wstecz dodanie prognoz nowego właściciela.](NwykupwsteczNowydodprog.gif)

#### 3.1 Naliczenia korekty

(OPIS)

(GIF)

#### 3.2 Sprawdzenie korekty

(OPIS)

(GIF)

#### 3.3 Księgowanie korekty

(OPIS)

(GIF)

#### 4.0 Usunięcie starego właściciela z lokalu

(OPIS)

(GIF)

## FIN