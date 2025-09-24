---
tilte: Dodanie bilansu otwarcia
---

# Dodanie bilansu otwarcia

Bilans otwarcia jest dokumentem, określającym stan nieruchomości na dany dzień (zazwyczaj jest to dzień przejęcia lub koniec roku), są w nim zawarte salda kont księgowych. Bilans otwarcia dodajemy do systemu tylko raz, w momencie zakładania zasobu w systemie. Później jest on tworzony automatycznie przy zamykaniu roku. Przed wprowadzeniem bilansu trzeba w programie wykonać kilka czynności:

- Utworzyć konta rozrachunkowe właścicieli (podkonta 201). Instrukcja: **Konta rozrachunkowe właścicieli**.
- Dodać kontrahentów. Instrukcja: **Edycja kontrahentów**.
- Zdefiniować i zaksięgować przynajmniej jeden miesiąc zaliczek.
- Dodać konta syntetyczne i analityczne, czyli utworzyć plan kont.

 W systemie występują dwa rodzaje bilansu otwarcia:

- `BO` — wprowadzamy w nim normalne salda kont księgowych.
- `BO-ODS` — wprowadzamy tutaj tylko i wyłącznie **saldo zaległości odsetkowej**, tzw. odsetki, a dokładniej odsetki, które nie zostały jeszcze zapłacone, pokryte. Od pozycji tutaj wprowadzonych, **nie będą liczone odsetki**.

#### Zasady wprowadzania BO

- Salda kont w pozycjach — definiujemy **jednostronnie**, nie definiujemy konta przeciwstawnego, czyli:
  - Jeśli saldo konta ma saldo po stronie `Wn`, to w polach:
    - `Pole Wn` > ustawiamy to konto.
    - `Pole Ma` > pozostawiamy puste `-----`.
  - Jeśli saldo konta ma saldo po stronie `Ma`, to w polach:
    - `Pole Wn` > pozostawiamy puste `-----`.
    - `Pole Ma` > ustawiamy to konto.
- Jest to częstą przyczyną źle wprowadzonego bilansu otwarcia — jedna pozycja nie może mieć podanego konta Wn i Ma na raz (**Ważne!!**).
- Jeśli wprowadzanie BO trzeba przerwać z jakichś powodów, to dokument tymczasowo można zbilansować na koncie 999-01 i zapisać. W późniejszym czasie można powrócić do edycji, usunąć pozycję 999-01 i kontynuować wprowadzanie sald.
- BO nie powinno mieć obrotów na koncie 999.
- Dobrze wprowadzone BO same się bilansuje, to jest, suma obrotów Wn równa się sumie obrotów Ma.
- W systemie księgujemy na kontach analitycznych, niesyntetycznych.

#### Dodanie / Edycja bilansu otwarcia

Edycja bilansu przebiega tak samo, jak wprowadzanie zwyczajnego dokumentu. Aby wprowadzić lub edytować bilans otwarcia, należy przejść do:

- Zakładka `Dekrety`.
- Na liście dokumentów zaznaczyć dokument BO lub BO-ODS, są one zawsze prezentowane jako ostatnie.
- Menu `Dokumenty` > `Edytuj dokument`.
- Pole `Typ dokumentu FK` > `BO` (zdefiniowane na stałe).
- Pole `Data księgowania` > `BO` (zdefiniowane na stałe).
- Pole `Opis dokumentu` > można np. wpisać: BO na 1 czerwca 2025.
- Pole `LP` > będzie się powiększało automatycznie.
- Pole `Data pozycji` > `BO` lub **naciskamy spację**, aby ustawić datę `DP`, jeśli wypada ona później niż data bilansu.
- Pole `Termin płatności` > `BO` lub **naciskamy spację**, aby ustawić datę `TP`, jeśli wypada on później niż data bilansu.
- Pole `Konto Wn` > wskazujemy konto księgowe, dla którego wprowadzamy saldo.
- Pole `Konto Ma` > wskazujemy konto księgowe, dla którego wprowadzamy saldo.
- Pole `Dowód` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `Treść` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `Wartość` > podajemy saldo konta.
- Pole `St. VAT` > pomijamy, pozostawiamy bez zmian.
- Klikamy: `Dodaj`.
- Wprowadzamy następne pozycje z saldami kont.
- Jeśli wprowadziliśmy wszystkie salda i dokument się bilansuje, to można go zapisać. Jeśli się nie bilansuje, to tymczasowo można go zbilansować na koncie technicznym `999-01`.
- Klikamy `Zatwierdź`.

Poniżej prezentujemy przykładowe dodawanie sald w BO. Do edycji BO można w każdej chwili powrócić. 

![Przykład edycji BO](edycjabo.gif)

#### Dokument BO a rozliczenie liczników/kosztów

Zdarza się, że dysponujemy dokumentem BO na dzień przejęcia WM w środku roku (np. 2020-05-01) a musimy jeszcze rozliczyć liczniki/koszty za cały rok (czyli od 2020-01-01). W takim wypadku konieczne jest odtworzenie zaliczek od początku rozliczanego okresu, tylko wtedy system będzie miał pełne informacje na temat naliczonych zaliczek. Będą do tego potrzebne wszystkie zmiany stawek, danych, sposobu naliczania zaliczek, prognoz liczników, wykupy lokali itp. Dodatkowo potrzebne będą odczyty liczników z początku rozliczanego okresu. Odtworzone zaliczki zaraz po zaksięgowaniu należy wyzerować w części księgowej, aby nie tworzyły obrotów przed BO, robimy to MY (tj dział wsparcia WELES3) - wtedy odtworzone zaliczki nie będą kolidowały z wprowadzonym BO a system będzie miał pełne informacje na temat zaksięgowanych obciążeń. W celu odtworzenie zaliczek należy zgłosić się do działu wsparcia WELES.

