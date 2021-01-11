---
title: Import operacji bankowych
---

# Import operacji bankowych

Za pomocą opisywanej funkcji można do systemu zaimportować wszystkie pozycje występujące na rachunku bankowym. Co więcej, w przeciwieństwie do importu płatności masowych, nie trzeba podpisywać z bankiem dodatkowej umowy oraz ponosić dodatkowych kosztów. Właściciele nie posiadają indywidualnych nr rachunków, przelewy kierują bezpośrednio na konto główne wspólnoty. Pozycje są identyfikowane następująco:

- Wpłaty — na podstawie numeru rachunku wpłacającego (z którego przychodzi przelew).
- Zapłaty — na podstawie numeru rachunku wyjściowego (na który jest kierowany przelew).
- Pozostałe uznania rachunku bankowego, np. odsetki od lokat, są księgowane automatycznie na wskazane konto.
- Pozostałe obciążenia rachunku bankowego, np. prowizje i opłaty, są księgowane automatycznie na wskazane konto.

#### Uruchomienie

Przed przystąpieniem do importu trzeba dla każdego budynku i rachunku bankowego, określić kilka ważnych ustawień. Aby to zrobić, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Importuj wyciąg elektroniczny`.
- Zakładka `Rachunki bankowe`.
- Pole `Zasób` > wybieramy budynek
- Pole `Konto` > wybieramy konto księgowe rachunku bankowego.
- Pole `Opis` > opis konta.
- Pole `Pozycje nierozpoznane Ma (Odsetki)` > ustalamy konto księgowe dla pozycji nierozpoznanych, uznań, zazwyczaj jest to konto `7xx-.. Przychody finansowe` lub `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Pozycje nierozpoznane Wn (Prowizje)` > ustalamy konto księgowe dla pozycji nierozpoznanych, obciążeń, zazwyczaj jest to konto `4xx/7xx-.. Koszty finansowe` lub `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Bank` > wskazujemy odpowiedni bank.
- Pole `Numer` > wpisujemy numer konta.
- Kliknąć: `Dodaj`.
- Podobnie uzupełniamy dla innych budynków lub rachunków.
- Pole `Hasło` > wpisać hasło.
- Kliknąć: `Zatwierdź`.

Powyższe ustawienia można dowolnie zmieniać w późniejszym czasie. Jeśli Państwa banku nie ma na liście, to prosimy się zgłosić do działu wsparcia Weles3.

![Uruchomienie importu](impoperacjiuruch.gif)

#### Pobranie pliku z banku

Z banku należy pobrać plik z listą operacji bankowych. Dane w pliku wyciągu powinny być w jednym z formatów:

- `Elixir`
- `MT940`
- `xml`

Pliki te zazwyczaj mają rozszerzenia: `*.ELX *.RES *.xml *.txt *.sta *.csv *.mt940`, należy tutaj zaznaczyć, że rozszerzenie nie decyduje czy plik się zaimportuje, do importu potrzeby jest właściwy format danych zawartych wewnątrz pliku. Plik musi być plikiem tekstowym, czyli zawierającym dane w postaci alfanumerycznej, więc importu nie przejdą formaty PDF, DOC, XLS.

Nie opiszemy tutaj pobierania pliku ze strony banku, każdy z nich ma swój sposób na generowanie raportu oraz różne formaty plików do wyboru, dodatkowo te rzeczy mogą się zmieniać w czasie. Jako pomoc w wyborze odpowiedniego formatu wyciągu podajemy przykłady nazw plików, które do tej pory są importowane do systemu:

- PKO BP:
    - `MT940_xx1440138700000000xxxxxxxx_20201209.txt`
    - `ACCOUNTS-HISTORY-STANDARD_xxxxxxx_20201228_xxxxxx_xxxxxxxx.xml`
    - `history_20201207_xxxxxx.xml`
    - `ELIXIR_xx102010550000xxxxxxxxxxxx_20201231.txt`
    - `xxxxxxxx.RES`
- Pekao:
    - `export20201201xxxxxx.mt940`
    - `export20210103xxxxxx.sta`
- Millennium:
    - `Historia_transakcji_20201210_xxxxxx.sta`
- ING:
    - `Wyciag_dla_Otwarte_Konto_Oszczęd._Firma__30.11.2020.sta`
    - `Wyciag_dla_Konto_Direct_dla_Firmy_w_PLN__30.11.2020.sta`
    - `Wyciag_dla_Konto Direct dla wspóln mieszk__31.10.2020.sta`
    - `Wyciag_dla_KONTO Z LWEM ZYSK w PLN__31.10.2020.sta`
    - `Lista_transakcji_nr_xxxxxxxxxx_xxxxxx.csv`
- BNP Paribas:
    - `export20201201xxxxxxxxxx.mt940`
- Pocztowy:
    - `11M_2020.mt940`
    - `xx13201120xxxxxxxxx0000001_1_MT940`
- Alior:
    - `export20201202xxxxxx.STA`
- mBank:
    - `xxxxxxx.dat`
- BZWBK:
    - `wyciag_xxxx_20201201.mt940x`
- GetIn:
    - `wyciagi_zbiorcze_2021-01-05_10-13-25.xml`
- BOŚ:
    - `_BOS_operacje_201201_xxxxxx.txt`
- Deutsche Bank:
    - `eWyciag_20210104_xxxxxx.csv`

Zazwyczaj ustalenie właściwego typu pliku należy przeprowadzić metodą prób i błędów. Najlepiej ze strony banku pobrać kilka różnych plików. Następnie skorzystać z funkcji do sprawdzania formatu w:

- Zakładka `Zasoby` > menu `Funkcje` > `Importuj wyciąg elektroniczny`.
- Zakładka `Sprawdzenie formatu`.

Należy tutaj wczytać plik i jeśli otworzy się tabelka z operacjami wyciągu, to oznacza, że format danych jest prawidłowy. Jest to opisane w dedykowanej [**instrukcji**](https://doc.weles3.pl/ksiegowe/importwyciagow/Sprawdzanie-formatu-pliku-WB.html).

Z importu operacji bankowych można korzystać nawet wtedy, gdy wspólnota posiada płatności masowe. Należy tutaj stosować pewną zasadę, z banku należy pobrać dwa pliki:

- Pierwszy z nich musi zawierać operacje tylko z wpłatami właścicieli na rachunki wirtualne, importujemy go w: `Importuj płatności masowe`.
- Drugi musi zawierać wszystkie pozostałe operacje z wyłączeniem wpłat masowych, importujemy go w: `Importuj wyciąg elektroniczny`.

Dla przykładu z banku PKO BP można pobrać paczkę przelewów składającą się z 3 plików:

- `*.ELX` > zawiera wszystkie operacje — pomijamy go.
- `*.SWR` > zawiera wyłącznie operacje skierowane na SWRK.
- `*.RES` > zawiera operacje z wyłączeniem tych, skierowanych na SWRK.

Pliki `SWR` i `RES` importujemy zgodnie z wcześniejszym opisem.

Do programu można importować paczkę wyciągów bankowych spakowanych w archiwum ZIP.

Jeśli napotykają Państwo problem z wyborem pliku pomimo zastosowania powyższych sposobów, to prosimy o kontakt z działem wsparcia Weles3.

#### Import pliku wyciągu

Aby zaimportować plik, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Importuj wyciąg elektroniczny`.
- Zakładka `Dodawanie`.
- Pole `Plik` > klikamy `Przeglądaj`.
- W oknie dialogowym wyszukujemy plik.
- Klikamy: `Otwórz`.
- Pole `Hasło` > wpisujemy hasło.
- Klikamy: `Zatwierdź`.

