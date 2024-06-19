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
- Pole `Algorytm` > tutaj wpisujemy sposób liczenia opłaty. **Pole jest opisane dokładniej w dalszej części instrukcji**.
- Pole `Algorytm licznikowy` > tutaj wpisujemy część licznikową algorytmu, jeśli opłata ma być powiązana z licznikami i rozliczana wg nich w przyszłości. Jeśli nie to pozostawiany ją pustą. **Pole jest opisane dokładniej w dalszej części instrukcji**.
- Kliknąć: `Dodaj`.
- Kliknąć: `Zatwierdź`.

Poniżej przykład dodania algorytmu utrzymania czystości od powierzchni.

![Dodanie algorytmu do budynku](algorrozsze.gif)

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

Jest to typowa struktura instrukcji (if/elseif/else). Możliwe jest pominięcie `AGDY` i `INACZEJ`, można też stosować wiele `AGDY`. System analizuje algorytm od lewej do prawej, z góry do dołu. Jeśli `[warunek]` jest prawdą, to system wykona `[instrukcję]` po słowie `WTEDY`, jeśli nie, to przejdzie do następnej linijki algorytmu. Wyjątkiem jest `INACZEJ` które zawsze stawiamy jako ostatnie, jest to alternatywa do warunków poprzedzających, w przypadku ich niespełnienia. Każdą funkcję zawsze zaczynamy, od `GDY` a kończymy `KGDY`. Wielkość liter i spacje są bez znaczenia. Jako `[instrukcję]` możemy użyć prostych działań na danych i stawkach opisanych wcześniej lub też zagnieździć kolejną instrukcję warunkową.

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

Najprostszy możliwy algorytm z wyborem:

    GDY Dx>0 WTEDY              Gdy np. powierzchnia jest większa od zera wtedy
        [instrukcja]            Nalicz opłatę wg działania (np. Sxxxx)
    KGDY                        Koniec

Za pomocą takiego algorytmu można zrealizować opłatę od lokalu. Radzimy nie stosować takich algorytmów, ponieważ nie zawierają one instrukcji w przypadku kiedy warunek nie zostanie spełniony, na przykład na brak opłaty lub korektę danej z warunku (nie naliczy się korekta). Prawidłowy algorytm przedstawiamy poniżej:

    GDY Dx>0 WTEDY              Gdy np. powierzchnia jest większa od zera wtedy
        [instrukcja]            Nalicz opłatę wg działania (np. Sxxxx)
    INACZEJ                     Jeśli warunek nie został spełniony wokonaj
        [instrukcja]            W tej instukcji możemy podać alternatywę, np. brak opłaty wpisać S9999 (stawkę zero)
    KGDY                        Koniec

Algorytm z wielokrotnymi warunkami. Dobrym przykładem jest tutaj algorytm dla naliczeń za odpady dla Warszawy, który obowiązywał od 2013-07-01 do 2020-03-01. Opłata uzależniona jest od ilości osób w lokalu, nie jest wielokrotnością jednej stawki oraz ma górny limit kwoty. 

    GDY D21<1 WTEDY             Sprawdzamy czy liczba osób w lokalu jest mniejsz od jeden
        S9999                   Jeśli tak to stosujemy stawkę zero, brak opłaty.
    AGDY D21<2 WTEDY            Jeśli liczba osób jest mniejsza od 2
        S1301                   To sotosujemy stawkę za jedną osobę
    AGDY D21<3 WTEDY            Jeśli liczba osób jest mniejsza od 3
        S1302                   To sotosujemy stawkę za dwie osoby
    AGDY D21<4 WTEDY            Jeśli liczba osób jest mniejsza od 4
        S1303                   To sotosujemy stawkę za trzy osoby
    INACZEJ                     W innych przypadkach czyli równe lub więcej niż 4
        S1304                   To sotosujemy stawkę maksymalną, za cztery osoby
    KGDY                        Koniec

System sprawdza kolejno, od góry, warunki podane: `GDY` > `AGDY` > `AGDY` > itd. Gdy któryś z nich zostanie spełniony jako pierwszy, to opłata przyjmie wartość z działania określonego po `WTEDY` dla tego warunku, reszta zostanie niesprawdzona/pominięta. Należy to mieć na uwadze przy konstruowaniu prawidłowego algorytmu.

Algorytmy zagnieżdżone. Przykładem tutaj może być algorytm dla naliczeń za odpady dla Wrocławia. Jako pierwsze sprawdzamy w nim czy lokal jest zamieszkały, a następnie sprawdzamy powierzchnię przypadającą na jednego mieszkańca i w zależności od niej wybieramy odpowiedni sposób naliczania opłaty.

    GDY D21>0 WTEDY             Sprawdzamy czy liczba osób większa od zera
        GDY D1/D21 =< 27 WTEDY      Sprawdzamy czy na osobę przypada mniej niż 27m2 wtedy
            D1 * S1302              Stosujemy opłatę od powierzchi lokalu
        INACZEJ                     Gdy jest inna wtedy
            D21 * S1303             Stosujemy opłatę od osoby.
        KGDY                        Koniec
    INACZEJ                     Gdy liczba osób jest równa zero wtedy
        S9999                   Stosujemy stawkę zero, brak opłaty
    KGDY                        Koniec