# Eksportuj zapłaty elektroniczne

Funkcja służy do generowania plików z poleceniem zapłaty np. za faktury kosztowe kontrahentów. Taki plik należy później zaimportować do systemu bankowego celem wykonania przelewów. Poniżej opisano kroki, jakie trzeba wykonać, aby móc korzystać z tej funkcji w programie.

### Konta bankowe kontrahentów

Chcąc wykonać przelew, konieczne jest określenie numerów kont bankowych kontrahentów (bez nich, bank nie będzie mógł przyjąć zlecenia — nie będzie wiedział, na jaki nr rachunku ma przelać środki). Możemy to zrobić w dwojaki sposób:
- Globalnie, dla wszystkich nieruchomości w systemie (np. gdy mamy do czynienia z firmą, która operuje tylko jednym rachunkiem bankowym dla wszystkich swoich klientów).
- Będąc w zakładce Zasoby, wybieramy menu Zasoby i Edytuj kontrahentów.

![Zapłaty elektroniczne](zaplaty1.png)

- W nowym oknie dialogowym możemy przypisać numer rachunku wybranemu kontrahentowi.

![Zapłaty elektroniczne](zaplaty2.png)

- Indywidualnie, na poziomie określonej nieruchomości (np. gdy mamy do czynienia z firmą, która używa płatności masowych dla swoich klientów i każda nieruchomość/wspólnota ma swój indywidualny, inny numer rachunku bankowego do wpłat)
- Z drzewa struktury wybieramy nieruchomość i przechodzimy do zakładki Administracja.

![Zapłaty elektroniczne](zaplaty3.png)

Z menu Elementy wybieramy Konta kontrahentów.

![Zapłaty elektroniczne](zaplaty4.png)

W nowym oknie dialogowym możemy przypisać indywidualny numer konkretnemu kontrahentowi.

![Zapłaty elektroniczne](zaplaty5.png)

### Rachunki bankowe

Kolejnym niezbędnym krokiem jest określenie Numeru konta bankowego nieruchomości, z którego wykonywane są transakcje (wpłaty/wypłaty) - jest to wspólne ustawienie dla Eksportu zapłat elektronicznych oraz dla Importu wyciągów elektronicznych.

- Będąc w zakładce Zasoby, wybieramy menu Funkcje i Eksportuj zapłaty elektroniczne.

![Zapłaty elektroniczne](zaplaty6.png)

- Po chwili otworzy się nowe okno dialogowe. Przechodzimy do zakładki Rachunki bankowe.

![Zapłaty elektroniczne](zaplaty7.png)

- Wybieramy Zasób (nieruchomość), dla której będziemy przypisywać numer konta bankowego.

![Zapłaty elektroniczne](zaplaty8.png)

- Wskazujemy Konto, na które księgowane są obroty — system pokaże tutaj wszystkie analityki konta określonego w zakładce Zasoby, menu Plan kont -> Konta syntetyczne z typem Rachunek bankowy.

![Zapłaty elektroniczne](zaplaty9.png)

- Wskazujemy Konto pozycji nierozpoznanych. W programie plik z płatnościami zawiera np. prowizje bankowe, wpłaty w kasie w banku/poczcie itp. — są to pozycje, których nie da się przypisać do konkretnego konta (właściciela/kontrahenta itp.). Wpłaty takie domyślnie będą trafiały na wskazane tutaj konto z planu kont.

![Zapłaty elektroniczne](zaplaty10.png)

- Wskazujemy Bank, z którym mamy podpisaną umowę — system wygeneruje wtedy plik w odpowiednim formacie kodowania (tak, żeby można było go bez problemu zaimportować do systemu bankowego). W przypadku, gdyby na liście brakowało Państwa banku, prosimy o kontakt mailowy z danymi kontaktowymi do opiekuna — postaramy się jak najszybciej zaktualizować listę, o ile będzie taka możliwość.

![Zapłaty elektroniczne](zaplaty11.png)

- Wprowadzamy Numer rachunku bankowego. Cyfry mogą być oddzielone spacją lub wprowadzone ciągiem (bez odstępów).

![Zapłaty elektroniczne](zaplaty12.png)

- Klikamy: Dodaj.

![Zapłaty elektroniczne](zaplaty13.png)

- Możemy od razu uzupełnić dane dla pozostałych nieruchomości.

![Zapłaty elektroniczne](zaplaty14.png)

- Całość zatwierdzamy Hasłem.

![Zapłaty elektroniczne](zaplaty15.png)

### Zapłaty

W zakładce Zapłaty wskazujemy, dla których kontrahentów program ma wygenerować plik z zapłatami elektronicznymi. System wyświetla tutaj TYLKO kontrahentów, dla których zostały wcześniej wprowadzone numery rachunków bankowych do wpłat! Z zakładki Zasoby wybieramy menu Funkcje i Eksportuj zapłaty elektroniczne.

![Zapłaty elektroniczne](zaplaty16.png)

Po chwili otworzy się nowe okno dialogowe. Mam tutaj dwie możliwości: 
- Automat — możemy wygenerować z systemu listę nieopłaconych faktur na podstawie terminu ich płatności (system na podstawie zaksięgowanych faktur kosztowych wygeneruje listę przelewów do zrealizowania).

- Wybieramy Rachunek/nieruchomość, dla której będziemy generować listę.

![Zapłaty elektroniczne](zaplaty17.png)

- Określamy ilość Dni przed TP (terminem płatności). Jeżeli wskażemy np. 7 dni, to system wygeneruje listę płatności do zrealizowania, którym w przeciągu 7 dni od bieżącej daty upływa termin płatności (ew. zaległe/przeterminowane płatności również zostaną pokazane).

![Zapłaty elektroniczne](zaplaty18.png)

- Klikamy: Pobierz nieopłacone — system powinien wygenerować listę przelewów w oknie poniżej.

![Zapłaty elektroniczne](zaplaty19.png)

- Każdy z przelewów możemy oczywiście edytować/poprawić klikając na niebieski znak klucza przy pozycji.

![Zapłaty elektroniczne](zaplaty20.png)

- Ręcznie — możemy ręcznie wskazać kontrahenta, dodać tytuł przelewu oraz kwotę.
- Wybieramy Rachunek/nieruchomość, dla której będziemy dodawać pozycje.

![Zapłaty elektroniczne](zaplaty21.png)

- Wskazujemy Kontrahenta (widoczni są TYLKO z wprowadzonym numerem konta bankowego).

![Zapłaty elektroniczne](zaplaty22.png)

- Wprowadzamy Dowód, czyli np. numer opłacanej faktury.

![Zapłaty elektroniczne](zaplaty23.png)

- Określamy Wartość przelewu.

![Zapłaty elektroniczne](zaplaty24.png)

- Klikamy: Dodaj.

![Zapłaty elektroniczne](zaplaty25.png)

- Okno Zatwierdzamy — program pobierze listę przelewów w formie pliku, który należy zaimportować do systemu bankowego (w zależności od banku będą to różne formaty — system sam o to zadba). 

![Zapłaty elektroniczne](zaplaty26.png)