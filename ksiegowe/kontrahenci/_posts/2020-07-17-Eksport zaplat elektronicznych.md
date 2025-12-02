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

Kolejnym niezbędnym krokiem jest określenie kilku parametrów konta bankowego nieruchomości, z którego wykonywane są transakcje (wpłaty/wypłaty) - są to wspólne ustawienia dla `Eksportu zapłat elektronicznych` oraz `Importu wyciągów elektronicznych`.

- Zakładka `Zasoby` > menu `Funkcje` > `Eksportuj zapłaty elektroniczne`.
- Zakładka `Rachunki bankowe`.
- Pole `Zasób` > wybieramy budynek.
- Pole `Konto FK` > wybieramy konto księgowe rachunku bankowego.
- Pole `Nazwa` > wpisujemy skróconą nazwę rachunku. (np Bieżące, FR, Lokata)
- Pole `Konto FK nierozpoznanych Ma (Odsetki)` > wskazujemy konto pozycji od banku. Na przykład: odsetki od lokat, wpłaty w kasie banku. Uznania takie domyślnie będą trafiały na wskazane tutaj konto.
- Pole `Konto FK nierozpoznanych Wn (Prowizje)` > wskazujemy konto pozycji od banku. Na przykład: prowizje bankowe, wypłaty w kasie w banku. Obciążania takie domyślnie będą trafiały na wskazane tutaj konto.
- Pole `Bank` > Wskazujemy bank, z którym mamy podpisaną umowę — system wygeneruje wtedy plik w odpowiednim formacie (tak, żeby można było go bez problemu zaimportować do systemu bankowego). W przypadku, gdyby na liście nie ma Państwa banku, prosimy o kontakt mailowy z danymi kontaktowymi do opiekuna — postaramy się jak najszybciej zaktualizować listę, o ile będzie taka możliwość.
- Pole `Rachunek bankowy` > wprowadzamy numer rachunku bankowego. Cyfry mogą być oddzielone spacją lub wprowadzone ciągiem (bez odstępów).
- Pole `Domyślny rachunek do zapłat` > wskazujemy, czy dodawany rachunek ma być domyślnym rachunkiem do płacenia za koszty zasobu. (**Patrz uwagi poniżej**).
- Klikamy: `Dodaj`.
- Jeśli trzeba, można dodać pozycje dla innych budynków.
- Klikamy: `Zatwierdź`.

Po zdefiniowaniu rachunków (i nr RB kontrahentów) można przejść do eksportu zapłat.

Uwagi do pola `Domyślny rachunek do zapłat`:

- `Tak` > ustawiamy tylko przy jednym rachunku bankowym zasobu i tylko przy takim, który ma służyć jako jedyny do opłat za koszty. Zachęcamy ustawienie `Tak` dla zasobów gdzie sytuacja jest jednoznaczna.
- Jeśli koszty zasobu, są **płacone z więcej niż jednego rachunku bankowego** danego zasobu, to zalecamy ustawienie `Nie` dla wszystkich rachunków bankowych tego zasobu, wtedy:
    - Numer rachunku, z którego zostanie zrobiony przelew, będzie sugerowany na podstawie wcześniejszych przelewów (zapłat, po zaimportowaniu ich do Weles3).
- Jeśli żaden z rachunków zasobu nie będzie miał ustawione `Tak` oraz mamy nowego kontrahenta, dla którego jeszcze nie było zapłat za jego koszty, to w eksporcie system oznaczy takie pozycje na czerwono - bedzie można je ręcznie edytować.

![Eksport zapłat ustawienia początkowe](eksportzaplat1.gif)

#### Eksport zapłat

