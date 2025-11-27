---
title: 2. Uprawnienia KSeF
---

# Uprawnienia KSeF

**Instrukcja w przygotowaniu.**

System Weles3 posiada swój własny certyfikat firmowy. Aby móc wysyłać i odbierać faktury przez KSeF w Weles3, osoba uprawniona w MCU musi nadać uprawnienia systemowi Weles3 do dostępu do KSeF danej wspólnoty.

`Moduł Certyfikatów i Uprawnień` jest dostępny pod adresem:

- [https://mcu.mf.gov.pl/web/login](https://mcu.mf.gov.pl/web/login)

Jest to rozwiązanie tymczasowe, będzie dostępny od końca stycznia 2026. Od 1 lutego 2026 jego rolę przejmie `Aplikacja Podatnika KSeF 2.0` (i `API KSef 2.0` w zintegrowanych systemach). Certyfikaty i upewnienia nadane w MCU nie stracą ważności przy tej zmianie. **[Podręcznik użytkownika MCU](https://ksef.podatki.gov.pl/media/0iafuqe5/podrecznik-uzytkownika-modulu-certyfikatow-i-uprawnien-mcu.pdf)**.

---

#### W najprostszym przypadku

Gdy w `ZAW-FA` jest podany Członek Zarządu wspólnoty, to on nadaje uprawnienia dla Weles w `MCU`.

Członek Zarządu, po zalogowaniu do `MCU` na kontekst (NIP) wspólnoty, nadaje uprawnienia na Weles sp. z o.o. sp. k. NIP 1231399770.

- Zalogować się > [https://mcu.mf.gov.pl/web/login](https://mcu.mf.gov.pl/web/login)
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

Po udzieleniu uprawnień, Członkowi Zarządu trzeba dostarczyć plik XML do podpisania - jest to opisane instrukcji [Autoryzacja KSeF](https://doc.weles3.pl/ksiegowe/ksef/autoryzacja-ksef.html).

---

#### Pozostałe przypadki

1. Firma Weles ma już nadane uprawnienia w MCU, wtedy podmiot/osoba podpisująca plik




Finalnie, niezależnie od toku postępowania, w `MCU` na **kontekście wspólnoty**, firmie Weles musi być nadany rodzaj uprawnień `Podmiotowi do wystawienia i przeglądania faktur`, bez `prawem do dalszego przekazywania uprawnienia`. To gwarantuje poprawną autoryzacje KSeF w Weles3 danej wspólnoty, opisaną w instrukcji: [Autoryzacja KSeF](https://doc.weles3.pl/ksiegowe/ksef/autoryzacja-ksef.html).

---

- [1. ZAW-FA - Członek Zarządu](#1-zaw-fa---członek-zarządu)
    - [1.1 Weles sp. z o.o. sp. k.](#11-weles-sp-z-oo-sp-k)
    - [1.2 Podmiot gospodarczy / firma / osoba prawna](#12-podmiot-gospodarczy--firma--osoba-prawna)
    - [1.3 Osoba fizyczna](#13-osoba-fizyczna)
- [2. ZAW-FA - Osoba fizyczna lub podmiot gospodarczy / firma](#2-zaw-fa---osoba-fizyczna-lub-podmiot-gospodarczy--firma)

Możliwe scenariusze nadawania uprawnień w `MCU` w zależności jaka osoba była wpisana w sekcję C formularza `ZAW-FA`.

### 1. ZAW-FA - Członek Zarządu

W tym przypadku mamy trzy ścieżki postępowania - wybieramy jedną z nich w zależności kogo chce autoryzować wspólnota mieszkaniowa.

#### 1.1 Weles sp. z o.o. sp. k.

Członek Zarządu, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na Weles **bezpośrednio**.

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

Po udzieleniu uprawnień, Członkowi Zarządu trzeba dostarczyć plik XML do podpisania - jest to opisane instrukcji [Autoryzacja KSeF](https://doc.weles3.pl/ksiegowe/ksef/autoryzacja-ksef.html).

#### 1.2 Podmiot gospodarczy / firma / osoba prawna

Członek Zarządu, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na **firmę** administratora/księgową:

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Podmiotowi do wystawienia i przeglądania faktur`.
- Sekcja `Dane podmiotu uprawnianego` > uzupełniamy danymi **firmy** administratora/księgowej (po NIP).
- Sekcja `Zakres uprawnień` > oznaczamy wszystkie pola wyboru:
    - `Wystawiania faktur` i `z prawem do dalszego przekazywania uprawnienia` **Ważne**.
    - `Przeglądania faktur` i `z prawem do dalszego przekazywania uprawnienia`**Ważne**.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

Nastepnie firma wchodzi na swój kontekst MCU i nadaje uprawnienia Weles.
Podmiotowi dla pracy dla klientów

#### 1.3 Osoba fizyczna

Członek Zarządu, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na **osobę fizyczną**, na przykład na samego administratora/księgową/pracownika:

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Osobie fizycznej do pracy z KSeF`.
- Sekcja `Dane osoby fizycznej` > uzupełniamy danymi **osoby fizycznej** (po PESEL).
- Sekcja `Zakres uprawnień` > oznaczamy pola wyboru:
    - `Wystawiania faktur`.
    - `Przeglądania faktur`.
    - Pozostałe pola > dla bezpieczeństwa, nie zaznaczamy lub wg własnego uznania.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

Następnie to samo co dla firmy

#### 2. ZAW-FA - Osoba fizyczna lub podmiot gospodarczy / firma

Osoba fizyczna lub firma, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na Weles sp. z o.o. sp. k. NIP 1231399770.

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

W ZAW-FA jest administrator lub administrator ma nadane uprawnienia przez zarząd (zarówno os. fiz, jak i firma)

Administrator (jeżeli jest uprawniany po NIP) musi nadać uprawnienia przynajmniej jednej osobie "Osobie fizycznej do pracy dla wszystkich klientów". Wtedy ta osoba będzie mogła składać podpisy dla Weles w EPUAP.

--->