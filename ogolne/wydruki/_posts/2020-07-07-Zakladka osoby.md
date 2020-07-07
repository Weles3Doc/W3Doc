# Zakładka Osoby

Zakładka Osoby podobnie jak Dokumenty służy do przygotowywania wydruków naliczeń, ale również tych niezaksięgowanych. Wydruki z tej zakładki nie są opatrzone numerem dokumentu. Niektóre podobne elementy posiadają też bardziej rozbudowane opcje dla przygotowywania zaawansowanych zestawień. Aby wygenerować wydruk dla wybranej osoby, klikamy dwukrotnie lewym przyciskiem myszy na jego pozycję lub zaznaczamy go klawiszem spacji na klawiaturze komputera (przy właścicielu, pokaże się zielony znaczek).

![Dokumenty](dok17.png)

Po prawej stronie okna wydruków znajduje się (zawsze jako pierwsza od góry) ramka ustawień wspólnych dla przygotowywanego wydruku — w tym przypadku to Osoby. Dostępne są w nim następujące pola:

- Data na wydruku > ustawiamy datę wydruku (widoczną na wydruku).
- Sortowanie > wybieramy porządek sortowania dokumentów w generowanym pliku.
  - Mieszkanie > sortowanie wg nr mieszkań.
  - Klucz > sortowanie w porządku alfabetycznym wg pola KLUCZ. Najczęściej kluczem jest nazwisko właściciela lokalu napisane wielkimi literami.
  - Numer > sortowanie wg nr dokumentów.
  - Lista korespondencji > możliwość wygenerowania Listy korespondencji lub wydruku z wydzielonym miejscem na podpis odbiorcy (Potwierdzenie odbioru).
- Użyj nagłówka > definiuje czy użyć graficznego nagłówka strony.

Aby wygenerować wydruk, należy dodać co najmniej jeden z dostępnych składników wydruków. Poniżej znajdują się ich opisy.

### Dane logowania

Dzięki temu elementowi na wydruku możemy w łatwy sposób przekazać właścicielom/najemcom ich dane do logowania — aby mogli się zalogować do programu.

![Dokumenty](dok3.png)

### Dane lokali

Przy pomocy tego wydruku możemy wydrukować listę danych lokali przypisanych do właściciela. Jeśli wybierzemy Zbiorczo, wydrukuje się nam suma wszystkich np. powierzchni lokali. Jeśli Lokalami dane poszczególnych lokali wydrukują się osobno.

![Dokumenty](dok4.png)

### Głosowanie uchwał

Za pomocą tego elementu można stworzyć indywidualną kartę do głosowania. Na wydruku zostaną zaprezentowane uchwały, które są aktualnie poddawane głosowaniu.

![Dokumenty](dok18.png)

### Informacje na wydruku

Element odpowiada za umieszczanie informacji, które zostały dodane do systemu w Menu Zasoby > Edytuj dane właścicieli > Pole Informacje do wydruku.

![Dokumenty](dok6.png)

### Kartoteka — rozrachunki

Na wydruku zostanie pokazana kartoteka konta, która pokarze pozycje księgowe z konta właściciela, sparowane z wpłatami. Dokument ten jest pomocy w prowadzeniu rozrachunków, które weszły na drogę sądową. Funkcja posiada trzy pola do zmiany parametrów wydruku:

- Układ > wybieramy czy układ ma być wg uznań lub obciążeń.
- Data końcowa > data końcowa.
- Sumuj rozrachunki > ustawiamy czy pod konta rozrachunkowe mają być pokazywane razem, czy oddzielnie.

![Dokumenty](dok7.png)

### Kartoteka konta

Ten element pozwala na dołączenie do wydruku wykazu obrotów (wszystkich operacji) na kontach księgowych właścicieli/najemców. Funkcja posiada cztery pola do wyboru parametrów wydruku:

- Miesiąc początkowy > wybieramy miesiąc F K, od którego ma się rozpoczynać zestawienie.
- Data końcowa > wybieramy datę, na której zestawienie ma się zakończyć.
- Zakres > możemy wybrać, wg czego będziemy sortować pozycje na wydruku, np. daty księgowania, terminu płatności.
- Sumuj rozrachunki > możemy tu określić, czy system ma sumować na wydruku rozrachunki z danych kont należności.
- Wydziel obroty przyszłe > wydzielając je, można na wydruku pokazać saldo na konkrety dzień oraz pozycje przyszłe, które nie wchodzą do salda.
- Pomiń pod konta > za pomocą tej opcji można pominąć konkretne pod konta.

![Dokumenty](dok8.png)

### Lista odczytywania liczników

Za pomocą tego elementu można stworzyć indywidualną kartę do spisu odczytów liczników. Na wydruku zostaną zaprezentowana tabelka z aktualnymi licznikami dodanymi w systemie.

![Dokumenty](dok19.png)

### Lokale

Wydruk pokaże na dokumencie zwrot Dotyczy lokali: następnie wymieni lokale posiadane przez właściciela.

![Dokumenty](dok9.png)

### Naliczenia