Jeśli w wprowadzanym BO znajdują się rozliczenia lub pozycje z późniejszym terminem płatności, to trzeba je wydzielić na osobne pozycje i następnie w polu Termin płatności określić inną datę niż BO. Przykład poniżej, lokal M01 ma z głównego salda na koniec roku, wydzielone pozycje z rozliczeniami, które mają przyszły termin płatności - tak wprowadzone BO gwarantuje poprawne naliczenie odsetek.

![Rozbicie sald w BO](rozbiciesaldwbo.png)

#### Import sald właścicieli do BO

W systemie można zaimportować salda właścicieli (salda kont 201). Salda pozostałych kont należy wprowadzić samodzielnie. Aby zaimportować salda, trzeba stworzyć tabelkę, która będzie się składała z 5 kolumn. Przykład tabelki:

![Przykład tabelki import BO](imprtbotabelka.png)

Gdzie:

- Pierwsza kolumna:
  - Nagłowek > umieszczamy tutaj specjalny ciąg znaków, który określa parametry importu BO:
    - `WMBO 999-01` > importowane pozycje podmieniają już istniejące salda w BO.
    - `WMBO= 999-01` > usuwa wszystkie dotychczasowe pozycje w BO właścicieli przed importem.
    - `WMBO+ 999-01` > importowane pozycje są dodawane jako kolejne do BO (nie zastępuje istniejących).
  - Kolejne wiersze > podajemy numer lokalu oraz numer konta rozrachunkowego, są one oddzielone znakiem pionowej kreski `|` (znak ten zazwyczaj znajduje się obok Enteru). Przykład: `M001|1`. Numer lokalu musi być taki sam jak w systemie. Numery (id) podkont rozrachunkowych można sprawdzić w zakładka `Administracja` > menu `Elementy` > `Konta należności`.
- Druga kolumna:
  - Nagłowek > wpisujemy `WN`.
  - Kolejne wiersze > wpisujemy kwoty (salda) do zaimportowania w danej pozycji po stronie Wn rozrachunków 201 właściciela.
- Trzecia kolumna:
  - Nagłowek > wpisujemy `MA`.
  - Kolejne wiersze > wpisujemy kwoty (salda) do zaimportowania w danej pozycji po stronie Ma rozrachunków 201 właściciela.
- Czwarta kolumna:
  - Nagłowek > wpisujemy `TR`.
  - Kolejne wiersze > uzupełniamy w nich dowolny tekst, np. `Bilans na 2020-01-01`.
- Piąta kolumna:
  - Nagłowek > wpisujemy `TP`.
  - Kolejne wiersze > jeśli kwota (saldo) jest na dzień BO to wpisujemy `1000-01-01`. Natomiast jeśli importujemy kwotę z przyszłym terminem płatności to wpisujemy tutaj faktyczny termin płatności pozycji, w formacie `RRRR-MM-DD`.

Kwotę uzupełniamy jednostronnie, albo po stronie Wn albo po stronie Ma, nigdy dwie strony na raz. Numer konta technicznego w nagłówku pierwszej kolumny należy poprawić na zgodny z planem kont, najczęściej jest to `999-01`, czasami zdarza się też `999-1`. Po imporcie można takie BO edytować i dokończyć wprowadzanie sald.

Gdy tabelka jest już przygotowana:

- Kopiujemy tabelkę wraz z tytułami kolumn z arkusza.
- Zakładka `Dekrety` > menu `Funkcje` > `Import danych`.
- Pole `Dane` > wklejamy tabelkę.
- Klikamy `Zatwierdź`.

Poniżej przedstawiamy sposób importu poprawnej tabelki. BO można importować wielokrotnie.

![Import BO](importbo.gif)

#### Import sald odsetkowych właścicieli

Salda odsetkowe właścicieli trzeba wydzielić od zwykłych sald i wprowadzić do specjalnego tylu bilansu otwarcia `BO-ODS`. System od umieszczonych tutaj sald nie będzie liczył kolejnych odsetek.

Sposób importu jest taki sam, z tym że, w tabelce w pierwszej kolumnie stosujemy inny nagłówek:
- `WMBOO 999-01` > importowane pozycje podmieniają już istniejące salda w BO-ODS.
- `WMBOO= 999-01` > usuwa wszystkie dotychczasowe pozycje w BO-ODS właścicieli przed importem.
- `WMBOO+ 999-01` > importowane pozycje są dodawane jako kolejne do BO-ODS (nie zastępuje istniejących).

Salda odsetkowe umieszczamy tylko i wyłącznie w kolumnie `WN`. Saldo odsetkowe musi być kwotą dodatnią. W nagłówku pierwszej kolumny zamiast konta `999-01`, można od razu umieścić konto odsetkowe np. `720-1`. Poniżej przykład tabelki:

![Przykład tabelki import BO-ODS](tabelkaboods.png)

Sposób importu:

![Import BO-ODS](importboods.gif)

#### Szybki wydruk BO

![Wydruk BO lub BO-ODS](szybkiwydrukbo.png)
