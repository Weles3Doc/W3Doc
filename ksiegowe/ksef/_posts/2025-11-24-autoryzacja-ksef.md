---
title: Autoryzacja KSeF
---

# Autoryzacja KSeF

**Instrukcja w przygotowaniu.**

Możliwe scenariusze autoryzacji Welesa w zależności jaka osoba była wpisana w sekcję C formularza `ZAW-FA`.

#### ZAW-FA - Członek Zarządu

W tym przypadku mamy trzy ścieżki postępowania - wybieramy jedną z nich w zależności kto jest wpisany w `ZAw-FA`.

#### 1. Podmiot gospodarczy / firma / osoba prawna.

Członek Zarządu, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na **firmę** administratora/księgową:

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Podmiotowi do wystawienia i przeglądania faktur`.
- Sekcja `Dane podmiotu uprawnianego` > uzupełniamy danymi **firmy** administratora/księgowej.
- Sekcja `Zakres uprawnień` > oznaczamy wszystkie pola wyboru:
    - `Wystawiania faktur` i `z prawem do dalszego przekazywania uprawnienia`.
    - `Przeglądania faktur` i `z prawem do dalszego przekazywania uprawnienia`.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

#### 2. Osoba fizyczna.

Członek Zarządu, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na **osobę fizyczną**, na przykład na samego administratora/księgową/pracownika:

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Osobie fizycznej do pracy z KSeF`.
- Sekcja `Dane osoby fizycznej` > uzupełniamy danymi **osoby fizycznej**.
- Sekcja `Zakres uprawnień` > oznaczamy pola wyboru:
    - `Wystawiania faktur`.
    - `Przeglądania faktur`.
    - Pozostałe pola > dla bezpieczeństwa, nie zaznaczamy.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

#### 3. Weles sp. z o.o. sp. k. (nie zalecamy)

Członek Zarządu, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na Weles sp. z o.o. sp. k. NIP 1231399770.

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Podmiotowi do wystawienia i przeglądania faktur`.
- Sekcja `Dane podmiotu uprawnianego` > uzupełniamy danymi Weles.
    - Pole `NIP` > 1231399770.
    - Pole `Pełna nazwa` > WELES SPÓŁKA Z OGRANICZONĄ ODPOWIEDZIALNOŚCIĄ SPÓŁKA KOMANDYTOWA.
- Sekcja `Zakres uprawnień` > oznaczamy pola wyboru:
    - `Wystawiania faktur`.
    - `Przeglądania faktur`
    - W obu przypadkach **nie zaznaczamy** > `z prawem do dalszego przekazywania uprawnienia`.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

#### ZAW-FA - Osoba fizyczna lub podmiot gospodarczy / firma.

Osoba fizyczna lub firma, po zalogowaniu do [MCU](https://mcu.mf.gov.pl/web/login) na kontekst (NIP) wspólnoty, nadaje uprawnienia na Weles sp. z o.o. sp. k. NIP 1231399770.

- Zakładka `Uprawnienia` > `Nadaj uprawnienie`.
- Pole `Rodzaj uprawnienia` > `Podmiotowi do wystawienia i przeglądania faktur`.
- Sekcja `Dane podmiotu uprawnianego` > uzupełniamy danymi Weles.
    - Pole `NIP` > 1231399770.
    - Pole `Pełna nazwa` > WELES SPÓŁKA Z OGRANICZONĄ ODPOWIEDZIALNOŚCIĄ SPÓŁKA KOMANDYTOWA.
- Sekcja `Zakres uprawnień` > oznaczamy pola wyboru:
    - `Wystawiania faktur`.
    - `Przeglądania faktur`
    - W obu przypadkach **nie zaznaczamy** > `z prawem do dalszego przekazywania uprawnienia`.
- Kliknąć `Nadaj uprawnienia` > dalej postępuje zgodnie z instrukcjami na ekranie.

W ZAW-FA jest administrator lub administrator ma nadane uprawnienia przez zarząd (zarówno os. fiz, jak i firma)

Administrator (jeżeli jest uprawniany po NIP) musi nadać uprawnienia przynajmniej jednej osobie "Osobie fizycznej do pracy dla wszystkich klientów". Wtedy ta osoba będzie mogła składać podpisy dla Weles w EPUAP.