Ten element pozwala na wydruk niezaksięgowanych dokumentów — naliczeń/zaliczek, rozliczeń/korekt, rachunków/faktur. Jest to jego podstawowe i domyślne zastosowanie w tym module. Wydruk pokaże każdy lokal właściciela oddzielnie w tabelce. Funkcja posiada pola do zmiany parametrów wydruku:

- Tytuł > wpisujemy tytuł tabelki.
- Miesiąc > wybieramy obciążenie.
- Rodzaj obciążenia > wybieramy czy drukować mają się tylko Zaliczki lub Rachunki, Lub Faktury VAT.
- Format rozliczenia > zmianę tego parametru widać dopiero przy wydruku rozliczeń (rachunki, faktury i korekty zawsze drukują się w pełnym formacie — bez względu na ustawienie). Decyduje on o tym, jak zwarta będzie forma wydruku:
  - Pełny > wyszczególnienie wszystkich pozycji na dokumentach obciążeniowych z okresu rozliczenia, oddzielne tabele obciążeń uprzednich, bieżących i różnicy (najbardziej obszerny wydruk) - domyślne ustawienie.
  - Pośredni > należności pogrupowane wg nazw algorytmów z podziałem na stawki (jeśli te ulegały zmianie), oddzielne tabele obciążeń uprzednich, bieżących i różnicy.
  - Skrócony > wszystko w jednej tabeli, tylko z pogrupowaniem wg nazw algorytmów (bez podziału na stawki).
- Grupowanie > wybieramy czy pozycje w tabelce mają być grupowane, czy pokazywane oddzielnie.
- Pokazywanie sposobu > czy program ma pokazywać w jaki sposób wyliczoną kwotę.
  - Pełne > pokazany zostanie sposób rozliczenia wszystkich wartości — domyślne ustawienie.
  - Bez R K > nie zostanie pokazany sposób (ilość i stawka) dla rozliczeń kosztów — R K R i R K L.
  - Nie pokazuj > zostanie pokazana tylko wartość końcowa naliczenia (bez ilości i stawek).
- Pokazywanie typu > czy ma być wyświetlany typ naliczenia — odpowiednia nazwa (w nawiasach), widoczna przy należności, którą można ustawić przy pomocy opcji Nazwy typów należności z menu Elementy zakładki Zasoby (domyślne oznaczenia: R — ryczałt, LP — prognoza licznika, LR — ryczałt, ale mamy licznik, L Z — zużycie wg licznika, R K R — rozliczenie kosztów ryczałt, R K L — rozliczenie kosztów licznik).
- Długie linie tekstu > funkcja określa sposób wyświetlania na wydruku długich ciągów tekstowych.

![Dokumenty](dok20.png)

### Obciążenia

Zestawienie obciążeń i wpłat właściciela, w podziale na miesiące. Funkcja posiada pięć pól do wyboru parametrów wydruku:

- Data od > wybieramy miesiąc, od którego ma się rozpoczynać zestawienie.
- Data do > data końcowa.
- Zakres > możemy wybrać, wg czego będziemy sortować pozycje na wydruku, np. daty księgowania, terminu płatności.
- Grupowanie > ustawiamy czy obciążenia miesięczne mają być pokazane w rozbiciu na grupy należności, czy nie.
- Wyświetlanie pozycji > możemy wybrać, ile pozycji dokumentu ma być wyświetlone na wydruku (np. jeżeli dokument obciążeniowy ma 4 pozycje, system je ukryje).
- Pomiń pod konta > za pomocą tej opcji można pominąć konkretne pod konta.

![Dokumenty](dok10.png)

### Obraz

Za pomocą tego elementu można umieścić grafikę/obraz na dokumencie. Na przykład skan pieczątki lu podpisu. Więcej na ten temat w instrukcji Grafiki na wydrukach.

### Odsetki

Szczegółowy opis tego elementu znajduje się w instrukcji Wydruki odsetkowe.

### Odstęp

Za pomocą tej funkcji możemy wprowadzić odstęp pomiędzy dwoma sąsiadującymi pozycjami na wydruku. W pole należy wprowadzić wartość odległości wyrażoną w punktach typograficznych (1 punkt to 1/72 cala = 0,3759 mm).

### Podział strony.

Wstawienie podziału strony — następny element wydruku będzie na następnej stronie.

### Raport odsetkowy

Wydruk, który prezentuje dane w rozbiciu na miesiące. W opcjach wydruku ustawiamy tylko miesiąc końcowy. Najważniejszą funkcją wydruku jest ukazanie właścicielowi, w którym miesiącu jego odsetki zostały pokryte. Więcej w instrukcji Wydruki odsetkowe.

### Raport z naliczeń

Przy pomocy tego wydruku możemy dołączyć do dokumentu informacje o sumie wybranych naliczeń na konkretny składnik (algorytm). W polu Nazwa algorytmu wybieramy Razem, konkretną nazwę algorytmu, lub Grupę należności, dla której chcemy wyświetlić raport.

![Dokumenty](dok11.png)

