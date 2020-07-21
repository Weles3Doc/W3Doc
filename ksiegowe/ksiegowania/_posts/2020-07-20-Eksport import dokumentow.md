---
title: Eksport Import dokumentów
---
# Eksport/Import dokumentów

Funkcja eksportu umożliwia uzyskanie z systemu dekretów w formacie CSV. Mając taki plik, można go dowolnie edytować, a następnie korzystając z funkcji Importu, wprowadzić do systemu. Narzędzie jest przydatne zwłaszcza przy wprowadzaniu powtarzających się cyklicznie operacji (np. Faktur kosztowych lub dekretów PK).

### Eksport dokumentu

- Aby wyeksportować dany dokument z systemu, należy skorzystać z zakładki Dekrety. 

![Eksport import dokumentów](ekspimpdok1.png)

- Tam należy wybrać żądany dokument poprzez kliknięcie wskaźnikiem myszy i następnie przejść do pozycji Export. 

![Eksport import dokumentów](ekspimpdok2.png)

- W ramce z prawej strony klikamy na dowolną pozycję i wciskamy na klawiaturze klawisz z kropką. Potwierdzeniem działania będzie pojawienie się komunikatu o dokumencie do pobrania.

![Eksport import dokumentów](ekspimpdok3.png)

### Przygotowanie danych

Na poniższych obrazkach pokazujemy, jak powinien wyglądać plik przygotowany do importu. Można także posłużyć się wyeksportowanym dokumentem jak szablonem i uzupełnić/zmienić go wg własnych potrzeb. Nazwy pól w niniejszym opisie są zgodne z nazwami dostępnymi w oknie dodawania dokumentu (menu Dokumenty -> Dodaj dokument).

- Prezentowany w przykładzie dokument, to PK z dwoma pozycjami na łączną kwotę 120 zł.

![Eksport import dokumentów](ekspimpdok4.png)

- Komórka A1 - nagłówek importowanego dekretu/dokumentu
  - Rozpoczyna się zawsze od frazy W3ImpDok. Następne są 3 pozycje oddzielone spacją:
  - Typ wprowadzanego dokumentu zgodny z nazwą podaną w polu Typ dokumentu FK, tutaj PK.
  - Data księgowania dokumentu, w systemie to pole Data księgowania — tutaj 2017-01-01.
  - Nazwa Dokumentu — w systemie to pole Opis dokumentu, tutaj Przeksięgowanie.
- Całość wygląda tak jak na obrazku poniżej:

![Eksport import dokumentów](ekspimpdok5.png)

- Kolumny z danymi poszczególnych pozycji dekretu/dokumentu:
  - Kolumna A to data księgowania danej pozycji, tutaj: 2017-01-01.
  - Kolumna B to termin płatności (wymagalności lub wpłaty) danej pozycji, tutaj: 2017-01-02.
  - Kolumna C to pole Treść, tutaj: Zwrot.
  - Kolumna D to pole Dowód, tutaj: PK.
  - Kolumna E to pole Konto Wn.
  - Kolumna F to pole Konto Ma.
  - Kolumna G to pole Wartość.
- Całość wygląda tak jak na obrazku poniżej:

![Eksport import dokumentów](ekspimpdok6.png)

Poniżej zostało pokazane jak podobny dokument, wyglądałby przy wprowadzaniu ręcznym za pomocą opcji z programu: menu Dokumenty > Edytuj dokument.

![Eksport import dokumentów](ekspimpdok7.png)

### Import dokumentu

Posiadając już przygotowany dokument, można go zaimportować do systemu, za pomocą narzędzia Importuj dane, znajdującego się w zakładce Dekrety i menu Funkcje. 

![Eksport import dokumentów](ekspimpdok8.png)

Import można wykonać na 2 sposoby:
- Wybierając plik (format CSV).

![Eksport import dokumentów](ekspimpdok9.png)

- Wkleić zawartość do pola Dane.

![Eksport import dokumentów](ekspimpdok10.png)

- Po imporcie możemy podejrzeć nasz dokument.

![Eksport import dokumentów](ekspimpdok11.png)

### Import sald właścicieli w Bilansie otwarcia (BO)

W bardzo podobny sposób można również zaimportować salda właścicieli do BO, aczkolwiek sama tabela jest już znacznie uproszczona. Składa się tylko z trzech kolumn.

![Eksport import dokumentów](ekspimpdok12.png)

- Pierwszy wiersz i jego oznaczenie:
  - Komórka A1 to fraza BO albo BO= (ze znakiem równości program najpierw usuwa istniejące BO i doda całkowicie nowe pozycje; bez znaku równości program po prostu doda kolejne pozycje do BO) i następnie numer konta, którym system domknie księgowanie dokumentu.
  - Komórka B1 to zawsze fraza TR jako treść.
  - Komórka C1 to zawsze fraza MIE jako mieszkanie.

- Kolumny i ich oznaczenia:
  - Kolumna A to saldo właściciela. Kwota z minusem będzie księgowana po stronie WN a kwota z plusem po stronie MA.
  - Kolumna B to oznaczenie, którego bilansu otwarcia dotyczy. Może być to BO czyli Bilans Otwarcia lub BOO, czyli Bilans Otwarcia — Odsetki.
  - Kolumna C to numer systemowy lokalu, następnie pionowa kreska, kolejna cyfra to numer podkonta właściciela, na które ma być zaksięgowana pozycja (zazwyczaj 1 = Rozrachunki, 2 = Media i eksploatacja, 3 = Fundusz remontowy itd.).

Tak wygląda zaimportowany przykładowy dokument z ustawieniami zaprezentowanymi powyżej.

![Eksport import dokumentów](ekspimpdok13.png)