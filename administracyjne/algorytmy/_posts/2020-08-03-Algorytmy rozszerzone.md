---
title: Algorytmy rozszerzone
---

# Algorytmy rozszerzone

Poniżej znajduje się szczegółowy opis dostępnych funkcji oraz operatorów przy wprowadzaniu algorytmu w wersji rozszerzonej.

- Z drzewa struktury wybieramy budynek i przechodzimy do zakładki Administracja.

![Algorytmy rozszerzone](algorozsz1.png)

- Z dostępnego menu Zasoby, wybieramy Edytuj algorytmy. Po chwili system wyświetli nowe okno dialogowe.

![Algorytmy rozszerzone](algorozsz2.png)

- Algorytm najlepiej jest zakładać Globalnie, czyli jeden na całą nieruchomość (lub ew. na strukturach grupujących — unikamy wprowadzania algorytmów indywidualnie, na mieszkaniach). W polu Lokal wskazujemy zatem najwyższy element struktury.

![Algorytmy rozszerzone](algorozsz3.png)

- W polu Algorytm wskazujemy który algorytm chcemy dodać (w przypadku kilku tych samych nazw należy patrzeć na Indeksy — ID algorytmu).

![Algorytmy rozszerzone](algorozsz4.png)

- W polu Data, określamy datę, od kiedy ma obowiązywać nasz algorytm.

![Algorytmy rozszerzone](algorozsz5.png)

- W polu Sposób wpr. alg. określamy czy chcemy wprowadzić algorytm w sposób Zwykły (dotychczasowy — wybierać dane, stawki, liczniki itp.), czy też Rozszerzony (zaawansowany — nowa funkcjonalność). Skupimy się tutaj na algorytmie rozszerzonym.

![Algorytmy rozszerzone](algorozsz6.png)

- Przechodzimy do pola Algorytm. Jak widać, jest ono nieco większe. W polu można wpisać odpowiedni algorytm, stosując odpowiednie i operatory lub po prostu go wkleić (Ctrl + C/V) z innej nieruchomości, schowka czy pliku tekstowego.  Struktura funkcji oraz operatorów jest opisana w dalszej części tego dokumentu.

![Algorytmy rozszerzone](algorozsz7.png)

- Wprowadzamy nasz algorytm. Założenie jest takie: pomnóż (operator gwiazdki - *) liczbę osób (dana Liczba osób ma indeks o numerze 205, więc wpisujemy D205) przez Stawkę za śmieci, ale z podziałem (instrukcja warunkowa — GDY), jeżeli liczba osób będzie mniejsza lub równa 2 to pomnóż przez stawkę o indeksie 1311 (S1311), w innym wypadku (INACZEJ) pomnóż przez stawkę o indeksie 1312 (S1312).

![Algorytmy rozszerzone](algorozsz8.png)

- W polu Algorytm licznikowy (jeżeli nie ma takiej potrzeby) nie wprowadzamy nic. Pole nie jest obowiązkowe (chyba że chcemy mieć naliczenia/rozliczenia związane z zużyciem liczników — np. przy ZW, CW, czy CO) i w tym przykładzie pozostawiamy je puste.

![Algorytmy rozszerzone](algorozsz9.png)

- Klikamy: Dodaj.

![Algorytmy rozszerzone](algorozsz10.png)

- Całość zatwierdzamy hasłem.

![Algorytmy rozszerzone](algorozsz11.png)

- Pozostaje jeszcze dodać odpowiednie stawki (jeżeli nie zostało to zrobione dotychczas), tj z menu Zasoby, wybieramy Edytuj stawki. (jeśli stawki są już określone, to pomijamy punkty 12 i 13)

![Algorytmy rozszerzone](algorozsz12.png)

- Odszukujemy interesujące nasz stawki oraz określamy ich wartość.

![Algorytmy rozszerzone](algorozsz13.png)

- Możemy teraz sprawdzić nasze naliczenie. Po przeliczeniu zaliczek widać, że system wyświetlił dwie pozycje dla naszego algorytmu — stawka 10 zł i 7 zł.

![Algorytmy rozszerzone](algorozsz14.png)

- Po wybraniu konkretnego lokalu widać, że algorytm liczy poprawnie (dla liczby osób = 4, system przyjął stawkę S1312).

![Algorytmy rozszerzone](algorozsz15.png)

### Instrukcja warunkowa

    GDY [warunek] WTEDY
        [wartość/instrukcja] 
    AGDY [warunek] WTEDY
        [wartość/instrukcja]
    INACZEJ
        [wartość/instrukcja] 
    KGDY

Jest to typowa struktura instrukcji warunkowej (if/else).

Operatory i oznaczenia:

- GDY WTEDY AGDY INACZEJ KGDY — to elementy typowej instrukcji warunkowej (jeśli/jeżeli). Funkcja zawsze zaczyna się, od GDY a kończy na KGDY. Dopuszczalne jest pominięcie części struktury, np. algorytm może wyglądać tak: GDY [warunek] WTEDY [wartość/instrukcja] INACZEJ [wartość/instrukcja] KGDY lub GDY [warunek] WTEDY [wartość/instrukcja] KGDY.
- / * + - — gwiazdka, ukośnik, plus i minus, operatory prostych działań arytmetycznych.
- () — nawiasy, służące grupowaniu i zmianie kolejności wykonywania działań
- LUB ORAZ — spójniki logiczne alternatywy i koniunkcji (logiczne lub i logiczne i)
- NIE — logiczne zaprzeczenie (odwrócenie wartości logicznej)
- < <= = >= > <> — operatory porządkujące (mniejszy, mniejszy-równy, równy, większy równy, większy, przedział), wskazujemy konkretną liczbę lub przedział
- $ — symbol dolara postawiony przed oznaczeniem danej lub stawki oznacza sprawdzenie, czy istnieje/jest ona zdefiniowana — jeżeli tak, to zwraca wartość “prawda” w przeciwnym przypadku fałsz.
- DXXX, SXXX, LXXX — wskazujemy Daną (np. o indeksie/numerze 21 - D21), Stawkę (np o indeksie/numerze 2001 - S2001) lub Licznik (np. typu pierwszego - L1). Możemy również wpisać konkretną liczbę za pomocą klawiatury numerycznej (np. 123).
- TYP — to typ naliczenia: 1 - (R), 2 - (LR), 3 - (LP), 4 - (LZ), 5 - (RKR), 6 - (RKL)

### Przykładowe algorytmy

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