### Rozrachunki

Pozwala na dołączenie do wydruku informacji o stanie rozrachunków na konkretną datę — wykaz salda na koncie i poszczególnych kontach księgowych właściciela. Funkcja posiada cztery pola do wyboru parametrów wydruku:

- Saldo na dzień > wybieramy datę pokazywanego stanu rozrachunków.
- Drukuj > wydruk można ograniczyć do grupy właścicieli spełniających warunki:
- Tylko zalegających indywidualnie > wydrukuje zalegających właścicieli.
- Tylko numery rachunków > w tabelce pojawi się tylko imię i nazwisko, pod konto i numer konta do wpłat.
- Tylko zalegających zbiorczo > wydrukuje zalegających właścicieli.
- Minimalna zaległość > element wygeneruje się dla osób, które mają większą zaległość niż kwota podana w tym polu.
- Maksymalna zaległość > element wygeneruje się dla osób, które mają mniejszą zaległość niż kwota podana w tym polu.
- Minimalny procent > element wygeneruje się dla osób, które mają większą zaległość niż wielokrotność miesięcznych zaliczek (czynszu, opłat).
- Maksymalny procent > element wygeneruje się dla osób, które mają mniejszą zaległość niż wielokrotność miesięcznych zaliczek (czynszu, opłat).
- Sumuj rozrachunki > możemy tu określić, czy system ma sumować na wydruku rozrachunki z różnych kont właściciela.
- Zakres > możemy wybrać, wg czego będziemy sortować pozycje na wydruku, np. daty księgowania, terminu płatności.
- Obroty przyszłe > określamy, czy system ma wygenerować na wydruku informację o przyszłych obrotach, które nie wchodzą w saldo na ustawioną datę.
- Pomiń pod konta > za pomocą tej opcji można pominąć konkretne pod konta.
- Kody Q R > pokazuje kod Q R obok salda. Właściciel za pomocą aplikacji bankowej na telefonie, po zeskanowaniu kodu może zrobić przelew — nie będzie przy tym trzeba uzupełniać danych przelewu.

![Dokumenty](dok12.png)

### Tekst

Dzięki temu wydrukowi możemy umieścić na dokumencie dowolny tekst — tytuł z treścią. Funkcja posiada dwa pola tekstowe:

- Tytuł > wpisujemy tytuł elementu/części, niecałego dokumentu. Możliwe jest skorzystanie z podpowiedzi — tekstu wprowadzonego za pomocą funkcji Treść na wydruku w menu Funkcje z zakładki Administracja lub Zasoby.
- Treść > wpisujemy dowolną treść, która ma być zaprezentowana pod tytułem wydruku na dokumencie. Dodając podwójne entery — tworzymy nowy akapit w treści.

![Dokumenty](dok13.png)

### Wpis

Dzięki temu wydrukowi możemy umieścić na dokumencie dowolny tekst oraz poddać go formatowaniu (justowaniu). Funkcja posiada następujące opcje:

- Pozycja (1-1000) > Określamy początkowe położenie tekstu, gdzie 1 oznacza lewą a 1000 prawą stronę.
- Justowanie > określamy sposób justowania tekstu (Do lewej, Centruj, Do prawej).
- Treść > Wpisujemy dowolną treść, która ma być zaprezentowana pod tytułem wydruku na dokumencie.

![Dokumenty](dok14.png)

### Wykaz do zapłaty

Pozwala w łatwy i czytelny sposób dołączyć właścicielowi do wydruku informację ze wskazaniem numeru konta (można go wprowadzić za pomocą funkcji Konta bankowe z menu Elementy w zakładce Administracja) i kwoty Do zapłaty (za dany dokument/miesiąc). Funkcja posiada trzy pola do wyboru parametrów wydruku:

- Tytuł > W oknie, można określić tytuł wydruku (np. Podsumowanie).
- Drukuj podsumowanie > Określamy, czy na wydruku ma generować się podsumowanie poszczególnych grup należności.
- Kody Q R > pokazuje kod Q R obok salda. Właściciel za pomocą aplikacji bankowej na telefonie, po zeskanowaniu kodu może zrobić przelew — nie będzie przy tym trzeba uzupełniać danych przelewu.

![Dokumenty](dok15.png)

### Zestawienie obciążeń (algorytmy)

Za pomocą tego elementu można pokazać tabelkę z obciążeniami właściciela za więcej niż jeden miesiąc.

![Dokumenty](dok21.png)

### Zużycia liczników

Wydruk ten może być dołączany tylko do rozliczeń/korekt i pozwala na dodanie do dokumentu, wydruku z informacją o stanie liczników (faktycznym zużyciu). Funkcja posiada opcję generowania Podsumowania (w przypadku wystąpienia więcej niż jednego licznika danego typu, w innym wypadku, system nie wyświetli takiego podsumowania), oraz sortowania po Typ, Lokalizacja, Numer.

![Dokumenty](dok16.png)

### Filtry

Jako ostatnie są prezentowane filtry wydruków, są one szerzej opisane w instrukcji Filtry wydruków.