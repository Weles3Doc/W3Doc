---
title: 6. Wysyłka faktur do KSeF
---

# Wysyłka faktur do KSeF

#### Ustawienie stawek

Aby wystawić `Faktury VAT` trzeba ustawić odpowiednie typy stawkom za pomocą:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj stawki`.
- Pole `Typ` > za wystawienie faktury odpowiadają typy:
    - `Brutto VAT (FV)`
    - `Netto VAT (FV)`
    - `ZW VAT (FV)`

Wszystkie trzy typy można używać w nieruchomościach vatowych, natomiast tylko `ZW VAT (FV)` używamy w przypadku podatników zwolnionych.

Co do zasady stawki staramy się ustawiać na strukturach, unikamy stawek na lokalach - przykład ustawienia stawek na lokalach użytkowych:

![Stawki LU](stawki-lu-01.png)

Przy powyższym ustawieniu lokalom użytkowym zostaną wystawione faktury do `KSeF` za media, reszta opłat będzie wystawiona na typie dokumentu, który jest określony obok numeru lokalu.

![Stawki LU](stawki-lu-02.png)

Być może inne lokale lub struktury w zasobie, mogą wymagać ustawienia odpowiednich stawek. Prosimy sprawdzić każdą nieruchomość. Uzgodnić z odbiorcami, czy nie potrzebują faktur przez `KSeF`. (*Pożytki, opłaty za hale garażowe/miejsca postojowe, mieszkania gdzie jest prowadzona działalność gospodarcza, zasoby lokalowe miast i gmin, refakturowanie*)

![Stawki LU](stawki-lu-03.png)

Oczywiście stawki ustawiamy tylko raz, na początku, jeśli się nie zmieniają to w następnych miesiącach nie ma potrzeby wykonywania tych czynności jeszcze raz. Przy zmianach stawek związanych ze zmianą planu gospodarczego lub zmiany pod rozliczenia - koniecznie trzeba zadbać aby nowa wartość miała poprawny typ. Możesz włączyć ochronę przed wystawianiem innych dokumentów niż faktury, z konkretne opłaty dla odbiorców z NIP, w tym celu zapoznaj się z instrukcją: Algorytmy niesprzedażowe.

#### Sprawdzenie naliczeń

Opłaty dla lokali można sprawdzić jeszcze przed zaksiegowaniem.

- Zakładka `Administracja` > przycisk `Naliczenia`.

Prosimy postępować zgodnie z instrukcją: [Przeliczenie naliczeń](https://doc.weles3.pl/administracyjne/naliczenia/Naliczenie-i-sprawdzenie.html). Dodatkowo naliczenia możesz najpierw zaksięgować w wersji testowej systemu `Weles 3`. Pamiętaj, że przesłanych do `KSeF` faktur, nie można cofnąć lub zmienic, jedynie skorygować następną fakturą, stąd poprawność dokumentów jest bardzo ważna.

#### Wysyłka do KSeF

Wysyłka faktur do `KSeF` odbywa się automatycznie podczas księgowania należności za pomocą:

- Zakładka `Administracja` > menu `Zasoby` > `Księguj należności`

Do `KSeF` trafią systemowe dokumenty o nazwie `Faktura VAT` oraz tylko te z nich, które posiadają `NIP` nabywcy. W należnościach mogą znajdować się faktury dla osób fizycznych bez NIP - dla takich faktur nie ma obowiązku wysyłki do `KSeF`.

W oknie mamy nowe pole `Wyślij do KSeF`, a w nim 3 nowe opcje:

- `Wyślij do KSeF` > jeśli w księgowanych naliczeniach znajdują się `Faktury VAT` z uzupełnionym NIPem odbiorcy, system wyśle te faktury do `KseF`. Używamy **tylko i wyłącznie** przy pierwszym księgowaniu obciążenia. Jeśli z jakiegoś powodu wycofaliśmy naliczenia już raz przesłane do `KSeF`, przy ponownym ich księgowaniu używamy następnej pozycji: *Odtwórz z KSeF (nie wysyłaj)*.
- `Odtwórz z KSeF (nie wysyłaj)` > opcja ta służy do odtwarzania naliczeń, na przykład przy ponownym ich księgowaniu po wycofaniu lub odtwarzaniu naliczeń w zasobach przejętych przez Państwa w administrowanie/zarządzanie/księgowość w trakcie roku. System nie wysyła faktur w tym trybie - porównuje je dokumentami w `KSeF` - jeśli są zgodnie w 100%, księguje i nadaje im numery KSeFowe.
- `Naliczenia próbne (nie wysyłaj)` > opcja słuzy do próbnego księgowania naliczeń bez wysyłania ich do `KSeF`. Obciążenia księgują się klasycznie, ale mają pewne ograniczenia:
    - Na liście miesięcy są oznaczone na żółto.
    - W danej chwili może istnieć tylko jedno próbne księgowanie w zasobie.
    - Nazwy dokumentów mają przedrostek `Próba....`, np.: `Próba Faktura VAT 27/ZAL/26-03`.
    - Nie można przekierować wydruków z `Wydruki` > `Dokumenty` do wysyłki mailowej.
    
Dzięki próbnym księgowaniom mogą Państwo sprawdzić wygląd/wydruki, wartości i numerację dokumentów oraz ich wpływ na konta księgowe, co jest przydatne przy rozliczeniach. Tymczasowo obciążyć rozrachunki właścicieli lub sporządzić wydruki z zakładki `Osoby`, choć te można nawet robić bez księgowania. Próbne obciążenia można odksięgować przez `Cofanie naliczeń`.

Bardzo ważną zmianą, którą pociąga za sobą wprowadzenie `KSeF`, jest brak możliwości zmiany daty księgowania obciążenia.

- Pole `Data księgowania` > będzie miało zawsze ustawiony dzień dzisiejszy.

![Wyślij do KSeF](ksieg-nal-01.png)

#### Cofanie naliczeń a KSeF

**Odradzamy cofanie naliczeń**, które zawierają faktury przesłane do KSeF. System pozwala na ich cofanie, jednakże potencjalne problemy z ich odtworzeniem, mogą przewyższyć korzyści wynikające z cofania, lepiej wystawić korektę.

Po cofnięciu można wprowadzić poprawki niewpływające, na wystawione już `Faktury VAT`. Przy ponownym księgowaniu trzeba użyć: `Wyślij do KSeF` > `Odtwórz z KSeF (nie wysyłaj)`.

**Stanowczo nie radzimy cofania więcej niż jednego obciążenia na raz**.

#### Sprawdzenie przesłanych faktur

Jeśli nie wystąpi żaden błąd podczas przesyłania faktur, okno `Księguj należności` zamknie się tak jak zazwyczaj. Jednak nie oznacza to jeszcze przetworzenia faktur przez system `KSeF`. Przetworzenie i nadanie numerów może zająć chwilę, w zależności od obciążeń serwerów. A w przypadku czasowej niedostępności lub awarii `KSeF`, faktury mogą być wystawione w trybie offline: [Tryby szczególne wystawiania faktur](https://ksef.podatki.gov.pl/informacje-ogolne-ksef-20/tryby-szczegolne-wystawiania-faktur).

Aby odświeżyć połączenie z KSeF i jednocześnie pobrać/sprawdzić numery faktur, należy przejść jeszcze raz do:

- Zakładka `Administracja` > menu `Zasoby` > `Księguj należności`

Przy wchodzeniu do tego okna, system odpytuje serwery `KSeF` o stan przetworzenia dokumentów i ewentualne nadane numery elektroniczne. Nic w tym oknie nie wykonujemy, po 5 sekundach zamykamy. Następnie należy odświeżyć system:

- Menu `Funkcje` > `Odśwież`. (Skrót klawiszowy `F` > `R`)

Pierwszym, najszybszym miejscem w którym zobaczymy nadane numery KSeF, jest:

- Zakładka `Dekrety`.

Po wejściu do zakładki wybieramy dekret `NAL`. W kolumnie z numerem faktury powinien pojawić się numer `KSeF`. Przykład ponizej.

![Dekret z KSeF](dekrety-nal-ksef01.png)

Wizualizacje wystawionych faktur `KSeF` sprzedażowych można sprawdzić w:

- Zakładka `Zasoby` > memu `Funkcje` > `Integracja KSeF`.
- Zakładka `Faktury`.

![Podgląd faktur z KSeF](ksef-wystawione-fak01.png)

System pobiera `Urzędowe poświadczenie odbioru dokumentu elektronicznego KSeF`, które można sprawdzić w:

- Zakładka `Zasoby` > memu `Funkcje` > `Integracja KSeF`.
- Zakładka `UPO`.

![Urzędowe poświadczenie odbioru dokumentu elektronicznego KSeF](ksef-upo01.png)

Wizualizacje faktury `KSeF` można też sprawdzić w formie klasycznej, za pomocą:

- Menu `Funkcje` > `Wydruki` > zakładka `Dokumenty`.

Na fakturze wystawianej w trybie online, znajdzie się jeden kod QR - zapewniający dostęp do faktury i weryfikację danych na niej zawartych – z oznaczeniem numeru KSeF faktury.

Na fakturze wystawianej w trybie offline - niedostępność KSeF lub offline24 oraz na fakturze wystawionej w trybie awaryjnym udostępnianej nabywcy w sposób inny niż przy użyciu KSeF znajdą się dwa kody. Pierwszy z napisem „OFFLINE”, drugi z napisem „CERTYFIKAT”.

![Wydruk w PDF faktur z KSeF](ksef-wydruk-fv01.png)
