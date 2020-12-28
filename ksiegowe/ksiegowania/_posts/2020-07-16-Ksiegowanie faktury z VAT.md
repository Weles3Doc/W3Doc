---
title: Księgowanie faktury z VAT
---

# Księgowanie faktury z VAT

Aby zaksięgować faktury kosztowe z VAT, należy przejść do:

- Zakładka `Dekrety` > menu `Dokumenty` > `Dodaj dokument`.
- Pole `Typ dokumentu FK` > `Faktury`.
- Pole `Data księgowania` > wskazujemy datę zadekretowania dokumentu.
- Pole `Opis dokumentu` > można zastosować wzór: `Koszty MM-RRRR`. 
- Pole `LP` > nr pozycji będzie się powiększał automatycznie.
- Pole `Data pozycji` > ustawiamy datę operacji księgowej.
- Pole `Termin płatności` > ustawiamy termin płatności faktury.
- Pole `Konto Wn` > pozostawiamy puste `-----`.
- Pole `Konto Ma` > zazwyczaj wskazujemy konto kontrahenta `202-xxxxxxxxx`.
- Pole `Dowód` > wpisujemy numer faktury.
- Pole `Treść` > opisujemy pozycję.
- Pole `Wartość` > podajemy kwotę brutto z dokumentu.
- Pole `St. VAT` > ustawiamy odpowiednią stawkę VAT.
- Pole `Typy` > 
    - `Podzielona płatność` > 
    - `Środki trwałe` > 
    - `Proporcja VAT` > 
    - `Metoda kasowa` > 
    - `GTU_12` > 
    - `Odbiorca powiązany` > 
    - `Dokument WEW` > 
- Pole `Korekta` > 
    - `Nie korekta` > 
    - `Korekta podstawy i VAT art. 89a ust. 1, 4` > 
    - `Korekta VAT art. 89b ust. 1, 4` > 
    - `Korekta VAT art. 90a-90c oraz art. 91` > 
- Pole `VAT` > w tym polu podpowie się wartość podatku VAT, to pole można edytować, jeśli trzeba.
- Klikamy: `Dodaj`.

Dodajemy drugą pozycję.

- Pola `Data pozycji` i `Termin płatności` > bez zmian.
- Pole `Konto Wn` > wskazujemy konto kosztowe `400-.....`.
- Pole `Konto Ma` > ustawiamy puste `-----`.
- Pola `Dowód` i `Treść` > mogą zostać bez zmian.
- Pole `Wartość` > wprowadzamy wartość netto z faktury.
- Pole `St. VAT` > ustawiamy na `ND`.
- Klikamy: `Dodaj`.

W tym momencie można wprowadzić pozostałe pozycje danego dokumentu lub następne faktury kosztowe dotyczące danego miesiąca. Po wprowadzeniu wszystkiego:

- Pole `Hasło` > wpisujemy hasło.
- Klikamy: `Zatwierdź`.

Do wprowadzania pozycji można w każdej chwili powrócić, zaznaczając dokument > menu `Dokumenty` > `Edytuj dokument`.

![Koszt z VAT](kosztzvat.gif)