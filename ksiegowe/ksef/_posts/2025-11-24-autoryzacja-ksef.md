---
title: 3. Autoryzacja KSeF
---

# Autoryzacja KSeF

Nie muszą mieć Państwo certyfikatów lub tokenów - przesyłanie i odbieranie faktur będzie się odbywało na certyfikacie firmy Weles. Weles musi mieć uprawnienia w `KSeF`, ale uwaga, jeśli nie ma ich nadanych, to przy wczytywaniu podpisanego pliku autoryzacyjnego, nada sobie samodzielnie uprawnienia w kontekście wspólnoty, o ile osoba podpisująca ma odpowiednie uprawnienia.

**[Opis uprawnień](https://doc.weles3.pl/ksiegowe/ksef/uprawnienia-ksef.html)**


#### Pobranie pliku

Aby pobrać plik autoryzacyjny, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Integracja KSeF`.
- Zaznaczyć zasób na liście. **Ważne**
- Kliknąć: `Pobierz plik do autoryzacji`.

Plik należy zapisać na komputerze i przesłać do osoby z odpowiednimi uprawnieniami. Pliki autoryzacyjne są jednorazowe oraz trzeba je podpisać i wgrać w ciągu 10 minut.

![Autoryzacja plikiem](plik-aut01.gif)

#### Podpis cyfrowy pliku

Po przygotowaniu pliku XML. Należy go podpisać cyfrowo. Plik należy przesłać do jednej z osób:

- Osobie podanej w formularzu `ZAW-FA` w sekcji C. (Najłatwiejszy sposób)
- Osobie wpisanej jako `Administrator` w `KSeF` wspólnoty.
- Osobie/firmie, która ma odpowiednie uprawnienia w `KSeF` wspólnoty, są to:
    - `Podmiotowi do wystawienia i przeglądania faktur`.
    - `Wystawiania faktur` i `z prawem do dalszego przekazywania uprawnienia`.
    - `Przeglądania faktur` i `z prawem do dalszego przekazywania uprawnienia`.

Osoba lub firma do podpisania pliku xml możne wykorzystać stronę rządową:

[https://podpis.gov.pl/podpisz-dokument-elektronicznie/](https://podpis.gov.pl/podpisz-dokument-elektronicznie/) (**Działa tylko dla osób fizycznych**)

Plik można podpisać za pomocą jednego ze sposobów:
- `Profil Zaufany (ePUAP)` > umożliwia podpisanie pliku, wykorzystywany przez osoby fizyczne.
- `Certyfikat kwalifikowany osoby fizycznej` > zawierający numer PESEL lub NIP osoby posiadającej uprawnienia do działania w imieniu zasobu.
- `Certyfikat kwalifikowany organizacji (tzw. pieczęć firmowa)` - dla firm, zawierający numer NIP.
- `Certyfikat KSeF` > wystawiany przez system KSeF. Certyfikat ten nie jest certyfikatem kwalifikowanym, ale jest honorowany w procesie uwierzytelniania. Certyfikat KSeF jest wyłącznie wykorzystywany na potrzeby systemu KSeF.

Do podpisania pliku można użyć innych programów/dostawców podpisów cyfrowych, ważne aby podczas podpisywania wybrać metodę: `XAdES otoczony`. Przykład:

![Xades otoczony](xades-otoczony.png)

Po podpisaniu, osoba podpisująca przekazuje plik do użytkownika Weles3 w celu importu do systemu. Plik powinien mieć rozszerzenie `xml`. Przykład nazwy:

- signed_PlikDoAutoryzacji_WIATRACZNA 1.**xml**

![Autoryzacja plikiem](plik-aut02.gif)

#### Import pliku

Aby zaimportować plik autoryzacyjny podpisany cyfrowo, należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Integracja KSeF`.
- Zaznaczyć zasób na liście. **Ważne**
- Pole: `Podpisany plik` > wybrać plik z dysku.
- Kliknąć: `Wyślij podpisany plik`.

Jeśli wszystko będzie w porządku, obok autoryzowanego zasobu pojawi się data autoryzacji oraz zakres nadanych uprawnień w polach `Odbiór` i `Wysyłka`.

![Autoryzacja plikiem](plik-aut03.gif)