---
title: Edycja kontrahentów
---

# Edycja kontrahentów

Kontrahenci to dostawcy mediów, usług oraz towarów na rzecz wspólnoty mieszankowej. Są oni wspólni dla wszystkich zasobów prowadzonych w danej bazie klienckiej, więc (zazwyczaj) wprowadzamy ich tylko raz. Wyjątkiem jest sytuacja w której w danym zasobie jeden dostawca prowadzi dwa rozrachunki z różnych tytułów z wspólnotą mieszkaniową, na przykład mamy dwie oddzielne umowy (których nie można połączyć) za które wspólnota musi robić dwa przelewy.

Konta kontrahentów znajdują się na koncie syntetycznym `202`. Struktura tego konta jest narzucona przez system i ma postać: `SSS-AAAAAAAAA`. Numeracja kont jest automatyczna, każdy kolejny kontrahent ma numer konta większy o jeden. Edycje tych kont prowadzimy przez niżej wymienioną funkcję.

#### Dodanie nowego kontrahenta

Aby dodać nowego kontrahenta, należy wykonać następujące czynności:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj Kontrahentów`.
- Kliknąć: `Nowy`.
- Pole `NIP` > podajemy NIP.
- Jeśli podamy NIP i klikniemy: `Pobierz z REGON`, system odszuka kontrahenta i uzupełni pola `Kontrahent` oraz `Adres`.
- Pole `Kontrahent` > podajemy nazwę kontrahenta.
- Pole `Klucz` > podajemy nazwę/skrót kontrahenta.
- Pole `Adres` > podajemy adres kontrahenta.
- Pole `Konto bankowe` > podajemy numer konta bankowego (lub pozostawiamy puste). W tym miejscu wpisujemy głowny numer, jeśli kontrahent dla każdego zasobu/umowy/rozrachunku nadaje inne, to takie indywidualne numery bankowe uzupełniamy w innym miejscu w systemie. W tym celu prosimy sprawdzić instrukcję: `Konta bankowe kontrahentów`. Konta podane w tym polu jest wykorzystywane w imporcie operacji bankowych oraz w eksporcie zapłat (zleceń przelewów za koszty).
- Pole `E-mail` > podajemy adres e-mail (lub pozostawiamy puste).
- Pole `Telefon` > podajemy numer telefonu (lub pozostawiamy puste).
- Kliknąć: `Utwórz`.

![Edycja kontrahentów](edycjakontahentow2.gif)

#### Edycja danych kontrahenta

Edytując dane kontrahentów prosimy zachować pewną ostrożność. Na przykład, raz wpisanego nipu nie zmieniamy ze względów podatkowych. Nie edytujemy też danych firmy radykalnie, niedopuszczalne jest zmienienie firmy A na firmę B. Aby edytować kontrahenta, należy wykonać następujące czynności:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj Kontrahentów`.
- Wybrać kontrahenta z listy.
- Kliknąć: `Edycja`.
- Pole `NIP` > jeśli trzeba, poprawiamy NIP.
- Jeśli podamy NIP i klikniemy: `Pobierz z REGON`, system odszuka kontrahenta i uzupełni pola `Kontrahent` oraz `Adres`.
- Pole `Kontrahent` > jeśli trzeba, poprawiamy nazwę kontrahenta.
- Pole `Klucz` > jeśli trzeba, poprawiamy nazwę/skrót kontrahenta.
- Pole `Adres` > jeśli trzeba, poprawiamy adres kontrahenta.
- Pole `Konto bankowe` > jeśli trzeba, poprawiamy numer konta bankowego (lub pozostawiamy puste).
- Pole `E-mail` > jeśli trzeba, poprawiamy adres e-mail (lub pozostawiamy puste).
- Pole `Telefon` > jeśli trzeba, poprawiamy numer telefonu (lub pozostawiamy puste).
- Kliknąć: `Zapisz`.

![Edycja kontrahentów](edycjakontahentow3.gif)

#### Usuwanie kontrahenta

Kontrahent nie może posiadać księgowań na swoim koncie `202`, aby móc go usunąć. Usuwanie jest bardzo proste, należy wykonać następujące czynności:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj Kontrahentów`.
- Wybrać kontrahenta z listy.
- Kliknąć: `Usuń`.

Kontrahent usunie się natychmiast.

![Edycja kontrahentów](edycjakontahentow4.gif)