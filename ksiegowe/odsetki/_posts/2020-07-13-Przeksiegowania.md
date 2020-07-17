---
title: Przeksięgowania
---
# Przeksięgowania

W przypadku gdy rozrachunki z właścicielami są prowadzone na więcej niż jednym podkoncie i jednocześnie właściciele wpłacają czynsz jednym przelewem, zachodzi potrzeba podzielenia wpłaty na różne konta rozrachunkowe. Aby wykonać przeksięgowania, należy przejść do:

- Zakładka Dekrety > Menu Dokumenty > Przeksięgowania.
- Pole Typ > wybrać:
  - Wg zakresu dat > jeśli przeksięgowania mają być zrobione na przestrzeni konkretnego okresu.
  - Bieżące > analiza kartoteki ma zajść od ustawionej daty. Nie definiujemy tutaj daty końcowej, datą końcową jest data ostatniego możliwego przeksięgowania. Dokument PK utworzy się z datą ostatniego przeksięgowania. Może on zawierać operacje z różnych miesięcy.
- W polu Sposób > wybrać: (pole aktywne tylko dla pola Typ > Wg zakresu dat)
  - Pełna analiza historii kartoteki > system zrobi przeksięgowania dla każdej daty, w której jest możliwość przeksięgowania kwoty z konta A na B.
  - Przeksięgowanie bieżącego salda > System nie analizuje kartoteki właściciela, robione jest przeksięgowanie salda na dzień poprzedzający dzień ustawiony w polu Data.
- Pola Od dnia oraz Na dzień > zależnie od wcześniejszych ustawień, definiujemy okres lub dzień przeksięgowania. 
- Klikamy: Dodaj.
- Wpisujemy hasło i zatwierdzamy.

Po zniknięciu okna w zakładce dekrety powinien pojawić się dokument PK Przeksięgowania.

![Przeksięgowania](przeksiegowania.gif)

### Uwagi:

- Aby zrobić przeksięgowania za cały miesiąc, zakres dat od ustawiamy od RRRR-XX-01 do RRRR-YY-01, czyli od pierwszego dnia miesiąca — do pierwszego dnia następnego miesiąca, a nie do RRRR-XX-31.
- Dokumenty PK stworzone przez system można dowolnie edytować (np. usunąć i zrobić ponownie).
- System nie dokona przeksięgowania, jeśli na podkoncie właściciela jest zadłużenie.
- System analizuje podkonto właściciela według terminów płatności pozycji, nie wg dat księgowań.
- Przeksięgowania można robić kilkukrotnie za ten sam okres, system nie będzie dublował przeksięgowań.
- System przeksięguje kwotę w takiej wysokości:
  - aby pokryć całą należność na koncie docelowym. (nie przeksięguje więcej, niż trzeba)
  - lub przeksięguje tyle ile może. (nie spowoduje ujemnego salda na koncie źródłowym) 
- Oczywiście przeksięgowań nie stosujemy, jeśli rozrachunki z właścicielem są prowadzone na jednym koncie rozrachunkowym.