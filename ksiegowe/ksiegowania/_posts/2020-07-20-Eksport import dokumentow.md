---
title: Eksport Import dekretów
---

# Eksport/Import dekretów

Funkcja eksportu umożliwia uzyskanie z systemu dekretów w formacie CSV. Mając taki plik, można go dowolnie edytować, a następnie korzystając z funkcji Importu, wprowadzić do systemu. Narzędzie jest przydatne zwłaszcza przy wprowadzaniu powtarzających się cyklicznie operacji (np. Faktur kosztowych lub dekretów PK).

#### Eksport dekretu

Aby wyeksportować dany dekret z systemu, należy przejść do:

- Zakładki `Dekrety`.
- Po lewej stronie okna wybrać dekret.
- Przycisk: `Eksport`.
- Kliknąć tabelkę, która się wyświetli.
- Na klawiaturze nacisnąć klawisz [ . ] kropki.

Wyskoczy monit o pobranie pliku CSV, zapisujemy go lub otwieramy bezpośrednio. Separator: `Przecinek`, zestaw znaków `Unicode UTF-8`, sugerujemy też ustawienie `Identyfikacji liczb specjalnych`.

![Eksport dekretu](eksportdekretu.gif)

#### Przygotowanie tabelki do importu

Poniżej przedstawimy jak samodzielnie stworzyć tabelkę do importu. Można także posłużyć się wyeksportowanym dekretem jak szablonem i uzupełnić/zmienić go wg własnych potrzeb. Nazwy pól w niniejszym opisie są zgodne z nazwami dostępnymi w oknie dodawania dokumentu (menu `Dokumenty` > `Dodaj dokument`).

![Tabelka do importu](imporddekretowtabelka.png)

Tabela do importu księgowań składa się z jednego wiersza „nagłówka” oraz 7 kolumn z danymi. W tabelce nie łączymy komórek i nie używamy żadnego typu formatowania komórek.

**Nagłówek**

Cały nagłówek wpisujemy w jednej komórce, nad pierwszą kolumną z danymi pozycji. Nagłówek ma postać:

```
<W3ImpDok>_<Typ dokumentu>_<Data księgowania>_<Nazwa dokumentu>
```

Gdzie:
- `W3ImpDok` > nagłówek importu dokumentów.
- `Typ dokumentu` > wpisujemy: `PK`, `Faktury`, `WB`, `ODS`, `NAL`, `KW`.
- `Data księgowania` > w formacie `RRRR-MM-DD`.
- `Nazwa dokumentu` > nazwa dokumentu widoczna na liście dokumentów w zakładce `Dekrety`.
- `_` > spacja, każdy z tych członów jest oddzielony spacją, **są one bardzo istotne**.

Przykłady:

```
W3ImpDok PK 2017-04-01 Przeksięgowanie salda
W3ImpDok Faktury 2017-03-31 Koszty marzec 2017
W3ImpDok WB 2017-02-15 WB marzec FR
```

**Wiersze z pozycjami**

Kolumny nie mają tytułów, funkcja komórki jest określona przez jej pozycje w tabelce. Kolumny mają postać:

```
| <Data pozycji> | <Termin płatności> | <Treść> | <Dowód> | <Konto WN> | <Konto MA> | <Kwota> |
```

Gdzie:
- `Data pozycji` > data w formacie `RRRR-MM-DD`.
- `Termin płatności` > data w formacie `RRRR-MM-DD`.
- `Treść` > ogólna nazwa tytułu księgowania, dowolny tekst.
- `Dowód` > numer dowodu wew. lub numer dokumentu, faktury.
- `Konto WN` > podajemy numer konta, na którym pozycja ma być zaksięgowana po stronie WN.
- `Konto MA` > podajemy numer konta, na którym pozycja ma być zaksięgowana po stronie MA.
- `Kwota` > kwota pozycji, zaokrąglona do dwóch miejsc po przecinku.

Wyżej wymienione pozycje wpisujemy w oddzielne komórki w tym samym wierszu. Numery kont podajemy z myślnikami, tak jak widzimy to w planie kont w zakładce `Konta FK`. Przykład:

```
201-1-0000086-2
130-01
400-2-001-006
```

Dla kont właścicieli lokali jest możliwy inny sposób określana konta:

```
<Numer lokalu>|<Numer podkonta>
```

Gdzie:
- `Numer lokalu` > taki jak w Weles3.
- `|` > klawisz pionowej kreski, oddziela te dwa człony.
- `Numer podkonta` > numer podkonta rozrachunkowego (zazwyczaj 1 , 2, 3 itd. do 9).

Przykład: `M01|1` `M01|2` `M01|3`.

**Przykłady gotowych tabelek**

![Tabelka do importu](imporddekretowtabelkaprzyklady.png)

#### Import dekretu

Gdy tabelka jest już gotowa, można ją zaimportować. Aby to zrobić, należy:

- W arkuszu kalkulacyjnym zaznaczyć i skopiować całą tabelkę.
- Menu `Funkcje` > `Import danych`.
- Pole `Dane` > wklejamy tabelkę.
- Pole `Hasło` > wpisujemy hasło.
- Klikamy: `Zatwierdź`.

Suma obrotów kont po stronie Wn i Ma musi być równa w importowanym dekrecie, bez tego system zgłosi błąd.

![Import dekretu](importdekretu.gif)