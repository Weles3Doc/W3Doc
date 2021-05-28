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

Kolejnym krokiem jest przywrócenie stawki użytej do naliczenia zaliczek od końca okresu rozliczeniowego. Trzeba ją przywrócić, w przeciwnym wypadku do rozliczania doliczy się korekta zaliczek. Powtarzamy wyżej wymienione punkty, stosując odpowiednią datę i wartość. Na koniec należy:

- Kliknąć: `Zapisz`.

Cały proces jest przedstawiony na poniższym materiale.

![RL po stawce wynikowej](rlpostwwynik2.gif)

#### Przeliczenie i sprawdzenie rozliczenia.

W celu sprawdzenia poprawności rozliczenia przeliczamy ponownie korektę RL.

- Przycisk `Naliczenia` > `K. bieżąca` > menu `Obciążenia` > `Nalicz korekty RL`.

Po chwili system wyświetli aktualne wyniki rozliczenia. Należy zwrócić uwagę na kolumnę `Ma być Wartość`, powinna ona zmienić się na kwotę odpowiadającą zaksięgowanym kosztom, w tym przypadku 2658,72 zł.

Kolumna `Było Wartość` prezentuje wcześniejsze obciążenia właścicieli, które podlegają rozliczeniu z zużyciem. Mogą to być zaliczki właścicieli, ale nie tylko, prócz tego może ona zwierać korekty lub rozliczenia. Jeśli kwota z tej kolumny ma taką samą wartość co przychody z konta 700 składnika, można wtedy założyć, że wszystkie zaliczki naliczone właścicielom są rozliczane.

Dodatkowe kroki sprawdzające są takie same jak przy standardowym rozliczeniu liczników:

- [Analiza liczników](https://doc.weles3.pl/administracyjne/rozliczenia%20licznikow/Analiza-licznikow.html)
- [Przeliczenie rozliczenia liczników](https://doc.weles3.pl/administracyjne/rozliczenia%20licznikow/Przeliczenie-rozliczenia.html)


#### Zaksięgowanie i sprawdzenie wydruków

Rozliczenie księgujemy na koniec okresu rozliczeniowego, postępujemy tak samo, jak w instrukcji:

- [Księgowanie rozliczenia liczników](https://doc.weles3.pl/administracyjne/rozliczenia%20licznikow/Ksiegowanie-rozliczenia-licznikow.html)

Po zaksięgowaniu należy sprawdzić efekty rozliczenia, należy wydrukować sprawozdanie finansowe za rozliczany okres:

- Menu `Funkcje` > `Wydruki` > zakładka `Zasób` > `Sprawozdanie finansowe`.

W tabelce przychody rozliczanego składnika powinny równać się kosztom, w konsekwencji saldo powinno wynosić zero. Jeśli saldo wynosi +/- kilka groszy, można je tak zostawić natomiast, jeśli jest większe, to można cofnąć rozliczenie i dodać stawkę wynikową z większą dokładnością. Być może spowoduje to zbliżenie się salda do zera.

![RL po stawce wynikowej](rlpostwwynik3.gif)