Po kliknięciu `Zatwierdź` okno może się zamknąć i wpłaty zostaną zaksięgowane w systemie. W tym momencie może też pojawić się błąd:

```
ERR
Brak konta FK dla rachunku 'WWEEEEOOOOPPPPLLLLNNNNYYYY'
Brak konta FK dla rachunku 'AABBBBCCCCDDDDEEEEFFFFGGGG'
Brak konta FK dla rachunku 'AAQQQQWWWWRRRRSSSSDDDDFFFF'
```

Oznacza to, że wpłata/zapłata z/na konto AA BBBB CCCC DDDD EEEE FFFF GGGG nie ma przypisanego konta księgowego, gdzie mogłaby się zaksięgować. Takie sparowanie trzeba teraz utworzyć, w tym celu, należy:

- Zamknąć okno błędu.
- Zakładka `Edycja`.
- Pole `Rachunek zasobu` > wybrać budynek i rachunek, dla którego był importowany plik.

W dolnej części okna pokaże się tabelka, w której przypisujemy `Rachunek obcy` do `Konta FK`. Należy odszukać pozycje, dla których `Konto FK` **nie jest określone**. Następnie:

- Z prawej strony pozycji klikamy na ikonkę lupy, pozycja załaduje się do górnej części okna.
- Pole `Rachunek obcy` > pomijamy.
- Pole `Nadawca` > będzie uzupełnione danymi nadawcy/odbiorcy przelewu.
- Pole `Treść` > będzie uzupełnione tytułem przelewu.
- Pole `Konto FK` > na podstawie wcześniejszych pól ustawiamy konto księgowe właściciela lub kontrahenta, ew. inne dowolne np. `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Konto FK zapłat` > podajemy tutaj konto do zapłat, jeżeli mają być one księgowane na innym koncie niż w polu `Konto FK`, można w ten sposób rozdzielić wpłaty i zapłaty.
- Kliknąć: `Dodaj`.

