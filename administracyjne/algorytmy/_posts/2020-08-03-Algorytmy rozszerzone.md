---
title: Algorytmy rozszerzone
---

# Algorytmy rozszerzone

System pozwala na wprowadzenie bardziej zaawansowanego sposobu (algorytmu) liczenia opłat lub rozliczeń. Wprowadzamy go tym samym oknem co zwykłe algorytmy:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj algorytmy`.
- Pole `Lokal` > wybrać cały budynek, algorytmy dodajemy zazwyczaj na cały budynek.
- Pole `Algorytm` > wybrać nazwę opłaty, algorytmu.
- Pole `Data` > wprowadzić datę, od kiedy ma obowiązywać opłata.
- Pole `Sposób wpr. alg.` > `Rozszerzony`.
- Pole `Algorytm` > tutaj wpisujemy sposób liczenia opłaty. Jest to opisane w dalszej części instrukcji.
- Pole `Algorytm licznikowy` > tutaj wpisujemy część licznikową algorytmu, jeśli opłata ma być powiązana z licznikami i rozliczana wg nich w przyszłości. Jeśli nie to pozostawiany ją pustą.
- Kliknąć: `Dodaj`.
- Kliknąć: `Zatwierdź`.

#### Operatory i oznaczenia

Poniżej przedstawiamy operatory i oznaczenia używane w działaniach algorytmów.

- `Dx` > literka D a zaraz po niej wpisujemy ID danej. W ten sposób wskazujemy daną w działaniu (np. o indeksie/numerze 21 - D21 „Liczba osób”). ID danych można sprawdzić w menu `Zasoby` > `Edytuj dane`.
- `Sxxxx` > literka S a zaraz po niej wpisujemy ID stawki. W ten sposób wskazujemy stawkę w działaniu (np. o indeksie/numerze 2001 - S2001 „Eksploatacja”). ID stawek można sprawdzić w menu `Zasoby` > `Edytuj stawki`.
- `Lx` > literka L a zaraz po niej wpisujemy ID licznika. W ten sposób wskazujemy licznik w działaniu (np. typu pierwszego - L1, zazwyczaj ZW). ID liczników można sprawdzić w menu `Elementy` > `Typy liczników`.
- `+` > znak plus oznacza dodawanie.
- `*` > znak gwiazdka oznacza mnożenie.
- `-` > znak minus oznacza odejmowanie.
- `/` > znak ukośnika oznacza dzielenie.
- `() `> nawiasy, służące grupowaniu i zmianie kolejności wykonywania działań.
- W działaniu można również wpisać konkretną liczbę za pomocą klawiatury numerycznej (np. 123).

#### Pole Algorytm

W tym polu wpisujemy działanie, za pomocą którego system będzie liczył opłatę. Sposób podany tutaj musi się zawsze sprowadzać do prostego iloczynu:

    Ilosć * stawka

Pole może pozostać puste, wtedy wymagane jest uzupełnienie pola `Algorytm licznikowy`. Poniżej przykłady działań możliwych do wpisania (pod małe litery trzeba podstawić ID danej lub stawki):

- `Dx * Syyyy` > proste możenie danej przez stawkę.
- `(Dx + Dz + Dq) * Syyyy` > mnożenie sumy danych przez stawkę. Można też stosować odejmowanie.
- `Dx * Szzzz * Syyyy` > w działaniu można też użyć drugiej stawki np. pełniącej funkcję współczynnika lub danej sterującej naliczeniem, przyjmującej wartość 0 (brak) lub 1 (nalicz). Drugą daną może być też norma na osobę lub lokal. Stawką, która pokaże się na wydruku, będzie stawka z lewej strony działania.
- `Syyyy` > naliczenie z samej stawki. Sugerujemy nie stosować takiego sposobu, ponieważ podczas wykupów wstecz korekta dla takiego algorytmu nie będzie się naliczała automatycznie. Opłata naliczy się od każdego lokalu, który posiada stawkę (ilość będzie równa 1). Dopuszczalne jest stosowanie tego sposobu dla naliczeń pożytków.

W działaniach w polu `Algorytm` nie można stosować liczników.

#### Pole Algorytm licznikowy

W tym polu wpisujemy działanie, dla opłat skojarzonych z licznikami. Działanie wpisane w tym polu ma pierwszeństwo nad działaniem z pola `Algorytm` a dokładniej, jeśli licznik użyty w działaniu ma dodaną prognozę, to opłata naliczy się z prognoz (przy naliczaniu zaliczek). W przypadku braku prognozy na liczniku, działanie w tym polu jest pomijane, ewentualna zaliczka będzie naliczana wg działania z pola `Algorytm`. Pole `Algorytm licznikowy` odpowiada też za rozliczenia liczników danej opłaty. Wcześniej naliczone zaliczki, w momencie przeliczania rozliczenia liczników, zostaną porównane do kwoty z działania określonego w tym polu. Pole może pozostać puste, wtedy wymagane jest uzupełnienie pola `Algorytm`. Poniżej przykłady działań możliwych do wpisania (pod małe litery trzeba podstawić ID typu licznika lub stawki/danej):

- `Lx * Syyyy` > proste możenie prognozy (zużycia) licznika przez stawkę.
- `(Lx + Lz) * Syyyy` > mnożenie sumy prognoz (zużyć) liczników przez stawkę. Można też stosować odejmowanie, w ten sposób można odpowiednio uwzględnić liczniki ogrodowe lub cyrkulacji.
- `Lx * Szzzz * Syyyy` > uwzględnienie w działaniu współczynnika wpisanego w stawce (może być też dana).

Przykłady z programu (ID mogą być inne):

- `L3 * S1100` > część licznikowa zazwyczaj stosowana w opłacie CO zm: Licznik CO * stawka za GJ.
- `L2 * S1150` > część licznikowa zazwyczaj stosowana w opłacie Podgrzew wody: Licznik CW * stawka za m3 podgrzewu wody.
- `(L1+L2) * S1200` > część licznikowa zazwyczaj stosowana w opłacie Zimna woda i ścieki: Licznik ZW+CW * stawka za m3 ZWiŚ.

#### Warunki w algorytmach

W algorytmach rozszerzonych możemy stosować warunki w naliczeniu opłat. Dzięki temu możemy opłatę uzależnić od wartości danej w sposób nieliniowy. Na przykład spowodować, aby opłata naliczyła się dopiero po przekroczeniu pewnej wartości lub naliczyć ją w pewnym jej przedziale. Można też zastosować różne sposoby naliczania, nazywamy to wyborem na przykład: Jeśli warunek jest spełniony, nalicz wg sposobu pierwszego, w innych przypadkach nalicz opłatę wg sposobu drugiego. Składnia instrukcji warunkowej:

    GDY [warunek] WTEDY
    [instrukcja]
    AGDY [warunek] WTEDY
    [instrukcja]
    INACZEJ
    [instrukcja]
    KGDY

Jest to typowa struktura instrukcji (if/elseif/else). Możliwe jest pominięcie `AGDY` i `INACZEJ`, można też stosować wiele `AGDY`. System analizuje funkcję od lewej do prawej, z góry do dołu. Jeśli `[warunek]` jest prawdą, to system wykona `[instrukcję]` po słowie `WTEDY`, jeśli nie, to przejdzie do następnej linijki algorytmu. Wyjątkiem jest `INACZEJ` które zawsze stawiamy jako ostatnie, jest to alternatywa do warunków poprzedzających, w przypadku ich niespełnienia. Każdą funkcję zawsze zaczynamy, od `GDY` a kończymy `KGDY`. Wielkość liter i spacje są bez znaczenia. Jako `[instrukcję]` możemy użyć prostych działań na danych i stawkach opisanych wcześniej lub też zagnieździć kolejną instrukcję warunkową.

Operatory logiczne używane w warunkach:

- `LUB` > spójnik logiczny alternatywy (logiczne OR). Przykład warunku:

    GDY `D21>0 LUB D31>3` WTEDY `[instrukcja]` KGDY

- `ORAZ` > spójnik logiczny alternatywy (logiczne AND). Przykład warunku:

    GDY `D1>0 ORAZ D100>3` WTEDY `[instrukcja]` KGDY

- `NIE` > logiczna negacja (odwrócenie wartości logicznej). Przykład warunku:

    GDY `NIE D3=2` WTEDY `[instrukcja]` KGDY

- `$` > symbol dolara, postawiony przed oznaczeniem danej lub stawki oznacza sprawdzenie, czy istnieje/jest zdefiniowana — jeżeli tak, to zwraca wartość prawda w przeciwnym przypadku fałsz. Odradzamy stosowanie tego operatora, w algorytmie lepiej użyć: `Sxxxx > 0`.  Przykład warunku:

    GDY `$Sxxxx` WTEDY `[instrukcja]` KGDY

- `TYP` > operator sprawdzający typ naliczenia: 1 - (R), 2 - (LR), 3 - (LP), 4 - (LZ), 5 - (RKR), 6 - (RKL). Używany tylko w polu `Algorytm licznikowy`. Przykład warunku (Opłata, która nalicza z prognoz liczników, ale nie podlega rozliczeniu liczników):

    GDY `TYP < 4` WTEDY `(L1+L2)*S1200` KGDY

Operatory relacji:

- `<` > mniejszy. Przykład warunku: `D1<100`.
- `<=` > mniejszy-równy. Przykład warunku:  `D1<=100`.
- `=` > równy. Przykład warunku: `D1=100`.
- `>=` > większy równy. Przykład warunku: `D1>=100`.
- `>` > większy. Przykład warunku: `D1>100`.
- `<>` > nie równa się. Przykład warunku: `D1<>100`.

#### Przykładowe algorytmy

Wywóz nieczystości — Wrocław


    GDY $S1301 WTEDY
        S1301
    INACZEJ
        GDY D21>0 WTEDY
            GDY D1/D21 =< 27 WTEDY
            D1 * S1302
            INACZEJ
            D21 * S1303
            KGDY
        INACZEJ
        S9999
        KGDY
    KGDY


- D1 - Dana o indeksie/numerze 1, czyli np. Powierzchnia użytkowa.
- D21 - Dana o indeksie/numerze 21, czyli np. Liczba osób.
- S1301 - Stawka o indeksie/numerze 1301, czyli np. Śmieci LU (używana do indywidualnych obciążeń w lokalu — stawka indywidualna).
- S1302 - Stawka o indeksie/numerze 1302, czyli np. Śmieci [m2] (obciążenie od m2 powierzchni).
- S1303 - Stawka o indeksie/numerze 1303, czyli np. Śmieci [os.] (obciążenie od ilości osób).
- S9999 - stawka zero.

Założenie/opis do algorytmu jest taki:

Jeżeli istnieje stawka S1301, wtedy obciążamy lokal stawką S1301. Jeśli nie ma zdefiniowanej stawki S1301, to rozpatrujemy kolejną (wewnętrzną) instrukcję warunkową i wtedy (inaczej): jeżeli Liczba osób jest większa niż 0 (zabezpieczenie przed dzieleniem przez zero, w przypadku gdy liczba osób faktycznie wynosi zero) to wtedy dzielimy powierzchnię użytkową (D1) przez liczbę osób (D21) - jeśli wynik tej operacji jest mniejszy bądź równy 27, to wynik będzie mnożeniem powierzchni użytkowej (D1) przez stawkę S1302, w innym przypadku wynik będzie mnożeniem liczby osób (D21) przez stawkę S1303.