Aby pobrać plik z zapłatami, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Eksportuj zapłaty elektroniczne`.
- Zakładka `Zapłaty`.

Jako pierwszą czynność wykonujemy:

- Klikamy: `Pobierz nieopłacone`.

Na ekranie pojawi się pop-up, w którym:

- Lista `Zasób` > wybieramy zasoby do eksportu zapłat za koszty, można zaznaczyć więcej niż jeden. Wszystkie oznaczamy klawiszem `=`.
- Pole `Dni przed TP` > określamy ilość dni, w których przeciągu upływa termin płatności pozycji kosztowej, które podpowiedzą się do eksportu. Jeżeli wskażemy np. 7 dni, to system wygeneruje listę płatności do zrealizowania, którym w przeciągu 7 dni od bieżącej daty upływa termin płatności (ew. zaległe/przeterminowane płatności również zostaną pokazane).
- Pole `Min data przelewu` > minimalna data zlecenia przelewu zapłaty w generowanym pliku. Domyślnie jest to data bieżąca + 1 dzień.
- Pole `Max data przelewu` > maksymalna data zlecenia przelewu zapłaty w generowanym pliku. Domyślnie jest to data bieżąca + 1 dzień.
- Pole `Uwzględnij rozrachunki` > decydujemy o uwzględnianiu `Łączenia rozrachunków`:
    - `Nie` > wpłaty są zaliczane na najstarsze faktury i do zapłaty pokazują się najnowsze faktury kosztowe.
    - `Tak` > system uwzględnia `Łączenie rozrachunków` i dopiero pozostałe pozycje (obciążenia/wpłaty) zapisuje na najstarsze.
- Pole `Wcześniej wyeksportowane` > decydujemy czy system:
    - `Nie uwzględniaj` > pominie pozycje które były już wcześniej wyeksportowane.
    - `Uwzględniaj` > uwzględni/pobierze pozycje które były już wcześniej wyeksportowane. 
- Klikamy: `Pobierz nieopłacone`.

W głównym oknie pojawi się nam lista pozycji zapłat za poszczególne faktury kosztowe do eksportu. Sprawdzamy ją dokładnie.

Pozycje zapłat można samodzielnie edytować lub dodawać/usuwać. Aby usunąć zbędną pozycję, klikamy na symbol `X` po prawej stronie pozycji. Aby edytować, klikamy na symbol `X`. 

Dodawanie / edycję pozycji rozpoczynamy od:

- Pole `Zasób` > wybieramy wspólnotę.
- Pole `Rachunek` > wybieramy rachunek, z którego mają wyjść zapłaty.
- Pole `Kontrahent` > wybieramy pożądanego dostawcę.
- Pole `Dowód` > wpisujemy tytuł przelewu lub numer faktury.
- Pole `Wartość` > podajemy kwotę przelewu.
- Pole `Termin zapłaty` > podajemy dzień, w którym ma zostać zlecony przelew.
- Klikamy: `Dodaj`.

Przed finalnym eksportem należy poprawić ewentualne niejasności - pozycje które sprawiają problem będą oznaczone kolorem czerwonym, bez tego przycisk `Zatwierdź` będzie nie aktywny.

![Eksport zapłat](eksport-zap01.png)

Gdy w oknie eksportu pozostaną pożądane pozycje, można pobrać plik z zapłatami, należy:

- Pole `Zapisz` > ustalamy czy:
    - `Nie zapisuj` > pozycje nie będą oznaczone jako wyeksportowane, będą się podpowiadać w przyszłości jeszcze raz.
    - `Zapisz eksportowane` > pozycje będą oznaczone jako wyeksportowane, nie będą się podpowiadać przy ponownych eksportach.
    - `Zapisz wszystkie` > TBD
- Kliknąć: `Zatwierdź`.

Plik należy zapisać na dysku. Następnie trzeba go zaimportować do systemu bankowego. W przypadku eksportu dla wielu zasobów pobierze się archiwum `ZIP`.

![Eksport zapłat](eksportzaplat2.gif)

#### Podgląd faktur do zapłaty

W systemie można podejrzeć faktury, którym zbliża się termin płatności. Aby to zrobić, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Eksportuj zapłaty elektroniczne`.
- Zakładka `Nadchodzące faktury`.

W oknie zostaną wyświetleni kontrahenci oraz ich faktury, pogrupowane na dni wg. terminu płatności.

![Eksport zapłat podgląd](eksportzaplat3.gif)