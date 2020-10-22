---
title: Eksport zapłat elektronicznych
---

# Eksport zapłat elektronicznych

Funkcja służy do generowania plików z poleceniem zapłaty np. za faktury kosztowe kontrahentów. Taki plik należy później zaimportować do systemu bankowego celem wykonania przelewów. Poniżej opisano kroki, jakie trzeba wykonać, aby móc korzystać z tej funkcji w programie.

#### Konta bankowe kontrahentów

Przed przystąpieniem do eksportu konieczne jest uzupełnienie numeru kont bankowych kontrahentów. W tym celu należy przejść do:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj Kontrahentów` — podany tutaj numer konta będzie obowiązywał we wszystkich nieruchomościach.

Natomiast jeśli wspólnota ma nadany indywidualny numer konta i jest on inny niż ogólny, to uzupełniamy go w:

- Zakładka `Administracja` > menu `Elementy` > `Konta kontrahentów`.

Wyżej wymienione sposoby są dokładniej opisane w instrukcji: **Konta bankowe kontrahentów**.

#### Uruchomienie eksportu zapłat

Kolejnym niezbędnym krokiem jest określenie kilku parametrów konta bankowego nieruchomości, z którego wykonywane są transakcje (wpłaty/wypłaty) - są to wspólne ustawienie dla `Eksportu zapłat elektronicznych` oraz dla `Importu wyciągów elektronicznych`.

- Zakładka `Zasoby` > menu `Funkcje` > `Eksportuj zapłaty elektroniczne`.
- Zakładka `Rachunki bankowe`.
- Pole `Zasób` > wybieramy budynek.
- Pole `Konto` > wybieramy konto księgowe rachunku bankowego.
- Pole `Pozycje nierozpoznane Ma (Odsetki)` > Wskazujemy Konto pozycji nierozpoznanych. W programie plik z płatnościami zawiera np. prowizje bankowe, wpłaty w kasie w banku/poczcie itp. — są to pozycje, których nie da się przypisać do konkretnego konta (właściciela/kontrahenta itp.). Wpłaty takie domyślnie będą trafiały na wskazane tutaj konto.
- Pole `Pozycje nierozpoznane Wn (Prowizje)` > Wskazujemy Konto pozycji nierozpoznanych. W programie plik z płatnościami zawiera np. prowizje bankowe, wpłaty w kasie w banku/poczcie itp. — są to pozycje, których nie da się przypisać do konkretnego konta (właściciela/kontrahenta itp.). Wpłaty takie domyślnie będą trafiały na wskazane tutaj konto.
- Pole `Bank` > Wskazujemy Bank, z którym mamy podpisaną umowę — system wygeneruje wtedy plik w odpowiednim formacie (tak, żeby można było go bez problemu zaimportować do systemu bankowego). W przypadku, gdyby na liście brakowało Państwa banku, prosimy o kontakt mailowy z danymi kontaktowymi do opiekuna — postaramy się jak najszybciej zaktualizować listę, o ile będzie taka możliwość.
- Pole `Numer` > wprowadzamy Numer rachunku bankowego. Cyfry mogą być oddzielone spacją lub wprowadzone ciągiem (bez odstępów).
- Klikamy: `Dodaj`.
- Jeśli trzeba, można dodać pozycje dla innych budynków.
- Wpisujemy hasło i zatwierdzamy.

![Eksport zapłat ustawienia początkowe](eksportzaplat1.gif)

#### Eksport zapłat

Aby pobrać plik z zapłatami, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Eksportuj zapłaty elektroniczne`.
- Zakładka `Zapłaty`.
- Pole `Rachunek` > wybieramy wspólnotę/rachunek, z którego mają wyjść zapłaty.
- Pole `Dni przed TP` > określamy ilość dni, w których przeciągu upływa termin płatności pozycji kosztowej, które podpowiedzą się do eksportu. Jeżeli wskażemy np. 7 dni, to system wygeneruje listę płatności do zrealizowania, którym w przeciągu 7 dni od bieżącej daty upływa termin płatności (ew. zaległe/przeterminowane płatności również zostaną pokazane).
- Pole `Minimalny TP` > minimalna data zlecenia przelewu zapłaty. Domyślnie jest to data bieżąca + 1 dzień.
- Klikamy: `Pobierz nieopłacone` > do dolnej części okna powinny się dodać pozycje z zapłatami. Na przycisk ten klikamy **jednokrotnie**, każde kliknięcie powoduje dodanie kolejnych, prosimy mieć to na uwadze, aby nie zlecić zapłaty dwa razy za tą samą pozycję.

Pozycje zapłat można samodzielnie edytować lub dodawać/usuwać. Aby usunąć zbędną pozycję, klikamy na symbol niebieskiego kluczyka po prawej stronie pozycji. Aby edytować, klikamy na symbol lupy. Natomiast dodawanie ręcznie nowej pozycji rozpoczynamy od przejścia do:

- Pole `Rachunek` > wybieramy wspólnotę/rachunek, z którego mają wyjść zapłaty.
- Pole `Kontrahent` > wybieramy pożądanego dostawcę.
- Pole `Dowód` > wpisujemy tytuł przelewu lub numer faktury.
- Pole `Wartość` > podajemy kwotę przelewu.
- Pole `Termin zapłaty` > podajemy dzień, w którym ma zostać zlecony przelew.
- Klikamy: `Dodaj`.

Gdy w oknie eksportu pozostaną pożądane pozycje, można pobrać plik z zapłatami, należy:

- Kliknąć: `Zatwierdź`.

Plik należy zapisać na dysku. Następnie trzeba go zaimportować do systemu bankowego.

![Eksport zapłat](eksportzaplat2.gif)

#### Podgląd faktur do zapłaty

W systemie można podejrzeć faktury, którym zbliża się termin płatności. Aby to zrobić, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Eksportuj zapłaty elektroniczne`.
- Zakładka `Nadchodzące faktury`.

W oknie zostaną wyświetleni kontrahenci oraz ich faktury, pogrupowane na dni wg. terminu płatności.

![Eksport zapłat podgląd](eksportzaplat3.gif)