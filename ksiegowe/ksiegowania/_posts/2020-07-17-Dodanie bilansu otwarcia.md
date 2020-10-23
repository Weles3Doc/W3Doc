---
tilte: Dodanie bilansu otwarcia
---

# Dodanie bilansu otwarcia

Bilans otwarcia jest dokumentem, określającym stan nieruchomości na dany dzień (zazwyczaj jest to dzień przejęcia lub koniec roku), są w nim zawarte salda kont księgowych. Bilans otwarcia dodajemy do systemu tylko raz, w momencie zakładania WM w systemie. Później jest on tworzony automatycznie przy zamykaniu roku. Przed wprowadzeniem bilansu trzeba w programie wykonać kilka czynności:

- Utworzyć konta rozrachunkowe właścicieli (podkonta 201). Instrukcja: **Konta rozrachunkowe właścicieli**.
- Dodać kontrahentów. Instrukcja: **Edycja kontrahentów**.
- Zdefiniować i zaksięgować przynajmniej jeden miesiąc zaliczek.
- Dodać konta syntetyczne i analityczne, czyli utworzyć plan kont.

 W systemie występują dwa rodzaje bilansu otwarcia:

- `BO` — wprowadzamy w nim normalne salda kont księgowych.
- `BO-ODS` — wprowadzamy tutaj tylko i wyłącznie **saldo zaległości odsetkowej**, tzw. odsetki, a dokładniej odsetki, które nie zostały jeszcze zapłacone, pokryte. Od sald tutaj wprowadzonych, **nie będą liczone odsetki**.

#### Zasady wprowadzania BO

- Salda kont w pozycjach — definiujemy **jednostronnie**, nie definiujemy konta przeciwstawnego, czyli:
  - Jeśli saldo konta jest na minus, to w polach:
    - `Pole Wn` > ustawiamy to konto.
    - `Pole Ma` > pozostawiamy puste `-----`.
  - Jeśli saldo konta jest na plus, to w polach:
    - `Pole Wn` > pozostawiamy puste `-----`.
    - `Pole Ma` > ustawiamy to konto.
- Jest to częstą przyczyną źle wprowadzonego bilansu otwarcia — jedna pozycja nie może mieć podanego konta Wn i Ma na raz (**Ważne!!**).
- Jeśli wprowadzanie BO trzeba przerwać z jakichś powodów, to dokument tymczasowo można zbilansować na koncie 999-01 i zapisać. W późniejszym czasie można powrócić do edycji, usunąć pozycję 999-01 i kontynuować wprowadzanie sald.
- BO nie powinno mieć obrotów na koncie 999.
- Dobrze wprowadzone BO same się bilansuje, to jest, suma obrotów Wn równa się sumie obrotów Ma.
- W systemie księgujemy na kontach analitycznych, niesyntetycznych.

#### Edycja bilansu otwarcia

Edycja bilansu przebiega tak samo, jak wprowadzanie zwyczajnego dokumentu. Aby wprowadzić lub edytować bilans otwarcia, należy przejść do:

- Zakładka `Dekrety`.
- Na liście dokumentów zaznaczyć dokument BO lub BO-ODS, są one zawsze prezentowane jako ostatnie.
- Menu `Dokumenty` > `Edytuj dokument`.
- Pole `Typ dokumentu FK` > `BO` (zdefiniowane na stałe).
- Pole `Data księgowania` > `BO` (zdefiniowane na stałe).
- Pole `Opis dokumentu` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `LP` > będzie się powiększało automatycznie.
- Pole `Data pozycji` > `BO` (zdefiniowane na stałe).
- Pole `Termin płatności` > `BO` lub **naciskamy spację**, aby ustawić datę TP, jeśli wypada on później niż data bilansu.
- Pole `Konto Wn` > wskazujemy konto księgowe, dla którego wprowadzamy saldo.
- Pole `Konto Ma` > wskazujemy konto księgowe, dla którego wprowadzamy saldo.
- Pole `Dowód` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `Treść` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `Wartość` > podajemy saldo konta.
- Pole `St. VAT` > pomijamy, pozostawiamy bez zmian.
- Klikamy: `Dodaj`.
- Wprowadzamy następne pozycje z saldami kont.
- Jeśli wprowadziliśmy wszystkie salda i dokument się bilansuje, to można go zapisać. Jeśli się nie bilansuje, to tymczasowo można go zbilansować na koncie 999-01.
- Wpisujemy hasło i zatwierdzamy.

