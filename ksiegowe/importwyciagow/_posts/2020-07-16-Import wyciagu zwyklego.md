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
- Pole `Bank` > wskazujemy odpowiedni bank. Jeśli Państwa banku nie ma na liście, to prosimy wybrać `-----`.
- Pole `Numer` > wpisujemy numer konta.
- Kliknąć: `Dodaj`.
- Podobnie uzupełniamy dla innych budynków lub rachunków.
- Kliknąć: `Zatwierdź`.

Powyższe ustawienia można dowolnie zmieniać w późniejszym czasie. 

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

Zazwyczaj ustalenie właściwego typu pliku należy przeprowadzić metodą prób i błędów. Najlepiej ze strony banku pobrać kilka różnych plików. Następnie wykonać import każdego z nich.

Z importu operacji bankowych można korzystać nawet wtedy, gdy wspólnota posiada płatności masowe. Należy tutaj stosować pewną zasadę, z banku należy pobrać dwa pliki:

- Pierwszy z nich musi zawierać operacje tylko z wpłatami właścicieli na rachunki wirtualne.
- Drugi musi zawierać wszystkie pozostałe operacje z wyłączeniem wpłat masowych.

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
- Zakładka `Import`.
- Pole `Wybierz lub przeciągnij i upuść plik` > wybieramy lub przeciągamy plik do importu, można też wczytać więcej wyciągów na raz, mogą być też spakowane archiwum ZIP.
- Klikamy: `Analizuj wyciągi zwykłe`.

![Import zwykły](imp_wb_zwyk_01.png)

Okno importu zmieni wygląd. Z lewej strony pokażą się importowane pliki. Na liście plików można kliknąć nazwę importowanego wyciągu, aby zapoznać się z importowanymi operacjami.

Jeśli kliki mają status `Prawidłowe pliki` to:

- Klikamy: `Importuj poprawne`.

Po kliknięciu okno się zamknie i operacje zostaną zaksięgowane w systemie. 

![Import zwykły](imp_wb_zwyk_02.png)

**W tym momencie może też pojawić się błąd**, jest to typowe dla tego rodzaju importu. Operacje dla których nie zostało jeszcze wskazane konto księgowe zostaną oznaczone jako `Brak konta FK dla rachunku`. Oznacza to, że wpłata/zapłata z/na konto AA BBBB CCCC DDDD EEEE FFFF GGGG nie ma przypisanego konta księgowego, gdzie mogłaby się zaksięgować. Takie sparowanie trzeba teraz utworzyć, w tym celu, należy:

- Kliknąć: `Powrót`.

![Import zwykły](imp_wb_zwyk_03.png)

Przechodzimy do:

- Zakładka `Przypisanie kont`.

![Import zwykły](imp_wb_zwyk_04.png)

W polu `Rachunek bankowy` wybrać rachunek dla którego importowane pozycje stwarzały problem.

![Import zwykły](imp_wb_zwyk_05.png)

W dolnej części okna pokaże się tabelka, w której przypisujemy `Rachunek podmiotu` do `Konta FK`. Należy odszukać pozycje, dla których `Konto FK` **nie jest określone**, takie pozycje są oznaczone jako `--- BRAK --- --- BRAK ---`. Następnie:

- Z **prawej** strony pozycji klikamy na ikonkę rysika ![Rysik](rysik.png), pozycja załaduje się do górnej części okna.
- Pole `Nazwa podmiotu` > będzie uzupełnione danymi nadawcy/odbiorcy.
- Pole `Treść` > będzie uzupełnione tytułem przelewu.
- Pole `Rachunek podmiotu` > pomijamy/nie zmieniamy.
- Pole `Konto FK` > na podstawie wcześniejszych pól ustawiamy konto księgowe właściciela lub kontrahenta, ew. inne dowolne np. `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Konto FK zapłat` > można pozostawić puste. Podajemy tutaj konto do zapłat, jeżeli mają być one księgowane na innym koncie niż wpłaty z pola `Konto FK`, można w ten sposób rozdzielić wpłaty i zapłaty.
- Kliknąć: `Dodaj`.

Powyższe czynności powtarzamy dla każdego rachunku podmiotu, który nie ma przypisanego konta księgowego. 

![Import zwykły](imp_wb_zwyk_06.png)

Gdy pozycje będą uzupełnione, należy:

- Kliknąć: `Zatwierdź`.

Należy powrócić do zakładki `Import` i ponownie spróbować dodać plik, postępując jeszcze raz od początku instrukcji.

Jeśli właściciele wypłacają czynsze poprzez pośredników np. Pocztę Polską, będą one oznaczone w tytule przelewu jako `Wpłata w UP....`, to takie pozycje należy przypisać do konta ksiegowego `249-01 Wpłaty do wyjaśnienia`. Następnie po imporcie edytować WB i poprawić wpłatę na prawidłowego właściciela, zgodnie z tytułem przelewu.

Zaimportowane wyciągi można dowolnie edytować i usuwać tak jak zwyczajny dekret. Można też je importować jeszcze raz, dodając do nazwy pliku frazę `_WYMUS_` lub wyłączając `Sprawdzanie powielania`. Cały proces importu pokazujemy na poniższym filmiku.

![Import wyciągu](importwbzwyklego.gif)

#### Edycja konta księgowego

Czasami zachodzi konieczność zmiany miejsca księgowania się operacji bankowych dla danego rachunku podmiotu. W systemie można to bez problemu zrealizować, aby to zrobić, należy:

- Zakładka `Zasoby` > menu `Funkcje` > `Importuj wyciąg elektroniczny`.
- Zakładka `Przypisanie kont`.
- Pole `Rachunek zasobu` > wybrać budynek i rachunek.
- Z prawej strony pozycji klikamy na ikonkę rysika ![Rysik](rysik.png), pozycja załaduje się do górnej części okna.
- Pole `Nazwa podmiotu` > będzie uzupełnione danymi nadawcy/odbiorcy przelewu.
- Pole `Treść` > będzie uzupełnione tytułem przelewu.
- Pole `Rachunek podmiotu` > pomijamy.
- Pole `Konto FK` > na podstawie wcześniejszych pól ustawiamy konto księgowe właściciela lub kontrahenta, ew. inne dowolne np. `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Konto FK zapłat` > można pozostawić puste. Podajemy tutaj konto do zapłat, jeżeli mają być one księgowane na innym koncie niż w polu `Konto FK`, można w ten sposób rozdzielić wpłaty i zapłaty.
- Kliknąć: `Dodaj`.
- Kliknąć: `Zatwierdź`.

![Edycja konta](importwbedycjakonta.gif)