---
title: Płatności on-line - uruchomienie
---

# Płatności on-line - uruchomienie

Aby uruchomić płatności przez podgląd właściciela, należy w pierwszej kolejności wykonać kilka czynności. Prosimy też zapoznać się z regulaminem usługi dostępnym [>TUTAJ<](https://docs.google.com/document/d/1PemdnnfQCmwqsxqHocUK33E_WHUoHukVCt7pBFn85fE/).

Płatności on-line są bezpieczne i darmowe dla Państwa - zachęcamy do uruchomienia.

Za płatność właściciela, zyskują Państwo `rabat` 0,10 zł/netto/miesiąc, który obniża Państwa abonament za Weles 3.

Im więcej właścicieli korzysta z płatności on-line przez `tomojdom.pl` tym tańszy staje się system dla Państwa. Zachęcamy do poinformowania właścicieli lokali o takiej możliwości.

Przelewy przychodzące do wspólnot są w zasadzie natychmiastowe, a tytuł przelewu jest jednoznaczny, od razu wiadomo której kartoteki właściciela dotyczy (przykład: `W3DP-XXXXX WIATRACZNA 1 201-1-0000001-1 Rozrachunki`).

W imporcie operacji bankowych wpłaty on-line są od razu przypisywane do właściwego odbiorcy.

#### Uprawnienia

Pierwszą ważną czynnością jest nadanie uprawnień do ustawiania płatności przez kartotekę internetową. Uprawnienia sugerujemy nadawać jednej lub dwóm osobom, które będą odpowiedzialne za dodawanie kont i dbanie o ich poprawność. Ma to krytyczne znaczenie dla bezpieczeństwa płatności właścicieli. Aby nadać uprawnienia, przechodzimy do:

- Zakładka `Zasoby` > menu `Funkcje` > `Administratorzy`.
- Z listy użytkowników wybieramy administratora.
- Klikamy: `Edycja`.
- Pole `Administratorzy` > pomijamy.
- Pole `Końcówka` > pomijamy.
- Pole `Hasło` > pomijamy.
- Pole `Uprawnienia` > zaznaczamy pozycję `Płatności`.
- Klikamy: `Zapisz`.

Gdy dany użytkownik widzi w systemie: Zakładka `Zasoby` > menu `Funkcje` > `Płatności przez podgląd właściciela`, oznacza to że ma już nadane uprawnienia i ten punkt można pominąć.

#### Dodanie NIP-u wspólnoty

Do uruchomienia płatności, konieczne jest dodanie NIP-u wspólnoty, aby to zrobić, należy przejść do:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj zasoby`.
- Z listy budynków wybieramy wspólnotę.
- Klikamy: `Edycja`.
- Pole `Wspólnota` > pomijamy.
- Pole `Adres` > pomijamy.
- Pole `Miejscowość` > pomijamy.
- Pole `NIP` > uzupełniamy NIP-em wspólnoty.
- Pole `Informacje` > pomijamy.
- Pole `Data` > pomijamy.
- Pole `Opcje` > pomijamy.
- Klikamy: `Zapisz`.

Jeśli NIP jest już dodany, to sprawdzamy jego poprawność, następnie zmiany opisywane w tym punkcie można pominąć.

#### Dodanie numerów kont bankowych

Jako następne trzeba określić numery kont wspólnoty, w tym celu przechodzimy do:

- Zakładka `Administracja` > menu `Elementy` > `Konta bankowe`.
- Pole `Podkonto` > wybieramy podkonto właściciela.
- Pole `Konto bankowe` > wpisujemy numer konta do wpłat.
- Klikamy: `Dodaj`.
- Jeśli trzeba, to uzupełniamy numery pozostałych kont do wpłat.
- Klikamy: `Zatwierdź`.

W przypadku gdy numery są już dodane, weryfikujemy ich poprawność.

#### Sprawdzenie ustawień i akceptacja regulaminu.

Ostatecznie uruchamiamy płatności on-line. Aby to zrobić, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Płatności przez podgląd właściciela`.
- Z listy budynków wybieramy wspólnotę.
- Klikamy: `Edycja`.
- Pole `Zasób` > powinno być uzupełnione, sprawdzamy je.
- Pole `NIP` > powinno być uzupełnione, sprawdzamy je.
- Pole `Adres` > powinno być puste, pole uzupełni się po kliknięciu `Zapisz`.
- Pole `Konta bankowe` > powinno być uzupełnione, sprawdzamy je, powinny się w nim **podpowiadać** konta z menu `Elementy` > `Konta bankowe` oraz struktury kont indywidualnych (części wspólne tych numerów).
- Pole `Dozwolone` > wpisujemy numer konta bankowego lub maskę kont płatności masowych:
  - Numer konta bankowego wpisujemy wtedy, gdy WM nie ma płatności masowych. Jeśli rachunki są dwa (lub więcej) to każdy wpisujemy w nowej linii.
  - Jeśli WM ma płatności masowe, to wpisujemy maskę kont wirtualnych, czyli stałą, niezmienną część rachunku wirtualnego. Sumę kontrolną zastępujemy znakiem podkreślenia `__`.

    >Przykład maski: `__102012341234___________`
    
    >Wpisujemy tylko: `__102012341234`
    
    Czyli bez końcowych podkreśleń. Jeśli maski są dwie (lub więcej) to każdą wpisujemy w nowej linii.
- Pole `Zgoda` > potwierdzają Państwo akceptację regulaminu.
- Klikamy: `Zapisz`.

Od tego momentu właściciele mają możliwość dokonywania wpłat na rachunek bankowy wspólnoty, przez kartotekę internetową za pomocą serwisu `Przelewy24` (PayPro S.A.). Jeśli płatności masowe są uruchomione na zasobie, to jego nazwa zostanie pogrubiona.

Poprawność uruchomienia mogą też Państwo sprawdzić logując się do podglądu właściciela: zakładka `Właściciele` > menu `Funkcje` > `Widok podglądu użytkownika`. Jeśli obok salda właściciela wyświetla sie przycisk `Zapłac teraz on-line` oznacza to że mają oni możliwość płacenia.

![Płatności](platnosci4.gif)