Poniżej prezentujemy przykładowe dodawanie sald w BO. Do edycji BO można w każdej chwili powrócić. 

![Przykład edycji BO](edycjabo.gif)

#### Dokument BO a rozliczenie liczników/kosztów

Zdarza się, że dysponujemy dokumentem BO na dzień przejęcia WM w środku roku (np. 2020-05-01) a musimy jeszcze rozliczyć liczniki/koszty za cały rok (czyli od 2020-01-01). W takim wypadku konieczne jest odtworzenie zaliczek od początku rozliczanego okresu, tylko wtedy system będzie miał pełne informacje na temat naliczonych zaliczek. Będą do tego potrzebne wszystkie zmiany stawek, danych, sposobu naliczania zaliczek, prognoz liczników, wykupy lokali itp. Dodatkowo potrzebne będą odczyty liczników z początku rozliczanego okresu. Odtworzone zaliczki zaraz po zaksięgowaniu należy wyzerować w części księgowej, aby nie tworzyły obrotów przed BO, robimy to MY (tj dział wsparcia WELES3) - wtedy odtworzone zaliczki nie będą kolidowały z wprowadzonym BO a system będzie miał pełne informacje na temat zaksięgowanych obciążeń. W celu odtworzenie zaliczek należy zgłosić się do działu wsparcia WELES.

#### Import sald właścicieli do BO

W systemie można zaimportować salda właścicieli (salda kont 201). Salda pozostałych kont należy wprowadzić samodzielnie. Aby zaimportować salda, trzeba stworzyć tabelkę, która będzie się składała z 3 kolumn. Przykład tabelki:

![Przykład tabelki import BO](imprtbotabelka.png)

Gdzie:

- Kolumna `MIE` > podajemy numer lokalu oraz numer konta rozrachunkowego, są one oddzielone znakiem pionowej kreski `|` (znak ten zazwyczaj znajduje się obok Enteru). Przykład: `M01|1`. Numer lokalu musi być taki sam jak w systemie. Numery (id) podkont rozrachunkowych można sprawdzić w zakładka `Administracja` > menu `Elementy` > `Konta należności`.
- Kolumna `TR` > uzupełniamy w niej dowolny tekst, np. `Bilans na 2020-01-01`.
- Ostatnia kolumna musi mieć określony nagłówek: `BO` spacja `nr konta technicznego`. Przykład: `BO 999-01`. Numer konta technicznego to zazwyczaj 999-01 lub 999-1, należy sprawdzić w planie kont. W tej kolumnie wpisujemy salda właścicieli:
  - Jeśli właściciel jest na `minus`, to kwotę wprowadzamy ze `znakiem ujemnym`. Saldo zaimportuje się po stronie Wn konta 201.
  - Jeśli właściciel jest na `plus`, to kwotę wprowadzamy ze `znakiem dodatnim`. Saldo zaimportuje się po stronie Ma konta 201.

Dodatkowo zamiast nagłówka (wrażenia) `BO` można użyć:
- `BO` > importowane pozycje podmieniają już istniejące salda w BO.
- `BOO` > importowane pozycje podmieniają już istniejące salda w BO-ODS.
- `BO=` > 
- `BOO=` > 
- `BO+` > importowane pozycje są dodawane jako kolejne do BO (nie zastępuje istniejących).
- `BOO+` > importowane pozycje są dodawane jako kolejne do BO-ODS (nie zastępuje istniejących).

Gdy tabelka jest już przygotowana:

- Kopiujemy tabelkę wraz z tytułami kolumn z arkusza.
- Zakładka `Dekrety` > menu `Funkcje` > `Import danych`.
- Pole `Dane` > wklejamy tabelkę.
- Wpisujemy hasło i zatwierdzamy.

Poniżej przedstawiamy sposób importu poprawnej tabelki. BO można importować wielokrotnie.

![Import BO](importbo.gif)