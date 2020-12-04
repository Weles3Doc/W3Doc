---
title: 1. Utworzenie płatności masowych
---

# Utworzenie płatności masowych

Do uruchomienia usługi płatności masowych w systemie Weles3, konieczne jest podpisanie odpowiedniej umowy z bankiem. Na załączniku do umowy powinna znajdować się informacja na temat struktury numeracji rachunków wirtualnych. Po otrzymaniu takiej informacji wygenerujemy indywidualne numery kont bankowych właścicielom. 

Postać rachunku wirtualnego

Obsługa płatności w Systemie Identyfikacji Masowych Płatności odbywa się w oparciu o standardowy numer rachunku bankowego (IBAN). Sposób budowy numeru rachunku wirtualnego został przedstawiony poniżej:

![Struktura SWRK](strukturaswrk.png)

Objaśnienia:

- A — liczba kontrolna — jest wyliczana indywidualnie do każdego numeru konta (przez system).
- B — numer rozliczeniowy jednostki banku — 8-cyfrowy identyfikator banku i oddziału.
- C — kod Klienta banku.
- D — identyfikator dodatkowy — (nieruchomości, rachunku), np. gdy umowa z bankiem podpisana jest z zarządcą, który posiada kilka nieruchomości, lub gdy księgowość prowadzona jest na dwóch rachunkach (np. z podziałem na tzw. zaliczkę i fundusz remontowy). Jeśli identyfikator dodatkowy nie występuje, D staje się rozszerzeniem E.
- E – identyfikator dłużnika/płatności/kontrahenta.

Aby założyć płatności w systemie, trzeba przesłać do działu wsparcia, części numeru oznaczone jako B i C.  (+ewentualnie D)

Przykład załącznika do umowy poniżej, informacje istotne zaznaczone na żółto:

![Załącznik SWRK](zaloncznikswrk.png)

### Uwagi:

- Prosimy nie przysyłać nam skanów umów z bankiem — wystarczy załącznik ze strukturą lub wypisana sama struktura w mailu, w postaci:
  - cc 1234  5678  9012  XXXX  XXXX  XXXX

- Jeśli WM posiada dwa rachunki bankowe, dla których będą tworzone oddzielne płatności masowe, to załączniki prosimy opisywać np. bieżące i FR.
- W systemie Weles 3 numeracja rachunków wirtualnych opiera się o numer kartoteki konta 201 właściciela — dzięki temu jest on unikalny.
- Nowemu właścicielowi jest generowany nowy, unikalny numer rachunku indywidualnego w momencie dodawania go do systemu.
- Nie stosujemy i stanowczo odradzamy prowadzenie numeracji w oparciu o numer lokalu.
- Jest możliwość importu już wygenerowanych/używanych wcześniej numerów rachunków — w tym celu prosimy nam przesłać zestawienie w arkuszu, zawierające kolumny: [nr lokalu] [nr konta ind].
- Na wydruku opłat za lokal — numer konta podajemy, dodając wydruk: Wykaz do zapłaty.
- Jest możliwość sporządzenia zbiorczego zestawienia rachunków wirtualnych, robimy to za pomocą: Menu Funkcje > Wydruki > Zasób > Lista kont indywidualnych.