---
title: 2. Uprawnienia KSeF
---

# Uprawnienia KSeF

System Weles3 posiada swój własny certyfikat firmowy do obsługi `KSeF 2.0`. Aby móc wysyłać i odbierać faktury przez KSeF w Weles3, osoba uprawniona musi nadać uprawnienia systemowi Weles3 do dostępu do KSeF danej wspólnoty.

`Aplikacja Podatnika KSeF 2.0 - wersja produkcyjna` jest dostępna pod adresem:

- [https://ap.ksef.mf.gov.pl/web/](https://ap.ksef.mf.gov.pl/web/)

---

Autoryzacja jest bardzo prosta, wystarczy przekazać plik `xml` osobie wymienionej w `ZAW-FA`,w sekcji `C`, do podpisu cyfrowego. Osoba ta podpisuje plik i odsyła do użytkownika Weles3, który następnie importuje plik do systemu. Cały ten proces jest opisany w instrukcji:

- [Autoryzacja KSeF](https://doc.weles3.pl/ksiegowe/ksef/autoryzacja-ksef.html)

**Jeśli to zadziała, to nie trzeba sie zagłębiać w dalszą treść tej instrukcji.**

---

W przypadku gdy **Weles jest już wpisany w `KSeF`**, wtedy podmiot/osoba podpisująca plik `xml`, musi mieć możliwość zalogowania się do kontekstu wspólnoty, aby **potwierdzić prawo dostępu** do danej wspólnoty. Mogą to być podmiot/osoba, która posiada jeno z poniższych:

- Jest wpisana w `ZAW-FA` wspólnoty.
- Ma jakiekolwiek uprawnienia w `KSeF` w kontekście wspólnoty. Jest `Administratorem` lub ma jakiekolwiek uprawnienia w zakładce `Uprawnienia` > `Zarządzaj uprawnienia`.
- Ma uprawnienie `Osobie fizycznej do pracy dla klienta` lub `Osobie fizycznej do pracy dla wszystkich klientów` w **KSeF na kontekście Administratora** (np jest pracownikiem), oraz sam administrator w `KSeF` wspólnoty, ma nadane jakiekolwiek uprawnienie z rodzaju: `Podmiotowi do przeglądania i wystawiania faktur`.

---

W przypadku **braku uprawnień** w `KSeF` na kontekście wspólnoty dla Weles, nie trzeba tych uprawnień wpisywać ręcznie. Weles nada je sobie sam przy imporcie pliku `xml`, jeżeli podmiot/osoba podpisująca ma uprawnienia do nadawania uprawnień kolejnym podmiotom/osobom. Czyli jedno z poniższych:

- Jest wpisana w `ZAW-FA` wspólnoty.
- Ma uprawnienie do zarządzania uprawnieniami. Jest `Administratorem` w kontekście wspólnoty.
- Ma uprawnienie do zarządzania uprawnieniami w kontekście `KSeF` administratora i administrator ma nadane uprawnienie `Podmiotowi do przeglądania i wystawiania faktur` w kontekście wspólnoty, z możliwością dalszej delegacji tj. `z prawem do dalszego przekazywania uprawnienia`.

---

Finalnie, niezależnie od toku postępowania, w `KSeF` na **kontekście wspólnoty**, firmie Weles musi być nadany rodzaj uprawnień `Podmiotowi do wystawienia i przeglądania faktur`, bez `prawem do dalszego przekazywania uprawnienia`. To gwarantuje poprawną autoryzacje KSeF w Weles3 danej wspólnoty, opisaną w instrukcji: Autoryzacja KSeF.

#### Nadawanie uprawnień Weles w MCU

Osoba fizyczna lub firma, po zalogowaniu do [Aplikacja Podatnika KSeF 2.0](https://ap.ksef.mf.gov.pl/web/) na **kontekst (NIP) wspólnoty**, może nadać uprawnienia na Weles sp. z o.o. sp. k. NIP 1231399770.

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Podmiotowi do wystawienia i przeglądania faktur`.
- Sekcja `Dane podmiotu uprawnianego` > uzupełniamy danymi Weles.
    - Pole `NIP` > 1231399770.
    - Pole `Pełna nazwa` > WELES SPÓŁKA Z OGRANICZONĄ ODPOWIEDZIALNOŚCIĄ SPÓŁKA KOMANDYTOWA.
- Sekcja `Zakres uprawnień` > oznaczamy pola wyboru:
    - `Wystawiania faktur`.
    - `Przeglądania faktur`.
    - W obu przypadkach **nie zaznaczamy** > `z prawem do dalszego przekazywania uprawnienia`.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

Po udanym potwierdzeniu uprawnień, powinny one się znaleźć w zakładce `Zarządzaj uprawnieniami`.

![Weles1](mcu-upr-weles1.png)