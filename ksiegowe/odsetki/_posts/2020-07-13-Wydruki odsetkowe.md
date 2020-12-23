---
title: 5. Wydruki odsetkowe
---

# Wydruki odsetkowe

Przy sprawdzaniu i przedstawianiu właścicielom, za co zostały naliczone odsetki, warto skorzystać z niżej opisanych wydruków, powiązanych z odsetkami. W tym celu przechodzimy do:

- Zakładka `Administracja` > Menu `Funkcje` > `Wydruki`.

W zakładce `Osoby` są trzy podstawowe wydruki:

- `Kartoteka konta`
- `Odsetki`
- `Raport odsetkowy`

Dodatkowo są też dostępne zbiorcze wydruki w zakładce `Zasób`:

- `Raport odsetkowy`
- `Zaległości odsetkowe`
- `Zaległości płatnicze`

Wszystkie te wydruki opisujemy poniżej. [Przykład wydruków — Kliknij, aby pobrać.](wydrukiodsetkowe.pdf)

#### Kartoteka konta

Analizując odsetki, zawsze sprawdzamy kartotekę konta posortowaną wg terminów płatności. Wydruk domyślnymi ustawieniami będzie w porządku. Można też go ograniczyć do okresu, za który są zaksięgowane odsetki, stosując ustawienia:

- `Miesiąc początkowy` > pierwszy miesiąc okresu, za który zostały zaksięgowane odsetki.
- `Data końcowa` > pierwszy dzień miesiąca po okresie, za który zostały zaksięgowanie odsetki.
- `Pole Zakres` > `Wszystkie` lub `Termin płatności`.

![Kartoteka konta](wdrodskarkonta.png)

#### Odsetki

Główny wydruk dotyczący odsetek. Przedstawia on dokładne wyliczenia odsetek z podziałem na zakresy dat, w którym występowało zadłużenie na koncie rozrachunkowym. Występują w nim kolumny:

- `Od — Do` > to daty wynikające z kartoteki konta wg terminów płatności, nie dat księgowań dokumentów.
- `Zaległość odsetkowa` > to suma odsetek niezapłaconych (niepokrytych) z poprzedniego okresu.
- `Zaległość podstawowa` > to zadłużenie właściciela nieuwzględniające naliczonych odsetek.
- `Stopa` > to wartość rocznej stopy odsetkowej wykorzystywanej do obliczeń.
- `Dni` > to ilość dni, w których utrzymuje się zadłużenie właściciela.
- `Odsetki` > to wyliczona wartość odsetek w danym zakresie dat.
- `Odsetki narastająco` > to odsetki sumarycznie od początku okresu, za który są naliczane.

![Odsetki](wdrodsodsetki.png)

#### Raport odsetkowy

Wydruk, który prezentuje dane w rozbiciu na miesiące. W opcjach wydruku ustawiamy tylko miesiąc końcowy. Najważniejszą funkcją wydruku jest ukazanie właścicielowi, w którym miesiącu jego odsetki zostały pokryte. Tabelka zawiera kolumny:

- `Wpłaty` > suma uznań w danym miesiącu.
- `Naliczone obciążenia` > suma obciążeń na koncie właściciela (bez odsetek).
- `Naliczone odsetki` > suma zaksięgowanych odsetek, których termin płatności upływa w danym miesiącu.
- `Zapłacone obciążenia` > przedstawia kwotę, która została przeznaczona na pokrycie obciążeń właściciela.
- `Zapłacone odsetki` > przedstawia kwotę, która została przeznaczona na pokrycie odsetek naliczonych właścicielowi.
- `Nadpłaty` > to kwota, która została z wpłat po pokryciu naliczonych obciążeń i odsetek.
- `Zaległości obciążeniowe` > przedstawia pozostałą sumę obciążeń do zapłacenia.
- `Zaległości odsetkowe` > przedstawia pozostałą sumę odsetek do zapłacenia.

![Raport odsetkowy](wdrodsraportods.png)

#### Zaległości odsetkowe

Wydruk podobny do raportu odsetkowego, uproszczony do mniejszej ilości kolumn.

- `Nadpłata` > to kwota, która została z wpłat po pokryciu naliczonych obciążeń i odsetek.
- `Zaległość obciążeniowa` > przedstawia pozostałą sumę obciążeń do zapłacenia.
- `Zaległość odsetkowa` > przedstawia pozostałą sumę odsetek do zapłacenia.

