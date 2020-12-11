---
title: Baza testowa
---

# Baza testowa

#### Wykonanie kopii testowej

Baza testowa służy do sprawdzania rozwiązań w bezpieczny sposób na kopii rzeczywistych danych, aby wykonać świeżą kopię bazy testowej, należy przejść do:

- Menu `Pomoc` > `Kopia testowa bazy`.

Narzędzie te dostępne jest w każdej z zakładek systemu. Po poprawnym wykonaniu kopii system poinformuje nas komunikatem na zielonym tle (komunikat wyświetlany będzie przez ok. 2 sekundy).

![Wykonanie kopii testowej](wykonanie-kopi.gif)

#### Przechodzenie w tryb testowy bazy

W celu przełączenia się w tryb testowy należy przejść do: 

- Menu `Pomoc` > `Przełącz tryb testowy`.

Opcja ta jest dostępna w każdej z zakładek systemu. Po przełączeniu w tryb testowy system otworzy nową zakładkę. Przebywanie w trybie testowym jest oznaczone czerwoną etykietą `WERSJA TESTOWA`.

![Przejście do wersji testowej](przelaczenie-test.gif)

#### Zakończenie pracy w trybie testowym bazy

Aby zakończyć pracę w trybie testowym, wystarczy zamknąć kartę przeglądarki, w której znajduje się baza testowa.

#### Uwagi:

- Zmian wprowadzonych w bazie testowej nie przenosimy do bazy głównej (produkcyjnej).
- Aby móc skorzystać z bazy testowej należy uprzednio choć raz kiedykolwiek wykonać kopię bazy.
- Baza testowa nie aktualizuje się samodzielnie. Aby móc przeprowadzać testy na aktualnym stanie bazy głównej należy ponownie wykonać jej kopię.
- Na Państwa dyspozycję możemy tymczasowo zablokować wykonywanie kopii bazy testowej. Dzięki temu możliwe będzie przeprowadzenie złożonych testów bez ryzyka nadpisania Państwa bazy przez innych administratorów.
- Baza testowa jest w pełni funkcjonalna jak baza główna (z wyjątkiem: wysyłek / forum / ustawień uprawnień).