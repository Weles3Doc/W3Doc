---
title: Rozliczenie po stawce wynikowej
---

# Rozliczenie po stawce wynikowej

W przypadku rozliczeń mediów (szczególnie licznikowych) może się tak zdarzyć, że nie chcemy korzystać z dostępnego w systemie mechanizmu automatycznych rozliczeń kosztów. Alternatywnie chcielibyśmy samemu wyliczyć stawkę, która przemnożona przez podstawę rozliczenia (np. zużycie wg liczników, powierzchnia lub liczba osób) da nam kwotę faktycznego obciążenia.

Instrukcja ma na celu jedynie pokazanie sposobu rozliczenia stawką wynikową. Pominięte zostały punkty takie jak:

- Ustawienie terminów rozliczenia liczników.
- Wprowadzenie odczytów.
- Analiza liczników (**Ważne**).
- Przeliczenie korekty rozliczenia liczników (RL) - w instrukcji zajmiemy się tylko CW.

Poniższa instrukcja zakłada, że wszyscy właściciele mają aktywne liczniki CW. Jeżeli zdarzy się, że któryś z właścicieli będzie rozliczany wg ryczałtu (nie ma wykazanego zużycia licznika), trzeba będzie wyodrębnić część kosztów na niego przypadających (instrukcja tego nie uwzględnia).

Mając wyżej wymienione punkty za sobą, przystępujemy do rozliczenia liczników wg stawki wynikowej.

#### Wydruk zużyć liczników i kosztów do rozliczenia

W pierwszej kolejności potrzebujemy informacji na temat sumarycznego zużycia liczników oraz wartości zaksięgowanych kosztów.

Zużycia liczników można sprawdzić w trzech miejscach, we wszystkich powinny być zgodne:

- Przycisk `Naliczenia` > `K. bieżąca` > menu `Obciążenia` > `Nalicz korekty RL`.
- Przycisk `Liczniki`.
- Menu `Funkcje` > `Wydruki` > zakładka `Zasób` > `Zużycia liczników`.

Koszty sprawdzamy w:
- Zakładka `Konta FK`.
- Menu `Funkcje` > `Wydruki` > zakładka `Zasób` > `Sprawozdanie finansowe`.

Tu należy zaznaczyć, aby ustawić poprawne daty Od i Do na wydrukach. Na niżej przedstawionym przykładzie z wydruków odczytujemy:

- Koszty = 2658,72 zł.
- Zużycie = 162 m3.

![RL po stawce wynikowej](rlpostwwynik1.gif)


#### Wyliczenie oraz dodanie stawki wynikowej

Przy rozliczeniu kosztów dążymy do sytuacji, gdzie pobrane zaliczki (700) równają się zaksięgowanym kosztom (400).

- Koszty = 2658,72 zł.
- Zużycie = 162 m3.

Chcąc wyliczyć stawkę wynikową, dzielimy wartość kosztów przez zużycie liczników. Z powyższego działania wynika, że nasza stawka wynikowa wynosi 16,4118 zł/m3. Bardzo ważne jest tutaj zastosowanie odpowiedniego przybliżenia przy wyniku. Zbyt małe przybliżenie spowoduje, że przychody nie będą się równały kosztom — pozostanie różnica rzędu kilku (nastu) złotych. Im większe przybliżenie, tym dokładniejszy wynik.

Obecną stawkę do rozliczenia liczników musimy zastąpić wyliczoną wcześniej stawką wynikową. Aby dodać stawkę wynikową, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj stawki`.
- Pole `Lokal` > wybrać cały budynek, stawki dodajemy zazwyczaj na cały budynek.
- Pole `Stawka` > wybrać żądaną stawkę.
- Pole `Data` > wprowadzić datę, od kiedy ma obowiązywać wartość stawki, będzie to początek okresu rozliczenia.
- Pole `Wartość` > wprowadzamy wartość stawki wynikowej.
- Pole `Typ` > wybieramy typ VAT stawki, jeśli WM nie jest vatowcem, to pozostawiamy `Brutto`.
- Kliknąć: `Dodaj`.

Kolejnym krokiem jest przywrócenie stawki użytej do naliczenia zaliczek od końca okresu rozliczeniowego. Trzeba ją przywrócić, w przeciwnym wypadku do rozliczania doliczy się korekta zaliczek. Powtarzamy wyżej wymienione punkty, stosując odpowiednią datę i wartość.

- Kliknąć: `Zapisz`.

Cały proces jest przedstawiony na poniższym materiale.

![RL po stawce wynikowej](rlpostwwynik2.gif)

#### Przeliczenie i sprawdzenie rozliczenia.

W celu sprawdzenia poprawności rozliczenia przeliczamy ponownie korektę RL.

- Przycisk `Naliczenia` > `K. bieżąca` > menu `Obciążenia` > `Nalicz korekty RL`.

Po chwili system wyświetli aktualne wyniki rozliczenia. Jak widać, Pozycja Ma być, zmieniła się na 77,00 zł, czyli dokładnie tyle, co zaksięgowane koszty.

Po chwili system wygeneruje dokument w formacie pdf. Jak widać, konto CW jest zbilansowane do zera (przychody = koszty). Rozliczenie jest wykonane prawidłowo.