![Zaległości odsetkowe](zaleglosciodsetkowe.png)

#### Zaległości płatnicze

Pozwala wydrukować zbiorcze zestawienie osób zalegających z opłatami na konkretną datę, zgodnie ze wskazanymi parametrami minimalnymi oraz maksymalnymi. Dokument może być wydrukowany w formie prezentowania indywidualnego (na każde konto osobno) lub zbiorczego (należności zostaną zsumowane). Konfiguracją i działaniem niektórych pól podobny jest do raportu Rozrachunki w zakładce Osoby. Dostępne są następujące opcje konfiguracji wydruku:

- `Data wydruku` > wybieramy datę.
- `Rodzaj zaległości` > wybieramy rodzaj zaległości:
    - `Właścicieli lokali` > pokazuje zaległości właścicieli na kontach.
    - `Wobec dostawców` > pokazuje zaległości wspólnoty wobec dostawców/kontrahentów.
- `Rozrachunki` > w jakiej formie mają zostać przedstawione na wydruku rozrachunki:
    - `Indywidualnie` > program przygotuje zestawienie dla wszystkich kont księgowych osobno.
    - `Zbiorczo` > wydruk zostanie przygotowany w formie zbiorczej — należności dla poszczególnych kont osób zostaną zsumowane razem — wykazani zostaną tylko globalnie zalegający (dla których suma należności spełnia kryteria wyszukiwania).
- `Sortowanie` > wybieramy, jak mają być poukładane pozycje na wydruku:
    - `Zaległość` > według kwoty zaległości malejąco — największe wartości z przodu/wyżej.
    - `Procent` > malejąco, wg stosunku zaległości (sumarycznie) do obciążeń w wybranym miesiącu — największe wartości procentowo (do obciążeń) z przodu/wyżej.
    - `Pierwszy lokal` > alfabetycznie/Rosnąco wg nazw/numerów lokali (dokładniej: pierwszego należącego do danej osoby).
    - `Klucz` > sortowanie w porządku alfabetycznym wg pola KLUCZ. Najczęściej kluczem jest nazwisko właściciela lokalu napisane wielkimi literami.
- `Minimalna/maksymalna zaległość` > kwota minimalna/maksymalna zaległości, jaka musi zaistnieć na dowolnym z kont księgowych właściciela/najemcy lub sumarycznie (patrz wyżej), aby osoba została pokazana na wydruku.
- `Minimalny/maksymalny procent` > wartość minimalna/maksymalna — wyrażona w procentach — jaką ma stanowić kwota zaległości w stosunku do ostatniego zaksięgowanego obciążenia zaliczkowego.
- `Zakres` > wybieramy, w jaki sposób ma być określony zakres, który dokument ma obejmować — np. wg daty księgowania, terminu płatności.
- `Pomiń pod konta` > mamy tutaj możliwość pominięcia pod konta na wydruku np. jeżeli chcemy pokazać tylko zaległości wobec Eksploatacji lub Funduszu remontowego.

! ! ! UWAGA ! ! !

- Pola `Minimalna zaległość` i `Minimalny procent` działają na poziomie każdego z kont księgowych osobno (jeśli takowe są zdefiniowane i rozliczane) lub sumarycznie — jeśli pole Rozrachunki zostanie ustawione na pozycję Zbiorczo. Przykładowo, możliwa jest sytuacja, w której uwzględniona zostanie na dokumencie osoba/firma posiadająca w sumie na swoim koncie księgowym (globalnie) dodatnie saldo (nadpłatę). Jest to możliwe tylko przy formie wydruku rozrachunków Indywidualnie i tylko wówczas, gdy na jednym z kont spełnione są warunki określone przez pola minimalne i rzeczywiście jest zaległość, a na innym jest wystarczająca nadpłata, aby (globalnie) tę zaległość pokryć.
- Między kryteriami wyboru `Minimalna zaległość` i `Minimalny procent` istnieje zależność logiczna koniunkcji (^ - logiczne i). Oznacza to, że na wydruku zaprezentowane będą tylko pozycje, które spełniają oba warunki jednocześnie — kwota zaległości jest powyżej wartości minimalnej i (jednocześnie) stanowi większy (od minimalnego) procent w stosunku do ostatniego zaksięgowanego obciążenia zaliczkowego.

![Zaległości płatnicze](zaleglosciplatnicze.png)