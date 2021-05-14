---
title: 3. Księgowanie korekty
---

# Księgowanie korekty

Po przygotowaniu korekty i po sprawdzeniu jej można przejść do księgowania. Aby zaksięgować zwyczajną korektę, należy:

- Menu `Funkcje` > `Księguj należności`.
- Pole `Księgowanie` > `Korekty`.
- Pole `Data` > ustawiamy miesiąc księgowania korekty w części administracyjnej. Zazwyczaj będzie to ostatni miesiąc korygowanego okresu. Można tutaj ustawić miesiąc późniejszy niż korygowany okres (ale nie większy niż ostatnie zaksięgowane naliczenia) wtedy księgowana korekta potencjalnie obejmie większą ilość zmian. Natomiast jeśli zostanie wybrany miesiąc wcześniejszy (lub w trakcie) niż okres korygowany to księgowanie korekty obejmie zmiany tylko do tego miesiąca, część korekty (zmian) pozostanie nie zaksięgowana, dostępna do następnych księgowań w `K.bieżąca`. W ten sposób można podzielić korektę na części.
- Pole `Data księgowania` > ustawiamy datę księgowania korekty w części księgowej. Zazwyczaj będzie to ostatni dzień miesiąca wybranego w polu `Data`. Jeśli potrzeba można tutaj wybrać datę późniejszą. Numeracja dokumentów przyjmie wartości z miesiąca wybranego w tym polu.
- Pole `Bazowy termin płatności` > ustawiamy datę w zależności od pożądanego terminu płatności, więcej w dokumentacji: **[Terminy płatności](https://doc.weles3.pl/administracyjne/system/Terminy-platnosci.html)**.
- Pole `Termin płatności zwrotów` > wybieramy:
  - `Data` > jeśli termin **zwrotów** ma być na pierwszy dzień następnego miesiąca po miesiącu określonym w polu `Data`.
  - `Bazowy termin płatności` > jeśli termin **zwrotów** ma być na datę określoną w polu `Bazowy termin płatności`.
- Pole `Opis` > umieszczamy opis księgowanej należności (tekst ten będzie widoczny na wydrukach).
- Pole `Hasło` > wpisać hasło.
- Klikamy: `Zatwierdź`.

Zaksięgowanie można sprawdzić w zakładce `Dekrety`, po czym można przejść do wydruku korekty.

Korekty przechodzące przez koniec roku można zaksięgować w podziale, pierwszy raz wskazując pole `Data` = RRRR-12 oraz pole `Data księgowania` = RRRR-12-31, drugi raz wskazując daty w roku następnym. Dzięki temu przychody poprzedniego roku zostaną w nim prawidłowo skorygowane.

![Księgowanie korekty](ksiegowaniekorekty.gif)