---
title: Sposób liczenia sald 201
---

# Sposób liczenia sald na kontach 201

W systemie jest możliwość ustalenia sposobu pokazywania sald właścicieli. Sposób ten można zmieniać tylko w dwóch określonych momentach:

- Przy zakładaniu WM, gdy nie ma w niej jeszcze żadnych księgowań.
    - Zakładka `Dekrety` > menu `Elementy` > `Sposób liczenia salda`
- Przy zamykaniu roku ustalamy sposób liczenia sald na następny rok.
    - Zakładka `Dekrety` > menu `Funkcje` > `Zamykanie roku FK`

Dostępne są trzy metodologie liczenia salda dla właścicieli lokali:

#### Obroty przyszłe osobno (nowa domyślna)

Zaległości są pokrywane przez wpłaty dopiero po upływie terminu płatności. Może jednocześnie istnieć saldo Wn i saldo Ma na jednym koncie.

Przykład:
- obciążenie w kwocie 100 zł z dnia 2018-01-01 z terminem na 2018-01-20
- wpłata w kwocie 80 zł z dnia 2018-10

Salda:
- 2018-01-01 - 2018-01-09: Wn 100 zł, Ma 0 zł
- 2018-01-10 - 2018-01-19: Wn 100 zł, Ma 80 zł
- 2018-01-20: Wn 20 zł, Ma 0 zł

#### Saldo wg daty księgowania (dotychczasowa domyślna)

Zaległości są pokrywane przez wpłaty z datą księgowania wpłaty. Opcja ta obowiązuje dla wszystkich kont niezwiązanych z właścicielami lokali.

Przykład:
- obciążenie w kwocie 100 zł z dnia 2018-01-01 z terminem na 2018-01-20
- wpłata w kwocie 80 zł z dnia 2018-10

Salda:
- 2018-01-01 - 2018-01-09: Wn 100 zł, Ma 0 zł
- 2018-01-10: Wn 20 zł, Ma 0 zł

#### Bez wyliczania salda

Zaległości nie są automatycznie pokrywane przez wpłaty. Opcja istnieje dla przypadków, gdy niezbędna jest informacja o całkowitym stanie zaległości (np o stanie funduszu remontowego).

Przykład:
- obciążenie w kwocie 100 zł z dnia 2018-01-01 z terminem na 2018-01-20
- wpłata w kwocie 80 zł z dnia 2018-10

Salda:
- 2018-01-01 - 2018-01-09: Wn 100 zł, Ma 0 zł
- 2018-01-10: Wn 100 zł, Ma 80 zł