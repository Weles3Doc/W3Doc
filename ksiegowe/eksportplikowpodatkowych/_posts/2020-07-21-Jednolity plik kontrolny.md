---
title: Jednolity Plik Kontrolny
---

# Jednolity Plik Kontrolny

Jednolity Plik Kontrolny jest zbiorem danych, tworzonym z systemów informatycznych podmiotu, zawierającym informacje o operacjach gospodarczych za dany okres, posiadającym u standaryzowany układ i format (XML) umożliwiający jego dalsze przetwarzanie.

Przed przystąpieniem do eksportu JPK należy:

- Uzupełnić dane podatkowe podmiotu.
- Każdemu dostawcy i odbiorcy uzupełnić NIP w systemie, bez tego JPK nie przejdzie weryfikacji (program zgłosi błąd).

Aby wygenerować plik JPK, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Podatki`.
- Zakładka `Eksport`.
- Pole `Zasób` > wybieramy nieruchomość.
- Pole `Formularz` > wybieramy jedną z odstępnych wersji JPK. Dalsze pola będą zależały od wyboru formularza.
- Pole `Data od` > wskazujemy miesiąc początkowy.
- Pole `Data do` > wskazujemy miesiąc końcowy.
- Pole `Zakres sprzedaż` > określamy wg jakiej daty będą brane pozycje VAT-owe do ewidencji podatku należnego.
- Pole `Zakres zakup` > określamy wg jakiej daty będą brane pozycje VAT-owe do ewidencji podatku naliczonego.
- Pole `Cel złożenia` > wpisujemy numer odpowiadający celowi złożenia.
- Pole `Zaokrąglenia liczb ujemnych` > wybrać jedno z:
    - `Od zera (właściwe)`.
    - `W górę (wsteczna zgodność)`.
- Pole `Rachunek bankowy` > w przypadku JPK_WB wybieramy konto księgowe rachunku bankowego, dla którego chcemy wygenerować zestawienie operacji w pliku.
- Pole `Korekta` > wskazujemy czy plik będzie pierwszym złożeniem, czy korektą.
- Pole `Przyczyna korekty` > opis przyczyny korekty.
- Pole `Nadwyżka z poprzedniego okresu` > podajemy kwotę, która zostanie podana w segmencie `D1.1 Przeniesienia` deklaracji.
- Pole `Pozycje NP` > ustawiamy czy system ma ujmować pozycje, które w systemie zostały naliczone z typem stawki: `NP VAT (FV)`.
- Pole `Weryfikacja schematu` > ustawiamy czy system ma sprawdzać plik pod względem zgodności z definicjami struktur dostarczanymi przez Ministerstwo Finansów — jeżeli wystąpi niezgodność, plik się nie pobierze i zostanie wyświetlony komunikat o błędzie.
- Pole `Akcja` > wybieramy:
    - `Pobranie` > pobierzemy plik xml.
    - `Podgląd` > otworzymy podgląd deklaracji w przeglądarce.
- Pole `Zwrot na rachunek` > ustawiamy zwrot nadpłaconego podatku:
    - Pole `Kwota zwrotu` > wpisujemy kwotę.
    - Pole `Opcje zwrotu` > wybieramy jedną opcje z listy:
        - `Zwrot na rachunek rozliczeniowy podatnika w terminie 15 dni`.
        - `Zwrot na rachunek VAT podatnika w terminie 25 dni`.
        - `Zwrot na rachunek rozliczeniowy podatnika w terminie 25 dni (art. 87 ust. 6 ustawy)`.
        - `Zwrot na rachunek rozliczeniowy podatnika w terminie 40 dni`.
        - `Zwrot na rachunek rozliczeniowy podatnika w terminie 60 dni`.
        - `Zwrot na rachunek rozliczeniowy podatnika w terminie 180 dni`.
- Pole `Przyszłe zobowiązania podatkowe` > ustawiamy czy nadpłatę podatku przeznaczamy na przyszłe podatki:
    - Pole `Kwota zobowiązania` > wpisujemy kwotę.
    - Pole `Nazwa zobowiązania` > wpisujemy na jaki cel przeznaczamy nadpłatę.
- Kliknąć: `Pobierz`.

Cały proces generowania pliku przedstawiamy na poniższym filmie.

![JPK](jpkeksport.gif)