Powyższe czynności powtarzamy dla każdego rachunku obcego, który nie ma przypisanego konta księgowego. Gdy pozycje będą uzupełnione, należy:

- Pole `Hasło` > wpisać hasło.
- Kliknąć: `Zatwierdź`.

Okno funkcji zamknie się, należy jednak powrócić do niej i ponownie spróbować dodać plik do systemu, zaczynając jeszcze raz od początku instrukcji.

Zaimportowane wyciągi można dowolnie edytować i usuwać tak jak zwyczajny dekret. Można też je importować jeszcze raz, dodając do nazwy pliku frazę `_WYMUS_`.

![Import wyciągu](importwbzwyklego.gif)

#### Edycja konta księgowego

Czasami zachodzi konieczność zmiany miejsca księgowania się operacji bankowych dla danego rachunku obcego. W systemie można to bez problemu zrealizować, aby to zrobić, należy:

- Zakładka `Zasoby` > menu `Funkcje` > `Importuj wyciąg elektroniczny`.
- Zakładka `Edycja`.
- Pole `Rachunek zasobu` > wybrać budynek i rachunek.
- Z prawej strony pozycji klikamy na ikonkę lupy, pozycja załaduje się do górnej części okna.
- Pole `Rachunek obcy` > pomijamy.
- Pole `Nadawca` > będzie uzupełnione danymi nadawcy/odbiorcy przelewu.
- Pole `Treść` > będzie uzupełnione tytułem przelewu.
- Pole `Konto FK` > na podstawie wcześniejszych pól ustawiamy konto księgowe właściciela lub kontrahenta, ew. inne dowolne np. `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Konto FK zapłat` > podajemy tutaj konto do zapłat, jeżeli mają być one księgowane na innym koncie niż w polu `Konto FK`, można w ten sposób rozdzielić wpłaty i zapłaty.
- Kliknąć: `Dodaj`.
- Pole `Hasło` > wpisać hasło.
- Kliknąć: `Zatwierdź`.

![Edycja konta](importwbedycjakonta.gif)