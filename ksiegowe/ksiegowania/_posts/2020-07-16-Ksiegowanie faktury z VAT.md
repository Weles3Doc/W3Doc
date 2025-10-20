---
title: Księgowanie kosztów z VAT
---

# Księgowanie kosztów z VAT

Aby zaksięgować faktury kosztowe z VAT, należy przejść do:

- Zakładka `Dekrety` > menu `Dokumenty` > `Dodaj dokument`.

W nagłówku okna uzupełniamy podstawowe pola dotyczace dekretu:

- Pole `Typ dokumentu FK` > `Faktury`.
- Pole `Data księgowania` > wskazujemy datę zadekretowania dokumentu.
- Pole `Opis dokumentu` > można zastosować wzór: `Koszty MM-RRRR`.

Następnie przechodzimy do wprowadzania pozycji:

- Pole `LP` > nr pozycji będzie się powiększał automatycznie.
- Pole `Data pozycji` > ustawiamy datę operacji księgowej.
- Pole `Termin płatności` > ustawiamy termin płatności faktury.
- Pole `Konto Wn` > pozostawiamy puste `-----`.
- Pole `Konto Ma` > zazwyczaj wskazujemy konto kontrahenta `202-xxxxxxxxx`.
- Pole `Dowód` > wpisujemy numer faktury.
- Pole `Treść` > opisujemy pozycję.
- Pole `Wartość` > podajemy kwotę **brutto** z dokumentu.
- Pole `St. VAT` > ustawiamy odpowiednią stawkę VAT.
- Pole `Typ` > te opcje służą do odpowiedniego oznaczenia pozycji w plikach JPK.
    - `Podzielona płatność` > mechanizm podzielonej płatności.
    - `Środki trwałe`. 
    - `Proporcja VAT`.
    - `Metoda kasowa`.
    - `GTU_12` > pozycja sprzedaży, która zalicza się do grupy GTU_12.
    - `Odbiorca powiązany` > pozycje na rzecz podmiotu powiązanego.
    - `Dokument WEW`.
    - `Rozliczenie w VAT kolejnym miesiącu`.
- Pole `Korekta` > pole odpowiada za oznaczanie korekt VATu w plikach JPK.
    - `Nie korekta` > zwyczajna pozycja.
    - `Korekta podstawy i VAT art. 89a ust. 1, 4` > związanych z uznaniem nieściągalności należności.
    - `Korekta VAT art. 89b ust. 1, 4` > związanych z opóźnieniem w opłaceniu faktury.
    - `Korekta VAT art. 90a-90c oraz art. 91` > korekta współczynnika proporcji VAT.
- Pole `VAT` > w tym polu podpowie się wartość podatku VAT, to pole można edytować, jeśli trzeba.
- Klikamy: `Dodaj`.

Dodajemy drugą pozycję.

- Pola `Data pozycji` i `Termin płatności` > bez zmian.
- Pole `Konto Wn` > wskazujemy konto kosztowe `400-.....`.
- Pole `Konto Ma` > ustawiamy puste `-----`.
- Pola `Dowód` i `Treść` > mogą zostać bez zmian.
- Pole `Wartość` > wprowadzamy wartość **netto** z faktury.
- Pole `St. VAT` > ustawiamy na `ND`.
- Klikamy: `Dodaj`.

W tym momencie można wprowadzić pozostałe pozycje danego dokumentu lub następne faktury kosztowe dotyczące danego miesiąca. Po wprowadzeniu wszystkiego:

- Klikamy: `Zatwierdź`.

Do wprowadzania pozycji można w każdej chwili powrócić, zaznaczając dokument > menu `Dokumenty` > `Edytuj dokument`.

Dodatkowe instrukcje:
- [Sprzedaż ZW](https://nowoczesnyzarzadca.pl/2020/11/25/sprzedaz_ZW.html)
- [JPK_V7](https://nowoczesnyzarzadca.pl/2020/09/22/JPK_V7.html)
- [Założenia JPK_V7](https://doc.weles3.pl/ksiegowe/eksportplikowpodatkowych/Zalozenia-JPK_V7.html)

![Koszt z VAT](kosztzvat.gif)

#### Księgowanie z proporcją VAT

Niektóre zasoby prowadzą działalność mieszaną, czyli mają w swoich strukturach zarówno lokale opodatkowane, jak i zwolnione z VAT. W takich przypadkach system pozwala na zaksiegowanie kosztów w podziale na części przypadające na VAT i te na obroty zwolnione.

Zasada księgowania faktury kosztowej z podziałem VAT:

1. Pierwsza pozycja - część kwoty z faktury przypadająca na VAT.
 - Pole `Konto Wn` > pozostawiamy puste `-----`.
 - Pole `Konto Ma` > wskazujemy konto dostawcy `202-xxxxxxxxx`.
 - Pole `Wartość` > podajemy kwotę **brutto** kosztu, przypadającą na VAT.
 - Pole `St. VAT` > ustawiamy odpowiednią stawkę VAT.
 - Pole `Typ` > można pozostawić puste lub wybierać właściwą opcję.
 - Pole `Korekta` > można pozostawić puste lub wybierać właściwą opcję.
 - Klikamy: `Dodaj`.

2. Druga pozycja - część kwoty z faktury przypadająca na zwolnienie z VAT.
 - Pole `Konto Wn` > pozostawiamy puste `-----`.
 - Pole `Konto Ma` > wskazujemy konto dostawcy `202-xxxxxxxxx`.
 - Pole `Wartość` > podajemy kwotę **brutto** kosztu, przypadającą na zwolnienie z VAT.
 - Pole `St. VAT` > wybieramy `ND`.
 - Klikamy: `Dodaj`.

3. Trzecia pozycja - kwota kosztu netto z faktury przypadająca na VAT.
 - Pole `Konto Wn` > wskazujemy konto FK kosztu 400-..., dotyczące kosztów VATowych.
 - Pole `Konto Ma` > pozostawiamy puste `-----`.
 - Pole `Wartość` > podajemy kwotę **netto** kosztu, przypadającą na VAT z punktu `1`.
 - Pole `St. VAT` > wybieramy `ND`.
 - Klikamy: `Dodaj`.

4. Czwarta pozycja - kwota kosztu z faktury przypadająca na zwolnienie z VAT.
 - Pole `Konto Wn` > wskazujemy konto FK kosztu 400-..., dotyczące kosztów zwolnionych z VAT.
 - Pole `Konto Ma` > pozostawiamy puste `-----`.
 - Pole `Wartość` > podajemy kwotę **brutto** kosztu, przypadającą na zwolnienie z VAT z punktu `2`.
 - Pole `St. VAT` > wybieramy `ND`.
 - Klikamy: `Dodaj`.

Po wprowadzeniu wszystkiego:

- Klikamy: `Zatwierdź`.

Przykład przed zaksięgowaniem:

![Koszt z VAT](propVAT1.png)

Przykład dekretu po zaksięgowaniu:

![Koszt z VAT](propVAT2.png)