---
tilte: Dodanie bilansu otwarcia
---
# Dodanie bilansu otwarcia

Bilans otwarcia jest dokumentem, określającym stan nieruchomości na dany dzień (zazwyczaj jest to dzień przejęcia lub koniec roku). Są w nim zawarte salda kont księgowych. Chcąc wprowadzić dokument BO do danej WM baza musi mieć utworzone odpowiednie konta w ogólnym planie kont. Kolejnym niezbędnym krokiem przed wprowadzeniem dokumentu BO jest określenie Kont należności, czyli sposobu księgowania na kontach właścicieli, czy obciążenia na kontach właścicieli będą księgowane na jednym koncie Rozrachunki, czy w rozbiciu na tzw. Zaliczkę (Media i eksploatacja) i Fundusz (Fundusz remontowy). Bilans otwarcia dodajemy do systemu tylko raz, w momencie zakładania WM w systemie. Później jest on tworzony automatycznie przy zamykaniu roku. W systemie występują dwa rodzaje bilansu otwarcia:

- BO — wprowadzamy w nim normalne salda kont księgowych.
- BO-ODS — wprowadzamy tutaj tylko i wyłącznie saldo zaległości odsetkowej, tzw. odsetki. Od sald wprowadzonych w tym typie BO nie będą liczone ewentualne odsetki.

Aby wprowadzić lub edytować bilans otwarcia, należy przejść do:

- Zakładka `Dekrety`.
- Na liście dokumentów, BO jest zawsze prezentowane jako pierwsze.
- Zaznaczyć dokument BO lub BO-ODS.
- Menu `Dokumenty` > `Edytuj dokument`.

Edycja BO przebiega tak samo, jak edycja innych dokumentów:

- Pole `Typ dokumentu FK` > `BO` (zdefiniowane na stałe).
- Pole `Data księgowania` > `BO` (zdefiniowane na stałe).
- Pole `Opis dokumentu` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `LP` > będzie się powiększało automatycznie.
- Pole `Data pozycji` > `BO` (zdefiniowane na stałe).
- Pole `Termin płatności` > `BO` lub naciskamy spację, aby ustawić datę.
- Pole `Konto Wn` > wskazujemy konto księgowe, dla którego wprowadzamy saldo.
- Pole `Konto Ma` > wskazujemy konto księgowe, dla którego wprowadzamy saldo.
- Pole `Dowód` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `Treść` > można np. wpisać: BO na 1 czerwca 2020.
- Pole `Wartość` > podajemy saldo konta.
- Pole `St. VAT` > pomijamy, pozostawiamy bez zmian.
- Klikamy: `Dodaj`.
- Wprowadzamy następne pozycje z saldami kont.
- Wpisujemy hasło i zatwierdzamy.

### Uwagi:

- Salda kont w pozycjach — definiujemy **jednostronnie**, czyli:
  - Jeśli saldo konta jest na minus, to w polach:
    - `Pole Wn` > ustawiamy to konto.
    - `Pole Ma` > pozostawiamy puste `-----`.
  - Jeśli saldo konta jest na plus, to w polach:
    - `Pole Wn` > pozostawiamy puste `-----`.
    - `Pole Ma` > ustawiamy to konto.
  - Jest to częstą przyczyną źle wprowadzonego bilansu otwarcia — jedna pozycja nie może mieć podanego konta Wn i Ma na raz (Ważne).
- Jeśli wprowadzanie BO trzeba przerwać z jakichś powodów, to dokument tymczasowo można zbilansować na koncie 999-01 i zapisać. W późniejszym czasie można powrócić do edycji, usunąć pozycję 999-01 i kontynuować wprowadzanie sald.
- W systemie księgujemy na kontach analitycznych, niesyntetycznych.

### Dokument BO a rozliczenie liczników/kosztów

Zdarza się, że dysponujemy dokumentem BO na dzień przejęcia WM (np 2020-03-01) a musimy jeszcze rozliczyć liczniki/koszty za cały rok (czyli od 2020-01-01). W takim wypadku konieczne jest odtworzenie zaliczek od początku rozliczanego okresu, tylko wtedy system będzie miał pełne informacje na temat naliczonych obciążeń. Będą do tego potrzebne wszystkie zmiany stawek, danych, sposobu naliczania zaliczek, prognoz liczników, wykupy lokali itp. Dodatkowo potrzebne będą odczyty liczników z początku rozliczanego okresu. Same zaliczki zaraz po zaksięgowaniu należy wyzerować, robimy to MY (tj dział wsparcia PHU WELES) - wtedy odtworzone zaliczki nie będą kolidowały z wprowadzonym BO a system będzie miał pełne informacje na temat zaksięgowanych obciążeń. W celu odtworzenie zaliczek należy zgłosić się do NAS (tj działu wsparcia PHU WELES). 