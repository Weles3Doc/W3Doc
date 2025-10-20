---
title: Księgowanie faktur kosztowych
---

# Księgowanie faktur kosztowych

Aby zaksięgować faktury kosztowe, należy przejść do:

- Zakładka `Dekrety` > menu `Dokumenty` > `Dodaj dokument`.
- Pole `Typ dokumentu FK` > ustawiamy `Faktury`.
- Pole `Data księgowania` > wskazujemy datę zadekretowania dokumentu, zazwyczaj koniec miesiąca.
- Pole `Opis dokumentu` > można zastosować wzór: `Koszty MM-RRRR` jeśli wprowadzamy zbiorczo. Można też tutaj umieścić numer dokumentu jeśli koszty wprowadzamy pojedynczo w dekretach. 

Następnie przechodzimy do wprowadzania pozycji:

- Pole `LP` > nr pozycji będzie się powiększał automatycznie.
- Pole `Data pozycji` > ustawiamy datę operacji księgowej.
- Pole `Termin płatności` > ustawiamy termin płatności faktury.
- Pole `Konto Wn` > zazwyczaj wskazujemy konto kosztowe 400-.....
- Pole `Konto Ma` > zazwyczaj wskazujemy konto kontrahenta 202-.....
- Pole `Dowód` > pisujemy numer faktury.
- Pole `Treść` > opisujemy pozycję.
- Pole `Wartość` > podajemy kwotę brutto z dokumentu.
- Pole `St. VAT` > pomijamy, pozostawiamy bez zmian.
- Klikamy: `Dodaj`.

Wprowadzamy następne faktury kosztowe dotyczące danego miesiąca. Gdy wszystkie pozycje będą dodane na koniec:

- Kliknąć: `Zatwierdź`.

Do wprowadzania pozycji można w każdej chwili powrócić, zaznaczając dokument > menu `Dokumenty` > `Edytuj dokument`.

![Księgowanie kosztów](ksiegowaniekosztu.gif)

#### Prowadzenie kosztów 

Zdecydowanie większość użytkowników prowadzi koszty zasobu w jednym dekrecie w miesiącu. Ten dekret zazwyczaj jest tworzony z ostatnim dniem miesiąca. Gdy wpłynie nowy koszt do zaksięgowania, jest on dodawany przez `Edytuj dokument`. Poniżej przykład:

![Księgowanie kosztów](ksieg_koszt_jed_dekret.png)

Koszty można też rejestrować pojedynczo, na zasadzie jeden dekret = jedna faktura kosztowa. Poniżej przykład:

![Księgowanie kosztów](ksieg_koszt_wiele_dekret.png)

#### Rozbijanie kosztów

Niektóre koszty wspólnoty mogą wymagać podziału na różne konta księgowe, na przykład, koszty ciepła. Aby wprowadzić taki podział należy:

W pierwszej wprowadzanej pozycji wykazać sumaryczną kwotę na kontrahencie.

- Pole `Konto Wn` > **puste**. Pole `Konto Ma` > 202-... Dostawca.

W kolejnych pozycjach dokonujemy podziału kwoty i wskazania kona kosztowego:

- Pole `Konto Wn` > 400-... koszt. Pole `Konto Ma` > **puste**.
- Pole `Konto Wn` > 400-... koszt. Pole `Konto Ma` > **puste**.
- Pole `Konto Wn` > 400-... koszt. Pole `Konto Ma` > **puste**.
- itd.

Przykład przed zaksięgowaniem:

![Księgowanie kosztów](ksieg_koszt_rozb_poz_1.png)

Po zaksięgowaniu:

![Księgowanie kosztów](ksieg_koszt_rozb_poz_2.png)