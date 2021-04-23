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
- `Syyyy` > naliczenie z samej stawki. Sugerujemy nie stosować takiego sposobu. Opłata naliczy się od każdego lokalu, który posiada stawkę (ilość będzie równa 1). Dopuszczalne jest stosowanie tego sposobu dla naliczeń pożytków.


#### Warunki w algorytmach

- GDY WTEDY AGDY INACZEJ KGDY — to elementy typowej instrukcji warunkowej (jeśli/jeżeli). Funkcja zawsze zaczyna się, od GDY a kończy na KGDY. Dopuszczalne jest pominięcie części struktury, np. algorytm może wyglądać tak: GDY [warunek] WTEDY [wartość/instrukcja] INACZEJ [wartość/instrukcja] KGDY lub GDY [warunek] WTEDY [wartość/instrukcja] KGDY.

- LUB ORAZ — spójniki logiczne alternatywy i koniunkcji (logiczne lub i logiczne i)

- NIE — logiczne zaprzeczenie (odwrócenie wartości logicznej)

- < <= = >= > <> — operatory porządkujące (mniejszy, mniejszy-równy, równy, większy równy, większy, przedział), wskazujemy konkretną liczbę lub przedział

- $ — symbol dolara postawiony przed oznaczeniem danej lub stawki oznacza sprawdzenie, czy istnieje/jest ona zdefiniowana — jeżeli tak, to zwraca wartość “prawda” w przeciwnym przypadku fałsz.

- TYP — to typ naliczenia: 1 - (R), 2 - (LR), 3 - (LP), 4 - (LZ), 5 - (RKR), 6 - (RKL)


GDY [warunek] WTEDY
    [wartość/instrukcja] 
AGDY [warunek] WTEDY
    [wartość/instrukcja]
INACZEJ
    [wartość/instrukcja] 
KGDY

Jest to typowa struktura instrukcji warunkowej (if/else).



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

