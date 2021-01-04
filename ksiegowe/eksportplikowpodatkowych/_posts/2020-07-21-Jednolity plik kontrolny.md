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
- Pole `Rachunek bankowy` > w przypadku JPK_WB wybieramy konto księgowe rachunku bankowego, dla którego chcemy wygenerować zestawienie operacji w pliku.
- Pole `Korekta` > wskazujemy czy plik będzie pierwszym złożeniem, czy korektą.
- Pole `Przyczyna korekty` > opis przyczyny korekty.
- Pole `Nadwyżka z poprzedniego okresu` > podajemy kwotę, która zostanie podana w segmencie `D1.1 Przeniesienia` deklaracji.
- Pole `Pozycje NP` > ustawiamy czy system ma ujmować pozycje, które w systemie zostały naliczone z typem stawki: `NP VAT (FV)`.
- Pole `Weryfikacja schematu` > ustawiamy czy system ma sprawdzać plik pod względem zgodności z definicjami struktur dostarczanymi przez Ministerstwo Finansów — jeżeli wystąpi niezgodność, plik się nie pobierze i zostanie wyświetlony komunikat o błędzie.
- Pole `Akcja` > wybieramy czy chcemy pobrać plik xml lub podejrzeć jego zawartość w nowym oknie.
- Kliknąć: `Pobierz`.

Cały proces generowania pliku przedstawiamy na poniższym filmie.

![JPK](jpkeksport.gif)