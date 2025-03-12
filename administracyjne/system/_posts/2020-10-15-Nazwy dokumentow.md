---
title: Nazwy dokumentów
---

# Nazwy dokumentów

Funkcja `Nazwy dokumentów` pozwala na zmianę tytułów oraz sposób numerowania dokumentów wystawianych z systemu. Rozróżniamy dwa miejsca, w których możemy zmienić nazwę dokumentów:

- Zakładka `Zasoby` > menu `Elementy` > `Nazwy dokumentów` — nazwa dokumentu będzie zmieniona **we wszystkich** nieruchomościach.
- Zakładka `Administracja` > menu `Elementy` > `Nazwy dokumentów` — nazwa dokumentu będzie zmieniona tylko **w wybranej** nieruchomości.

Domyślnie z systemu można wystawić numerowane dokumenty o nazwach:

- `Zawiadomienie` > zwyczajny dokument z opłatami.
- `Faktura VAT` > standardowa Faktura VAT.
- `Rachunek` > wydruk w formie podobnej do Faktury VAT tylko pozbawiony jest wyszczególnionych wartości VAT.

Najczęstszym przypadkiem zmiany nazwy dokumentu jest zmiana `Rachunku` na `Faktura` (bez VAT) lub na `Nota księgowa`. Proces ten opisujemy poniżej, aby zmienić nazwę, należy przejść do:

- Zakładka `Administracja` > menu `Elementy` > `Nazwy dokumentów`.
- Po prawej stronie pozycji `Rachunek` klikamy na ikonę ołówka, pozycja wczyta się w górnej części okna.
- Pole `Nazwa należności` > wpisujemy nazwę normalną dokumentu.
- Pole `Nazwa korekty` > wpisujemy nazwę dokumentu korygującego.
- Pole `Skrót należności` > wpisujemy skrót nazwy normalnego dokumentu.
- Pole `Skrót korekty` > wpisujemy skrót nazwy korekty.
- Pole `Numer` > ustawiamy wzór numeru dokumentu. **Uwaga!** nie zalecamy zmiany w tym polu. Sprawdź dalszą część instrukcji.
- Klikamy: `Dodaj`.
- Klikamy: `Zatwierdź`.

Zmiana nazwy i numeracji nie zmienia zaksiegowanych już dokumentów. Po kliknięciu `Zatwierdź` każdy nowo zaksięgowany dokument będzie już wg. nowych ustawień. Zmiana nie ma ram czasowych, na przykład, cofnięcie i ponownie zaksięgowanie naliczeń/korekt/rozliczeń spowoduje, że nazwy lub/i numery dokumentów zostaną nadane już nowym sposobem. Dlatego po zmianie nie sugerujemy cofać naliczeń. Jeśli chcemy zmienić nazewnictwo i numerację od nowego roku, to wstrzymujemy się z księgowaniami naliczeń za styczeń, do czasu zaksięgowania wszystkich rozliczeń i korekt za rok poprzedni. Dopiero po tym zmieniamy numerację.

#### Zmiana numeracji

Za zmianę wzoru numeru dokumentu odpowiada pole `Numer`. Określamy w nim układ parametrów numeru oraz znaków alfanumerycznych + znaki specjalne. Parametry które mozemy użyć w wzorze numeru podajemy poniżej:

- `{NR}` > numer w roku (numeracja łączna dokumentów i korekt).
- `{1R}` > numer w miesiącu (numeracja łączna dokumentów i korekt).
- `{2R}` > numer w roku (numeracja osobna dokumentów i korekt).
- `{3R}` > numer w miesiącu (numeracja osobna dokumentów i korekt).
- `{ROK}` > ostatnie 2 cyfry roku.
- `{TYP}` > ZAL/KOR.
- `{MC}` > miesiąc.

Powyższe zostaną zastąpione odpowiednią wartością, oprócz tego możemy stosować:

- Tekst > małe i duże litery.
- Cyfry.
- Znaki specjalne: `/ \ | - _ ( )` i inne.

Poniżej przedstawiamy zmianę nazwy dokumentu `Rachunek` na `Faktura`.

![Zmiana nazwy dokumentu](zmiananazwydokumentu.gif)