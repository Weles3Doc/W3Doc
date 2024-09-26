---
title: 2. Ustawienie rozliczenia kosztów
---

# Ustawienie sposobu rozliczenia kosztów

Po zdefiniowaniu terminów rozliczeń można przejść do ustawienia rozliczenia kosztów. Aby określić sposób rozliczenia kosztów, należy:

- Zakładka `Administracja` > przycisk `Naliczenia`.
- Na liście miesięcy zaznaczamy `K. bieżąca`.
- Menu `Obciążenia` > `Rozliczenia kosztów`.
- Pole `Rozliczany składnik` > wybieramy pozycję do rozliczenia.
- Pole `Element struktury` > w tym polu zazwyczaj wskazujemy całą nieruchomość, najwyższy element struktury w zakładce `Administracja`. Wtedy gdy rozliczana kwota dotyczy wszystkich podległych lokali i nie istnieją inne obostrzenia. Można też wskazać podległą strukturę, wtedy rozliczenie zajdzie tylko dla lokali pod tą strukturą. Stosujemy to, gdy chcemy obciążyć tylko daną grupę właścicieli lub zróżnicować sposoby i kwoty rozliczeń pomiędzy strukturami. W polu można też wskazać pojedynczego właściciela, wtedy rozliczenie i kwota będzie dotyczyło tylko jego.
- Pole `Typ` > w tym polu wybieramy typ rozliczenia:
    - `Algorytm - pełny koszt` > jako `Wartość` wprowadzamy całość poniesionych kosztów, zostanie ona rozliczona wg wprowadzonego dalej algorytmu.
    - `Algorytm - różnica` > jako `Wartość` wprowadzamy różnicę między poniesionymi kosztami a przychodami z tytułu należności, zostanie ona rozliczona wg wprowadzonego dalej algorytmu.
    - `Obciążenia - pełny koszt` > jako `Wartość` wprowadzamy całość poniesionych kosztów, zostanie ona rozliczona proporcjonalnie do wcześniejszych obciążeń z wybranej należności. (zaliczek + korekt + RL + RK, w zależności co występuje)
    - `Obciążenia - różnica` > jako `Wartość` wprowadzamy różnicę między poniesionymi kosztami a przychodami, zostanie ona rozliczona proporcjonalnie do wcześniejszych obciążeń z wybranej należności. (zaliczek + korekt + RL + RK, w zależności co występuje)
    - `Obciążenia z wagą - pełny koszt` > rozliczenie wg wcześniejszych obciążeń jak wyżej, z możliwością określenia tzw. wagi, czyli dodatkowego współczynnika wpływającego na udział w rozliczeniu.
    - `Obciążenia z wagą - różnica` > rozliczenie wg wcześniejszych obciążeń jak wyżej, z możliwością określenia tzw. wagi, czyli dodatkowego współczynnika wpływającego na udział w rozliczeniu.
- Pole `Sposób` > pole istotne tylko w przypadku pozycji skojarzonych z licznikami, określamy tutaj czy rozliczenie zostanie przeprowadzone:
    - `Łącznie` > razem dla lokali z licznikami i ryczałtowych.
    - `Ryczałt` > tylko dla lokali ryczałtowych, bez licznika.
    - `Licznik` > tylko dla lokali posiadających licznik.
    - `Licznik + ryczałt` > oddzielnie dla lokali z licznikami i ryczałtowych pojawi się możliwość wprowadzenia dwóch wartości, dla obu sposobów oddzielnie.
- Pole `Sposób wpr. alg` > wybór tutaj ma wpływ na następne pole, jeśli wybierzemy:
    - `Zwykły` > to w polu `Algorytm` dane wg, których będzie liczony udział w RK, będzie można wybrać za pomocą specjalnej formatki.
    - `Rozszerzony` > to w polu `Algorytm` dane wg, których będzie liczony udział w RK, będzie można wpisać z klawiatury.
- Pole `Algorytm` > wybieramy lub wpisujemy tutaj dane, lub działanie na danych wg. których zostanie wyliczony udział w RK.
- Pole `Wartość` > podajemy kwotę do rozliczenia (z uwzględnieniem pola `Typ`), zazwyczaj sprawdzamy ją z wydrukami oraz stanem kont, może być to też dowolna kwota.
- Pole `Typ VAT` > ustawiamy typ VAT rozliczanej kwoty. Zazwyczaj stosujemy `Brutto`, gdy rozliczenie jest bez VAT. W przypadku wspólnot Vatowych decydujemy, czy kwotę traktujemy jako Netto, Brutto, ZW lub NP.
- Pole `Wydruk` > ustawiamy pokazywanie pozycji, dla których wynik rozliczenia jest równy zero.
    - `Drukuj tylko niezerowe` > pozycje zerowe nie będą pokazywane.
    - `Drukuj wszystkie` > będą pokazywane wszystkie.
- Kliknąć: `Dodaj`.
- Wprowadzić inne pozycje, jeśli trzeba.
- Kliknąć: `Zatwierdź`.

Nie można ustawić rozliczenia kosztów i liczników **na raz** dla tego samego składnika. Składnikom opłat, które są poprzedzone rozliczeniem liczników, ustawiamy rozliczenie różnicy, nie — pełen koszt. Rozliczenie wg obciążeń robimy tylko wtedy gdy dla danego składnika są zaksięgowane wcześniejsze zaliczki lub korekty, lub inne rozliczenia. Jeśli ich nie będzie, to system zgłosi błąd zerowej podstawy rozliczenia. W systemie można robić korekty do rozliczeń kosztów, polega to na zrobieniu jeszcze raz rozliczenia za ten sam okres z nowym sposobem rozliczenia lub kwotą. Za pozycje, które są rozliczone w systemowych rozliczeniach kosztów, nie można robić korekt. Zazwyczaj dla jednego składnika opłat, na jednej tej samej strukturze, nie dodajemy dwóch lub więcej sposobów rozliczeń, w takich przypadkach system zgłosi błąd. Możliwe jest dodanie takich sposobów, ale muszą się one nawzajem wykluczać na każdym z lokali. W polu `Algorytm` należy zawsze wybrać jakąś daną lub wpisać działanie na danych, lub algorytm, nie może pozostać puste.

![Ustawienie rozliczenia kosztów](ustawienierozliczeniakosztow.gif)