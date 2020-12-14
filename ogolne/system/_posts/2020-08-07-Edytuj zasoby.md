---
title: Edytuj zasoby
---

# Edytuj zasoby

Za pomocą powyższego narzędzia możemy utworzyć nową wspólnotę w systemie oraz edytować dane i opcje już istniejących nieruchomości. 

#### Edycja danych wspólnoty

Aby edytować dane lub opcje istniejącej wspólnoty, należy przejść do:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj zasoby`.
- Wybrać nieruchomości z listy po lewej stronie okna.
- Kliknąć: `Edycja`.
- Pole `Wspólnota` > jeśli trzeba, wpisać nową nazwę wspólnoty.
- Pole `Adres` > jeśli trzeba, wpisać nowy adres wspólnoty, na przykład można dodać pod adresem dane administratora.
- Pole `Miejscowość` >jeśli trzeba, wpisać nową nazwę miejscowości.
- Pole `NIP` > wpisać NIP wspólnoty.
- Pole `Informacja` > wpisać dodatkowe informacje, jeśli występują.
- Pole `Data` > pozostawić bez zmian — jeśli zajdzie potrzeba zmiany, należy zgłosić się do działu wsparcia technicznego Weles 3.
- Pole `Opcje` > zaznaczamy żądane preferencje.
    - `Księgowanie należności jedną pozycją` > zaznaczenie tej opcji powoduje, że opłaty za lokal na koncie rozrachunkowym właściciela są księgowane jedną pozycją. Odznaczenie tej pozycji spowoduje, że należności będą zaksięgowane w podziale na grupy należności.
    - `Blokada dostępu właścicieli do e-kartoteki` > blokada odstępu do podglądu internetowego właścicielom.
    - `Blokada funkcji forum` > blokada forum.
    - `Numer WB w dowodzie pozycji` > przy wprowadzaniu wyciągów bankowych przez `Dodaj wyciąg bankowy`, domyślnie w polu `Dowód` uzupełniane jest ten sam tekst do w polu `Treść`. Włączenie tej opcji spowoduje, że w polu `Dowód` będzie wpisywany numer dekretu np. `36-2020/WB 14`.
    - `Oznaczenie dokumentów niekorygujących` > opcja dotyczy korekt. Jeśli korekta nic nie koryguje, to zostanie zaksięgowana jako zwyczajna zaliczka lub opłata.
    - `Rozszerzona analityka odsetek` > opcja określa sposób księgowania odsetek po stronie przychodów `7xx`. Domyślnie odsetki księgują `7xx-y`, gdzie `y` oznacza podkonto rozrachunkowe właściciela. Zaznaczenie tej opcji spowoduje, że do tego podziału dojdzie dodatkowy, podział na typy właścicieli. Struktura konta będzie wyglądała następująco: `7xx-z-y`, gdzie `z` to ID typu właściciela. W takim przypadku konto `7xx` musi mieć ustawioną analitykę 11.
- Kliknąć `Zapisz`.

![Edycja danych lub opcji](edytujzasoby3.gif)

#### Dodanie nowej wspólnoty

Aby dodać nową nieruchomość, należy przejść do:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj zasoby`.
- Kliknąć: `Nowy`.
- Pole `Wspólnota` > wpisać nazwę nowej wspólnoty.
- Pole `Adres` > wpisać nazwę i adres nowej nieruchomości.
- Pole `Miejscowość` > wpisać nazwę miejscowości, w której znajduje się Wspólnota.
- Pole `NIP` > wpisać NIP wspólnoty.
- Pole `Informacja` > wpisać dodatkowe informacje, jeśli występują.
- Pole `Data` > wpisać datę założenia wspólnoty **w systemie**. Bardzo ważna data, więcej szczegółów poniżej.
- Pole `Opcje` > zaznaczamy żądane preferencje.
- Klikamy: `Utwórz`. 

Po utworzeniu wspólnoty trzeba jeszcze wyrazić zgody na przetwarzanie danych osobowych w menu `Funkcje` > `Ochrona danych osobowych`. Po udzieleniu zgód można przesłać do działu wsparcia dane do założenia nieruchomości lub kontynuować zakładanie samodzielnie.

Odnośnie do daty założenia nieruchomości, jeśli Bilans otwarcia (lub przejęcia) nowego budynku jest np. na RRRR-**04-01**, ale najbliższe rozliczenie w systemie ma być wykonane za cały rok, to datę założenia wspólnoty ustawiamy koniecznie na początek roku tj. RRRR-**01-01**.

- Czyli nieruchomość zakładamy **od początku okresu** rozliczeniowego.

Stan właścicieli oraz zaliczki lub opłaty należy odtworzyć w systemie od początku tego okresu w części administracyjnej, aby system miał informacje o ich wysokości. Następnie trzeba sprawdzić ich poprawność i zaksięgować. Po tym prosimy zgłosić się do działu wsparcia, wyzerujemy je w części księgowej tak, aby nie tworzyły obrotów przed bilansem otwarcia (lub przejęcia).

Zalecamy niepomijanie procedury odtwarzania naliczeń na początku, przy zakładaniu budynku w systemie.

![Dodanie nowej wspólnoty](edytujzasoby2.gif)