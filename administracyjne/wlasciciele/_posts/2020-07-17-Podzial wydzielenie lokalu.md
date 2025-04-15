---
title: Podział / Wydzielenie lokalu
---

# Podział / Wydzielenie lokalu

Niniejsza instrukcja opisuje sytuację, w której właściciel sprzedaje tylko część swojego mieszkania. Może też posłużyć do wprowadzenia sprzedaży lokalu gminy lub miasta, którego zasoby są prowadzone w systemie w jednym lokalu zbiorczym.

Uwagi:

- Instrukcja opisuje wydzielenie lokalu **od daty bieżącej** (w miesiącu gdzie nie są zaksięgowane naliczenia).
- Wydzielenie lokalu **od daty wstecznej** robimy podobnie jak w instrukcji: Wykup wstecz lokalu. Z tą różnicą, że na lokalu zbiorczym pomniejszamy dane, a nie zerujemy oraz nie usuwamy na koniec właściciela z lokalu.

Wydzielenie lokalu składa się z kilku zasadniczych etapów:

#### Dodanie nowego, wydzielonego lokalu

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj mieszkania`.
- Klikamy: `Nowy`.
- Pole `Nazwa` > wpisujemy numer wydzielonego lokalu. 
- Pole `Informacje` > wpisać ew informacje.
- Kliknąć: `Utwórz`.

Nowy lokal nie pokaże się od razu, trzeba do niego przydzielić odbiorcę.

![Podział lokalu](podziallokalu0.gif)

#### Dodanie właściciela wydzielonego lokalu

- Zakładki `Administracja` > menu `Zasoby` > `Edytuj właścicieli`.
- Pole `Lokal` > wybrać wydzielony lokal.
- Pole `Data` > podać datę.
- Pole `Operacja` > wybrać `Nowy właściciel`.
- Pole `Udziałowcy` > `Właściciel główny`.
- Pole `Struktura` > wybrać strukturę, pod którą ma się podłączyć lokal (**Ważne!!**).
- Pole `Dokument` > wybrać jeden z dokumentów:
  - `Zawiadomienie` > zwyczajny dokument z opłatami.
  - `Faktura VAT` > wybieramy tylko, gdy chcemy wystawić wszystkie pozycje opłat na FV.
  - `Rachunek` > wybieramy wtedy, gdy chcemy wystawić opłaty na Rachunku lub na Fakturze uproszczonej.
- Pole `Typ` > określamy typ kartoteki, wypieramy jedną z dostępnych, ew. pozostawiamy `Ogólne`.
- Pole `Nazwa` > wpisujemy Imię i nazwisko lub nazwę odbiorcy.
- Pole `Adres` > podajemy pełen adres.
- Pole `Weryfikacja adresu` > `Sprawdzaj strukturę`.
- Pole `Informacje` > podajemy ew. dodatkowe informacje.
- Klikamy: `Dodaj`.
- Klikamy: `Zatwierdź`.

Lokal powinien się pojawić w polu `Struktura`.

![Podział lokalu](podziallokalu1.gif)

#### Edycja danych

Następnym etapem jest edycja danych na lokalach. Przechodzimy do:

-  Menu `Zasoby` > `Edytuj dane`. 

Schemat działania jest następujący:

- Na pierwotnym lokalu, dane **pomniejszamy** od daty wydzielenia.
- Na nowym lokalu, dane **dodajemy** od daty wydzielenia.

Na przykładzie, na którym działamy, z lokalu LU01 wydzielamy lokal LU01B od 1 lipca. Lokal LU01 ma powierzchnię 137,40. Wydzielony lokal będzie miał powierzchnię 68,7, więc nową powierzchnią lokalu M01 będzie 68,7 (podział na pół). W oknie edycji danych dodajemy dwie pozycje z wartością nowej powierzchni od daty podziału, na oba lokale. Podobnie postępujemy z innymi danymi lokalu, jak na przykład: Udział, Powierzchnia komórki, Liczba osób. (jeśli są dodane i jest taka potrzeba).

![Podział lokalu](podziallokalu2.gif)

#### Edycja liczników

Następnie można przystąpić do przeniesienia liczników, oczywiście, jeśli są takie, które zmieniły lokalizację. Analogicznie do danych, składa się to z dwóch czynności:

- Na pierwotnym lokalu, **zamknięcie** przenoszonych liczników.
- Na nowym lokalu, **dodanie** nowych liczników.

Do zamknięcia liczników używamy narzędzia:

- Menu `Zasoby` > `Edytuj odczyty`.

W lokalu pierwotnym wybieramy liczniki, które będą przeniesione, dodajemy im odczyt na datę wydzielenia, z zaznaczoną opcją: `Odczyt Końcowy`.

![Podział lokalu](podziallokalu3.gif)

Do dodania liczników na nowym lokalu używamy:

- Menu `Zasoby` > `Edytuj liczniki`.

W polu `Licznik` wybieramy: `Nowy licznik`, pozostałe pola uzupełniamy danym liczników z lokalu pierwotnego.

![Podział lokalu](podziallokalu4.gif)

#### Sprawdzenie naliczeń

Po wykonaniu zmian sprawdzamy naliczenia dla obu lokali.

![Podział lokalu](podziallokalu5.gif)