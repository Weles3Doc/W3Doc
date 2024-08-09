---
title: 4. Przeliczenie rozliczenia
---

# Przeliczenie rozliczenia

Po dodaniu odczytów na koniec okresu rozliczeniowego można przejść do przeliczenia i sprawdzenia rozliczenia. Aby to zrobić, należy przejść do:

- Zakładka `Administracja`.
- W polu struktury zaznacz cały zasób.
- Przycisk: `Naliczenia`.
- Zaznacz: `K.bieżąca`.
- Menu `Obciążenia` > `Nalicz korekty RL`.

Rozliczenie przeliczamy dla całego zasobu, w polu `Struktura`, zaznaczając najwyższy element (cały budynek). Dzięki temu wystarczy to zrobić tylko raz, można przeliczać też na podległych strukturach lub na lokalach.

Klikając `Nalicz korekty RL`, są przeliczane korekty zwyczajne, rozliczenia liczników, należy sprawdzić więc, czy oprócz pożądanych pozycji nie naliczają się zbędne korekty, które należałoby wykasować lub zaksięgować przed.

Rozliczenie można w tym momencie poprawiać i przeliczać do woli. Właściciele nie widzą niezaksięgowanych rozliczeń.

Porównaj zużycie w kolumnie `Ilość` w `K. bieżąca` do zużycia prezentowanego pod przyciskiem `Liczniki`. Duża ilość liczb po przecinku może sugerować że z rozliczeniem jest coś nie tak. Rozbieżność w tych polach może sugerować na pomijanie liczników w rozliczeniu lub zerową stawkę.

Kolumna `Było Wartość` prezentuje przychody które biorą udział w rozliczeniach. Porównaj tą kwotę z kwotą przychodów na koncie 7xx składnika. Zazwyczaj sie zgadzają, ale  nie zawsze, w rozliczeniu nie zostaną uwzględnione opłaty lokali ryczałtowych.

Kolumna `Ma być Wartość` to wynik mnożenia kolumn `Ilość` i `Stawka`.

Kolumna `Wartość` to różnica kolumn `Było Wartość` i `Ma być Wartość`. Kwota z plusem to dopłata (obciążenie), kwota z minusem to nadpłata (zwrot) właściciela.

![Przeliczenie RL](przeliczenierl.gif)

#### Sprawdzenie zużyć

Zużycia będą dostępne od razu po przeliczeniu rozliczenia, w kolumnie `Ilość` przy pozycjach oznaczonych jako `(LZ)`. Oczywiście zużycia można sprawdzić na całej WM lub na strukturze albo na pojedynczym lokalu. Obowiązkowo należy porównać zużycie całego budynku z `K.bieżąca` z zużyciem widocznym pod przyciskiem `Liczniki`. Różnice te mogą wskazywać na zerowe stawki lub pomijane zużycie. Dodatkowo należy zwrócić uwagę na ilość cyfr po przecinku w zużyciu w rozliczeniu. Jeśli lokal właściciela został wcześniej rozliczony to jego zuzycie (i rozliczenie) może nie prezentować się w rozliczeniu.

Do sprawdzania zużyć służy też zbiorczy wydruk:

- Menu `Funkcje` > `Wydruki` > `Zasób` > `Zużycia liczników`.

![Sprawdzenie rozliczenia](sprrozliczenia1.gif)

#### Sprawdzenie struktury rozliczenia

Sprawdzenie struktury korekty na całym zasobie i na lokalach pozwala wyłapać częste błędy przy rozliczeniu:

- Przerwa we własności lokalu.
- Indywidualne lub inne stawki niż pożądana.
- Ujemne zużycia.
- Odczyty na złe daty.
- Brak rozliczenia.

Aby uzyskać zestawienie, należy przejść do:

- Zakładka `Administracja`.
- Pole `Struktura` > kliknąć całą nieruchomość lub inną podrzędną strukturę.
- Przycisk `Naliczenia`.
- Wybrać `K.bieżąca`.
- Menu `Widok` > `Struktura naliczeń w lokalach` lub `Struktura naliczeń` przy wybraniu pojedynczego lokalu w polu `Struktura`.

![Sprawdzenie rozliczenia](sprrozliczenia2.gif)