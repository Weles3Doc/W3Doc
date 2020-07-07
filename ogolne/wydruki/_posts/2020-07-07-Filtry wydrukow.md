# Filtry wydruków

System pozwala na ustawienie prostych filtrów w wydrukach dokumentów. Mamy tutaj możliwość: wykluczenia byłych właścicieli, wygenerowania zawiadomienia dla właścicieli, u których zmieniły się wartości obciążeń względem konkretnego miesiąca, czy też utworzyć dokument tylko dla właścicieli, którzy nie mają wprowadzonych adresów e-mail (przydatne, gdy części właścicieli wysyłamy zawiadomienia przez e-mail, a pozostałym tradycyjne papierowe). Funkcje filtrów są tylko opcją, a nie samodzielnym wydrukiem — mogą być użyte tylko w połączeniu z jakimś innym wydrukiem/wydrukami (np. Dokument + Wykaz do zapłaty).

![Filtry wydruków](filtrywydrukow.gif)

### Aktualny właściciel

![Filtry wydruków](filtr1.png)

Opcja ta pozwala na wskazanie właścicieli, którzy na dany dzień mają/nie mają lokalu. Jest przydatna, gdy chcemy wygenerować wydruk tylko dla aktualnych właścicieli lokali lub odwrotnie — gdy chcemy wysłać pismo tylko do byłych właścicieli (przykładowo o planowanym rozliczeniu kosztów, które będzie także ich dotyczyło). Funkcja posiada dwa pola wyboru:

- Na dzień — określamy konkretną datę, z którą system ma sprawdzać stan posiadania lokalu.
- Posiadanie — ustawiamy parametry filtrów:
  - Posiada lokal — wydruk tylko dla posiadających lokal we wskazanym dniu.
  - Nie posiada lokalu — wydruk tylko dla nieposiadających lokalu we wskazanym dniu.

### Dane kontaktowe

![Filtry wydruków](filtr2.png)

Dzięki temu filtrowi możemy wskazać tylko tych właścicieli, którzy posiadają określone dane kontaktowe, takie jak: adres e-mail, czy kontaktowy nr telefonu. Funkcja jest szczególnie przydatna, gdy nie wszyscy właściciele posiadają wprowadzone adresy e-mail do programu (część zawiadomień wysyłamy za pomocą poczty elektronicznej a pozostałe tradycyjnie papierowe). Funkcja ta posiada dwa pola wyboru:

- Forma kontaktu — wybieramy rodzaj kontaktu, którego posiadanie system ma sprawdzać.
  - Telefon — system sprawdza, czy właściciel ma wprowadzony jakikolwiek nr telefonu (stacjonarny lub komórkowy).
  - Telefon komórkowy — system sprawdza, czy właściciel ma wprowadzony nr telefonu komórkowego.
  - Telefon stacjonarny — system sprawdza, czy właściciel ma wprowadzony nr telefonu stacjonarnego.
  - E-mail — system sprawdza, czy właściciel ma wprowadzony adres poczty elektronicznej.
- Posiadanie — ustawiamy parametry filtrów:
  - Posiada — wydruk tylko dla tych, którzy posiadają wskazaną formę kontaktu wprowadzoną do systemu.
  - Nie posiada — wydruk tylko dla tych, którzy nie posiadają wskazanej formy kontaktu wprowadzonej do systemu.

### Zmiany naliczeń

![Filtry wydruków](filtr3.png)

Filtr ten pozwala wygenerować zawiadomienia tylko dla tych właścicieli, którym zmieniły się wartości zaliczek, w porównaniu do innego, wskazanego przez nas obciążenia. Funkcja ta jest szczególnie przydatna, gdy zawiadomień o zaliczkach nie przekazujemy właścicielom w sposób cykliczny, ale incydentalny — przykładowo, gdy zaliczki ulegają zmianie tylko niektórym właścicielom i tylko dla nich chcemy przygotować wydruk. Funkcja posiada dwa pola wyboru:

- Miesiąc — wskazujemy konkretne naliczenie, do którego system ma przyrównać bieżące, aktualnie drukowane obciążenia.
- Zmiana — ustawiamy parametry filtrów:
  - Zmiana naliczeń — wydruk tylko wtedy, gdy nastąpiła zmiana w naliczeniach w porównaniu do wskazanego wyżej miesiąca/naliczenia.
  - Brak zmiany — wydruk tylko wtedy, gdy obciążenia nie uległy zmianie w porównaniu do wskazanego wyżej miesiąca/naliczenia.

### Dane

![Filtry wydruków](filtr4.png)

Filtr ten pozwala wygenerować wydruki tylko dla tych osób, dla których zostaną spełnione warunki określone w polach wyboru filtru. Przykładowo do lokali można dodać daną określającą numer budynku/klatki, dzięki temu drukować dokumenty dla określonej grupy. Można też określić kryterium odnośnie do powierzchni, drukować tylko dokumenty lokalom przekraczającym 100 metrów kwadratowych. Gdy zostanie wybrana dana Liczba garaży — dokumenty stworzą się tylko dla właścicieli garaży.

### Wydruk główny i zależny

![Filtry wydruków](filtr5.png)


Tworząc dokument, można uzależnić wydruk od tego, czy inne wydruki mają do przedstawienia jakiekolwiek informacje. Ustawiamy to za pomocą ikon wskazanych po lewej:

- (i) - domyślny — oznacza wydruk główny, wydrukuje się zawsze, jeśli warunki ustawione w opcjach wydruku zostaną spełnione dla właściciela.
- (?) - oznacza wydruk zależny — wydrukuje się tylko wtedy, jeżeli chociaż jeden z wydruków głównych pokarze informacje.
Filtr ten ma za zadanie ograniczenie generowania niepełnych dokumentów, na przykład takich gdzie na wydruku uzyskujemy sam tekst, bez tabelki z opłatami. Szczególnie pomaga na pominięcie byłych właścicieli przy drukowaniu zawiadomień o opłatach.
