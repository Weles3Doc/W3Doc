---
title: Hurtowa poprawa numerów liczników
---

# Poprawa numerów liczników

Zdarza się, że w procesie zakładania budynku w systemie, numery liczników są pomijane lub nie są od razu dostępne. W takim wypadku liczniki są dodawane z numerami technicznymi. Takie numery można łatwo poprawić za pomocą importu z arkusza. Jeśli mają już Państwo gotowe zestawienie tabelaryczne, to można z niego skorzystać, trzeba je sprowadzić do formatu rozpoznawanego przez system, opisanego w dalszej części instrukcji. Takie zestawienie można też wygenerować z systemu, aby to zrobić, przechodzimy do:

- Zakładka `Administracja` > menu `Funkcje` > `Wydruki`.
- Zakładka `Zasób`.
- Dodajemy wydruk `Lista odczytywania liczników`.
- Pole `Typ` > `Lista importu`.
- Pole `Bez grup liczników` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Bez typów właścicieli` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Sortowanie` > pozostawiamy bez zmian lub wybieramy pozycje.
- Pole `Format` > `CSV (;) - Excel`.
- Klikamy: `Podgląd wydruku`.

Pobieramy plik i otwieramy go w arkuszu kalkulacyjnym, wybierając odpowiednie kodowanie znaków i separator.

![Poprawa numerów](listalicznikow.gif)

Takie zestawienie formatujemy do postaci tabelki, w której znajduje się trzy kolumny:

- `MIE` > wpisujemy numer lokalu (taki jak w systemie).
- `NR` > wpisujemy numer licznika w systemie.
- `NNR` > wpisujemy nowy numer licznika.

Formatowanie zestawienia otrzymanego z systemu przedstawiamy poniżej.

![Poprawa numerów](poprawanumerow2.gif)

Tak sformatowaną tabelkę kopiujemy (wraz z tytułami kolumn) i wklejamy w:

- Menu `Funkcje` > `Import danych` > `Pole dane`.
- Wpisujemy hasło i zatwierdzamy.

Okno powinno się zamknąć. Nowe numery powinny być od razu widoczne na licznikach. Czasami trzeba też odświeżyć okno: menu `Funkcje` > `Odśwież`.

![Poprawa numerów](poprawanumerow3.gif)

### Uwagi:

- Numer licznika może mieć 12 znaków.
- Jeśli wystąpi błąd podczas importu, proszę sprawdzić, czy pomiędzy arkuszem a systemem są zgodne numery lokali i liczników oraz ich typy.
- Przyczyną błędów może być też brak zer wiodących w numerach liczników lub niewidoczne spacje dodane w komórkach.