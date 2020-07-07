# Grafiki na wydrukach

Program pozwana na umieszczenie plików graficznych na systemowych wydrukach. Dzięki temu wydrukom można nadać profesjonalny wygląd — dodając nagłówek lub dodać skan pieczątki, lub podpisu na końcu dokumentu. Wszystko zaczyna się od stworzenia grafiki/skanu do umieszczenia w programie. W przypadku:

- Nagłówka strony zalecamy rozmiar grafiki 2244 × 300 oraz ustawienie DPI na 300, co w konsekwencji da obraz rozmiaru 19,00 cm x 2,54 cm. Nagłówek dokumentu tworzymy w zewnętrznym programie. Przykład:

![Przykład nagłówka](przykladnaglowka.png)

- Skan pieczątki/podpisu — tutaj rozmiar grafiki i DPI zależy od fizycznego rozmiaru pieczątki i opcji skanowania. Schemat postępowania jest tutaj następujący:
- Podczas skanowania, w opcjach ustawiamy obszar skanowania jak najbardziej dopasowany do rozmiaru pieczątki/podpisu.
- Importujemy plik do systemu, DPI ustawiamy takie same jak użyte podczas skanowania.

Proces skanowania przedstawiamy poniżej.

![Skanowanie podpisu](skanowanie.gif)

Po stworzeniu lub zeskanowaniu obrazu trzeba dodać go do systemu. Aby zaimportować plik, należy przejść do:

- Menu funkcje > Wydruki.
- W oknie wydruki > Menu funkcje > Obrazy dla wydruków.
- Zakładka Dodawanie.
- Pole Plik > wybieramy plik z dysku komputera.
- Pole DPI > wpisujemy pożądane DPI.
- Pole Opis > wpisujemy opis pliku.
- Wpisujemy hasło i zatwierdzamy.

Okno zamknie się, wczytana grafika jest od razu możliwa do użycia na wydrukach.

![Dodanie grafiki](dodanieobrazka.gif)

Jeśli importowaliśmy plik, który ma być użyty jako nagłówek, to trzeba ustawić ten parametr w systemie. Aby to zrobić, należy przejść do:

- Menu funkcje > Wydruki.
- W oknie wydruki > Menu funkcje > Obrazy dla wydruków.
- Zakładka Edycja.
- Pole Obraz > wybieramy plik z listy.
- Pole Nazwa > pozostawiamy bez zmian lub ew. zmieniamy na inne.
- Pole DPI > pozostawiamy bez zmian lub ew. zmieniamy na inne.
- Pole Użyj jako nagłówka > wybieramy Użyj.
- Pole Nagłówek dla > ustawiamy Weles 3 F K, jeśli ma być dostępny w każdym budynku.
- Klikamy: Dodaj.
- Wpisujemy hasło i zatwierdzamy.

Od tego momentu można używać nagłówka na wydrukach. Powyższe czynności na ogół wykonujemy tylko raz.

![Ustawienie nagłówka](ustawienienaglowka.gif)

Aby użyć dodanej grafiki na wydrukach, należy przejść do:

- Menu funkcje > Wydruki.
- W polu Użyj, nagłówka można ustawić drukowanie się nagłówka strony.
- Skomponować wydruk.
- Za dodanie skanu pieczątki lub podpisu, lub innej grafiki, odpowiada wydruk: Obraz.
- Pole Obraz > ustawiamy odpowiedni plik.
- Pole Pozycja > ustawiamy odległość, to pole jest zależne od pola Justowanie.
- Pole DPI > ustawiamy DPI.
- Pole Justowanie > ustawiamy justowanie.
- Klikamy: Podgląd wydruku.

Aby nie powtarzać za każdym razem tych czynności, sugerujemy skorzystać ze Schematów wydruków.

![Użycie grafiki](uzyciegrafiki.gif)

![Użycie grafiki](przykladgrafikipdf.png)

### Uwagi:

- W polu DPI określamy gęstość obrazka, czyli liczba punktów (kropek) obrazu przypadająca na cal. Szerokość obrazka na wydruku to 2.54 * szerokość pikseli / dpi [cm], czyli przykładowo obrazek o szerokości 2480 pikseli przy 300 dpi ma szerokość 21 cm na wydruku (szerokość formatu A4). Istnieją następujące zależności: im wyższa liczba dpi tym obrazek na wydruku jest lepszej jakości (słabiej widać kropki/rozmycie), ale też staje się mniejszy, jeśli natomiast zmniejszamy liczbę dpi, obrazek staje się większy, ale też bardziej stają się widoczne jego niedoskonałości (kropki — punkty/piksele). Najlepiej stosować obrazy o możliwie najwyższej (wysokiej) rozdzielczości pikseli i dopasować je do wydruku zwiększając liczbę DPI.

Do wyliczania szerokości obrazu na wydruku, wykorzystujemy równanie:
- szerokość na wydruku [cm] = 2,54 * szerokość obrazka [pikseli] / DPI.

Do wyliczenia wartość DPI, aby uzyskać konkretny rozmiar obrazu na wydruku, wykorzystujemy przekształcone równanie:
- DPI = 2,54 * szerokość obrazka [pikseli] / szerokość na wydruku [cm].