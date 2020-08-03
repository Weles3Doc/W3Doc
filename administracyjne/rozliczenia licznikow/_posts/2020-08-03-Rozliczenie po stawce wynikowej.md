---
title: Rozliczenie po stawce wynikowej
---

# Rozliczenie po stawce wynikowej

W przypadku rozliczeń mediów (szczególnie licznikowych) może się tak zdarzyć, że nie chcemy korzystać z dostępnego w systemie mechanizmu automatycznych rozliczeń kosztów. Alternatywnie chcielibyśmy samemu wyliczyć stawkę, która przemnożona przez podstawę rozliczenia (np. zużycie wg liczników, powierzchnia lub liczba osób) da nam kwotę faktycznego obciążenia.

### Wyliczenie stawki dla algorytmu licznikowego
Instrukcja ma na celu jedynie pokazanie sposobu rozliczenia stawką wynikową. Pominięte zostały punkty takie jak:

- Ustawienie terminów rozliczenia liczników,
- Wprowadzenie odczytów
- Analiza liczników
- Przeliczenie korekty rozliczenia liczników (RL) - w instrukcji zajmiemy się tylko CW.

Poniższa instrukcja zakłada, że wszyscy właściciele mają aktywne liczniki CW. Jeżeli zdarzy się, że któryś z właścicieli będzie rozliczany wg ryczałtu (nie ma wykazanego zużycia licznika), trzeba będzie wyodrębnić część kosztów na niego przypadających (instrukcja tego nie uwzględnia)!


Mając wyżej wymienione punkty za sobą, przystępujemy do rozliczenia liczników wg stawki wynikowej.

### Wydruk zużyć liczników i kosztów do rozliczenia

W pierwszej kolejności potrzebujemy informacji na temat sumarycznego zużycia liczników oraz wartości zaksięgowanych kosztów. W tym celu:

- Z drzewa struktury wybieramy nieruchomość i przechodzimy do zakładki Administracja.

![RL po stawce wynikowej](rlstawkawynik1.png)

- Z menu Funkcje, wybieramy Wydruki.

![RL po stawce wynikowej](rlstawkawynik2.png)

- Przechodzimy do zakładki Zasób. Z listy wydruków, wybieramy Rozliczenie (za cały rozliczany okres) i Zużycia liczników dla K. bieżąca (najlepiej ze szczegółowym podsumowaniem).

![RL po stawce wynikowej](rlstawkawynik3.png)

- Na koniec, klikamy w Podgląd wydruku (F12).

![RL po stawce wynikowej](rlstawkawynik4.png)

- Po chwili system wyświetli dokument w formacie pdf. Jak widać, zaksięgowane koszty dla CW to 77,00 zł (mamy niedobór 14,00 zł). Zużycie liczników dla CW to 4 m3.

![RL po stawce wynikowej](rlstawkawynik5.png)

### Wyliczenie oraz dodanie stawki wynikowej

Przy rozliczeniu kosztów dążymy do sytuacji, gdzie pobrane zaliczki (700) równają się zaksięgowanym kosztom (400).

Chcąc wyliczyć stawkę wynikową, dzielimy wartość kosztów (77,00 zł) przez zużycie liczników (4 m3). Z powyższego działania wynika, że nasza stawka wynikowa wynosi 19,25 zł/m3. Bardzo ważne jest tutaj zastosowanie odpowiedniego przybliżenia przy wyniku. Zbyt małe przybliżenie spowoduje, że przychody nie będą się równały kosztom — pozostanie różnica rzędu kilku (nastu) złotych. Im większe przybliżenie, tym dokładniejszy wynik.

Księgując obecne rozliczenie liczników, przychody nie będą się równały kosztom. Sumarycznie, po stronie przychodów będzie 56,00 zł, po stronie kosztów 77,00 zł. Obecną stawkę do rozliczenia liczników musimy zastąpić wyliczoną wcześniej stawką wynikową.

Chcąc dodać stawkę wynikową:

- Będąc w zakładce Administracja, wybieramy z menu Zasoby funkcję Edytuj stawki.

![RL po stawce wynikowej](rlstawkawynik6.png)

- Po chwili otworzy się nowe okno dialogowe. Z pola Lokal wybieramy całą nieruchomość. W polu Stawka odszukujemy naszą stawkę.

![RL po stawce wynikowej](rlstawkawynik7.png)

- Data wprowadzenia stawki to początek rozliczanego okresu.

![RL po stawce wynikowej](rlstawkawynik8.png)

- W pole Wartość wprowadzamy naszą stawkę wynikową. Określamy również Typ VAT.

![RL po stawce wynikowej](rlstawkawynik9.png)

- Dodajemy pozycję do listy przyciskiem Dodaj.

![RL po stawce wynikowej](rlstawkawynik10.png)

- Kolejnym krokiem jest przywrócenie stawki użytej dla naliczenia zaliczek. Naliczenia za CW są wg prognoz liczników (pomnożone przez stawkę CW [m3]). Przy obecnym układzie, stawka wzięta do zaliczek zmieni się! Musimy zatem wprowadzić kolejną pozycję przywracającą prawidłową stawkę od bieżących naliczeń.

![RL po stawce wynikowej](rlstawkawynik11.png)

- Na koniec wprowadzamy hasło i zatwierdzamy okno przyciskiem Zatwierdź.

![RL po stawce wynikowej](rlstawkawynik12.png)

### Księgowanie korekty oraz wydruki sprawdzające.

W celu sprawdzenia poprawności rozliczenia przeliczamy ponownie korektę RL.

- Z menu Obciążenia, wybieramy Nalicz korekty RL.

![RL po stawce wynikowej](rlstawkawynik13.png)

- Po chwili system wyświetli aktualne wyniki rozliczenia. Jak widać, Pozycja Ma być, zmieniła się na 77,00 zł, czyli dokładnie tyle, co zaksięgowane koszty.

![RL po stawce wynikowej](rlstawkawynik14.png)

- Możemy przystąpić do zaksięgowania rozliczenia. Z menu Funkcje, wybieramy Księguj należności.

![RL po stawce wynikowej](rlstawkawynik15.png)

- Otworzy się nowe okno dialogowe. Z pola Księgowanie, wybieramy Korekty RL.

![RL po stawce wynikowej](rlstawkawynik16.png)

- Pola Data, Data księgowania i Bazowy termin płatności, mogą zostać bez zmian.

![RL po stawce wynikowej](rlstawkawynik17.png)

- Na koniec wpisujemy hasło i zatwierdzamy przyciskiem Zatwierdź.

![RL po stawce wynikowej](rlstawkawynik18.png)

- Dokument pokaże się na liście zaksięgowanych obciążeń.

![RL po stawce wynikowej](rlstawkawynik19.png)

- Pozostaje jeszcze sprawdzić salda po rozliczeniu. Z menu Funkcje wybieramy Wydruki.

![RL po stawce wynikowej](rlstawkawynik20.png)

- Z zakładki Zasób, wybieramy wydruk Rozliczenie.

![RL po stawce wynikowej](rlstawkawynik21.png)

- Następnie, klikamy w Podgląd wydruku (F12).

![RL po stawce wynikowej](rlstawkawynik22.png)

- Po chwili system wygeneruje dokument w formacie pdf. Jak widać, konto CW jest zbilansowane do zera (przychody = koszty). Rozliczenie jest wykonane prawidłowo.

![RL po stawce wynikowej](rlstawkawynik23.png)