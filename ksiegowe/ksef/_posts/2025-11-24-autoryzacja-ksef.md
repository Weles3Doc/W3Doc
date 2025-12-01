---
title: 3. Autoryzacja KSeF
---

# Autoryzacja KSeF

Testowanie integracji `KSeF` można zrobić w bazie testowej `Weles3`. Baza testowa Weles3 łączy się ze środowiskiem przedprodukcyjnym (Demo) KSef. Autoryzacja w bazie głównej Weles3 nie jest możliwa - ministerstwo nie udostępniło wersji produkcyjnej - (będzie od 1 lutego lub 1 kwietnia 2026).

Nie muszą mieć Państwo certyfikatów - przesyłanie i odbieranie faktur będzie się odbywało na certyfikacie firmowym firmy Weles. (Weles musi mieć uprawnienia w `MCU`, ale uwaga, jeśli nie ma ich nadanych, to przy wczytywaniu podpisanego pliku autoryzacyjnego nada sobie samodzielnie uprawnienia w kontekście wspólnoty. (o ile osoba podpisująca ma odpowiednie uprawnienia))

#### Testowanie

Testy KSeF robimy w wersji testowej Weles3.

Proszę zrobić świeżą kopię testową.
- Menu `Pomoc` > `Kopia testowa bazy`.

Proszę przejść do wersji testowej Weles3.
- Menu `Pomoc` > `Przełącz tryb testowy`.

Z racji tego, że są to czynności wykonywane w wersji testowej - autoryzacje mogą być utracone, poprzez nadpisanie wersji testowej. Na Państwa życzenie możemy zablokować robienie nowej kopii testowej. W takim przypadku prosimy o maila na adres firmowy.

#### Pobranie pliku

Aby pobrać plik autoryzacyjny, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Integracja KSeF`.
- Zaznaczyć zasób na liście. **Ważne**
- Kliknąć: `Pobierz plik do autoryzacji`.

Plik należy zapisać na komputerze i przesłać do osoby z odpowiednimi uprawnieniami.

![Autoryzacja plikiem](plik-aut01.gif)

#### Podpis cyfrowy pliku

Po przygotowaniu pliku XML. należy go podpisać cyfrowo. Plik należy przesłać do jednej z osób:

- Osobie podanej w formularzu `ZAW-FA` w sekcji C. (Najłatwiejszy sposób)
- Osobie wpisanej jako `Administrator` w `MCU`.
- Osobie/firmie, która ma odpowiednie uprawnienia w `MCU`, Są to:
    - `Podmiotowi do wystawienia i przeglądania faktur`.
    - `Wystawiania faktur` i `z prawem do dalszego przekazywania uprawnienia`.
    - `Przeglądania faktur` i `z prawem do dalszego przekazywania uprawnienia`.

Osoba lub firma do podpisania pliku xml możne wykorzystać:

[https://podpis.gov.pl/podpisz-dokument-elektronicznie/](https://podpis.gov.pl/podpisz-dokument-elektronicznie/)

Plik można podpisać za pomocą jednego ze sposobów:
- `Profil Zaufany (ePUAP)` > umożliwia podpisanie pliku, wykorzystywany przez osoby fizyczne.
- `Certyfikat kwalifikowany osoby fizycznej` > zawierający numer PESEL lub NIP osoby posiadającej uprawnienia do działania w imieniu zasobu.
- `Certyfikat kwalifikowany organizacji (tzw. pieczęć firmowa)` - dla firm, zawierający numer NIP.
- `Certyfikat KSeF` > wystawiany przez system KSeF. Certyfikat ten nie jest certyfikatem kwalifikowanym, ale jest honorowany w procesie uwierzytelniania. Certyfikat KSeF jest wyłącznie wykorzystywany na potrzeby systemu KSeF.

![Autoryzacja plikiem](plik-aut02.gif)

#### Import pliku

Aby zaimportować plik autoryzacyjny podpisany cyfrowo, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Integracja KSeF`.
- Zaznaczyć zasób na liście. **Ważne**
- Pole: `Podpisany plik` > wybrać plik z dysku.
- Kliknąć: `Wyślij podpisany plik`.

Jeśli wszystko będzie w porządku, obok autoryzowanego zasobu pojawi się data autoryzacji oraz zakres nadanych uprawnień w polach `Odbiór` i `Wysyłka`. Pliki autoryzacyjne są jednorazowe.

![Autoryzacja plikiem](plik-aut03.gif)