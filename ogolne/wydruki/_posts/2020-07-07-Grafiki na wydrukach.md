---
title: Grafiki na wydrukach
---

# Grafiki na wydrukach

Program pozwana na umieszczenie plików graficznych na systemowych wydrukach. Dzięki temu wydrukom można nadać profesjonalny wygląd — dodając nagłówek lub dodać skan pieczątki, lub podpisu na końcu dokumentu. Wszystko zaczyna się od stworzenia grafiki/skanu do umieszczenia w programie.

W przypadku nagłówka strony zalecamy rozmiar grafiki `2244 × 300` oraz ustawienie DPI na `300`, co w konsekwencji da obraz rozmiaru 19,00 cm x 2,54 cm. Nagłówek dokumentu tworzymy w zewnętrznym programie. Przykład:

![Przykład nagłówka](przykladnaglowka.png)

W przypadku skanu pieczątki/podpisu — tutaj rozmiar grafiki i DPI zależy od fizycznego rozmiaru pieczątki i opcji skanowania. Schemat postępowania jest tutaj następujący:

- Podczas skanowania, w opcjach ustawiamy obszar skanowania jak najbardziej dopasowany do rozmiaru pieczątki/podpisu.
- Importujemy plik do systemu, DPI ustawiamy takie same jak użyte podczas skanowania.

#### Dodanie obrazu do systemu

Po stworzeniu lub zeskanowaniu obrazu trzeba dodać go do systemu. Aby zaimportować plik, należy przejść do:

- Menu `Funkcje` > `Wydruki`.
- Menu `Funkcje` > `Obrazy dla wydruków`.
- Klikamy: `Utwórz`.
- Pole `Plik` > wybieramy plik z dysku komputera.
- Pole `Nazwa` > wpisujemy opis pliku.
- Pole `DPI` > wpisujemy pożądane DPI (np. 300).
- Pole `Użyj jako nagłowka` > `Tak` / `Nie` > decydujemy, czy obraz ma być nagłowkiem.
- Pole `Nagłówek dla` > wyświetli się tylko wtedy, gdy w poprzednim polu wybraliśmy `Tak`.
    - `Weles 3 FK` > wybieramy tę pozycję jeśli chcemy, aby dodawany plik był nagłowkiem dla wszystkich zasobów.
    - Jeśli dodawany plik jest indywidualny, wybieramy konkretny zasób z listy.
- Klikamy: `Utwórz`.

Okno zamknie się, wczytana grafika jest od razu możliwa do użycia na wydrukach. W podobny sposób edytujemy ustawienia pliku graficznego, z tą różnicą że po wybraniu pliku, naciskamy `Edytuj`.

![Dodanie grafiki](dodanieobrazka.gif)

#### Użycie nagłówka na wydrukach

Jeśli importowaliśmy plik, który ma być użyty jako nagłówek, to od razu będzie on używany przez system przy tworzeniu wydruków. Ustawienia dotyczące nagłówka znajdują się w:

- Menu `Funkcje` > `Wydruki`.

W każdej zakładce znajduje się pole `Użyj nagłówka`.

![Ustawienie nagłówka](uzyjnaglowka.png)

Można tutaj ustawić:

- `Użyj i skaluj` > domyślny wybór, zazwyczaj nie trzeba zmieniać, nagłówek zostanie pokazany na wydruku, jego szerokość zostanie dostosowana do marginesów bocznych strony.
- `Użyj` > nagłowek zostanie użyty, jego rozmiar będzie determinowany przez ustawione DPI podczas dodawania pliku.
- `Nie używaj` > wyłącza pokazywanie nagłówka.

#### Użycie obrazów na wydrukach

Aby użyć grafiki na wydrukach, należy przejść do:

- Menu `Funkcje` > `Wydruki`.

Następnie należy skomponować wydruk z listy elementów dostępnych w środkowej części okna. W dowolnym momencie należy dodać element `Obraz`, a w opcjach ustawić:

- Pole `Obraz` > wybieramy:
    - `Obraz pobrany z dysku` > grafikę można dodać prosto z dysku komputera. Jeśli to wybierzemy, dodajemy plik w polu `Plik z dysku`.
    - Jako kolejne pozycje w tym polu będą wyświetlane wcześniej dodane pliki graficzne do systemu, wybieramy jeden z nich.
- Pole `Pozycja` > ustawiamy odległość, to pole jest zależne od pola `Justowanie`.
- Pole `DPI` > ustawiamy DPI. Wpisując wartość możemy dostosować wielkość obrazka. Typowy zakres od 100 do 600 DPI. Pozostawiając te pole puste, zostanie użyte domyślne DPI określone przy dodawaniu pliku.
- Pole `Justowanie` > ustawiamy justowanie.

Na koniec sprawdzamy wygląd wydruku w PDF:

- Klikamy: `Podgląd wydruku`.

Zachęcamy do samodzielnego przetestowania różnych ustawień w elemencie `Obraz`.

![Użycie grafiki](uzyciegrafiki.gif)

#### Przykładowy wydruk

Poniżej przedstawiamy przykładowy wydruk z użytym nagłówkiem strony oraz stopką graficzną.

![Użycie grafiki](przykladgrafikipdf.png)

#### Skanowanie

Proces skanowania przedstawiamy poniżej. Prosimy zapamiętać DPI skanowanych obrazków.

![Skanowanie podpisu](skanowanie.gif)

#### Uwagi:

- W polu DPI określamy gęstość obrazka, czyli liczba punktów (kropek) obrazu przypadająca na cal. Szerokość obrazka na wydruku to 2.54 * szerokość pikseli / dpi [cm], czyli przykładowo obrazek o szerokości 2480 pikseli przy 300 dpi ma szerokość 21 cm na wydruku (szerokość formatu A4). Istnieją następujące zależności: im wyższa liczba dpi tym obrazek na wydruku jest lepszej jakości (słabiej widać kropki/rozmycie), ale też staje się mniejszy, jeśli natomiast zmniejszamy liczbę dpi, obrazek staje się większy, ale też bardziej stają się widoczne jego niedoskonałości (kropki — punkty/piksele). Najlepiej stosować obrazy o możliwie najwyższej (wysokiej) rozdzielczości pikseli i dopasować je do wydruku zwiększając liczbę DPI.

Do wyliczania szerokości obrazu na wydruku, wykorzystujemy równanie:
- szerokość na wydruku [cm] = 2,54 * szerokość obrazka [pikseli] / DPI.

Do wyliczenia wartość DPI, aby uzyskać konkretny rozmiar obrazu na wydruku, wykorzystujemy przekształcone równanie:
- DPI = 2,54 * szerokość obrazka [pikseli] / szerokość na wydruku [cm].