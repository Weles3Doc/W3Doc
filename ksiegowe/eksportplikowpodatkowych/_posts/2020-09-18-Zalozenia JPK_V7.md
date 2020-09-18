---
title: Założenia eksportu JPK_V7
---
# Zakres JPK_V7

Weles3 pozwala generować deklaracje JPK_V7M i JPK_V7K. Zgodnie z wymogami raportowymi system
pozwala generować:
- miesięczną ewidencję
  - sprzedaży VAT
    - z uwzględnieniem pozycji
      - LpSprzedazy, NrKontrahenta, NazwaKontrahenta
      - DowodSprzedazy, DataWystawienia, DataSprzedazy, TypDokumentu
      - TypDokumentu, MPP, KorektaPodstawyOpodt
      - GTU_12
      - K_10, K_13, K_15, K_16, K_17, K_18, K_19, K_20
    - bez pozycji
      - KodKrajuNadaniaTIN
      - GTU_01 - GTU_11, GTU_13
      - SW, EE, TP, TT_WNT, TT_D, MR_T, MR_UZ, I_42, I_63
      - B_SPV, B_SPV_DOSTAWA, B_SPV_POWIZJA
      - K_11, K_12, K_14, K_21 - K_36
      - SprzedazVAT_Marza
  - zakupu VAT
    - z uwzględnieniem pozycji
      - LpZakupu, NrDostawcy, NazwaDostawcy
      - DowodZakupu, DataZakupu, DokumentZakupu, MPP
      - K_40 - K_47
    - bez pozycji
      - DataWplywu, IMP, ZakupVAT_Marza
- okresową deklarację (miesięczną lub kwartalną)
  - z uwzględnieniem pozycji
    - P_10, P_13, P_15, P_16, P_17, P_18, P_19, P_20
    - P_37, P_38, P_39
    - P_40 - P_48
    - P_51, P_53, P_62, P_68, P_69
  - bez pozycji
    - P_11, P_12, P_14, P_21 - P_36
    - P_49, P_50
    - P_52, P_54 - P_61
    - P_63 - P_67

Specyfikacje pól wraz z komentarzami można poznać w [Broszurze informacyjnej MF](https://www.gov.pl/attachment/aa25bab7-1932-49b1-8b49-d84ffc90c665).

Pozycje nie uwzględniane w eksporcie są to pozycje, które, jak uważamy, leżą poza zakresem
obszaru zarządzania nieruchomościami. Jeżeli któraś z pomijanych pozycji będzie konieczna
dla Państwa działalności, [prosimy o kontakt](mailto:weles@e-adm.pl).

# Typy dokumentów VAT

Księgując dokumenty VATowe system pozwoli zaklasyfikować je do grup:
- Podzielona płatność
- Środki trwałe (dla zakupu na poczet środków trwałych)
- Proporcja VAT (dla faktur zakupu rozliczanych proporcją)
- Metoda kasowa (dla faktur zakupu z metoda kasową)

Można nie wskazać żadnej oraz wskazać wiele grup na raz.
System będzie odpowiednio klasyfikował te pozycje w pliku JPK_V7

# Niezbędne dane podatkowe

Do wypełnienia deklaracji niezbędne jest podanie danych podatkowych:
- NIP
- Urząd skarbowy
- Nazwa pełna
- Zaliczka (miesięcznie/kwartalnie)
- Mail (JPK_V7 wymaga podania adresu e-mail)
  
# Korekty związane z par. 89a ustawy o VAT

Par. 89a ust. 1 ustawy o VAT pozwala pomniejszyć __podstawę opdatkowania oraz podatek należny__ z tytułu faktury z tytułu dostawy towarów lub świadczenia usług na terytorium kraju w przypadku
wierzytelności, których nieściągalność została uprawdopodobniona. 

JPK_V7 wymaga odrębnego pokazania tego typu korekt.

Aby zrealizować korektę wynikającą z par. 89a ust. 1 ustawy o VAT należy w systemie wykonać
księgowanie:
- osobno dla każdej stawki VAT
  - __Konto odbiorcy__ Wn
    - ```ujemna``` kwota burtto
    - stawka VAT
    - ```ujemna``` wartość VAT
    - __opcja Korekta__: ```Korekta podstawy i VAT art. 89a ust. 1, 4```
- łącznie
  - __Konto odbiorcy__ Wn
    - ```dodatnia``` sumaryczna kwota brutto
    - stawka VAT ```ND```
    - __bez opcji Korekta__
  - __Konto rozrachunkowe korekt VAT 89a__ Ma
    - ```dodatnia``` sumaryczna kwota VAT
    - stawka VAT ```ND```
    - __bez opcji Korekta__

Par. 89a ust 4 ustawy o VAT wymaga powiększenia __podstawy opdatkowania oraz podatku należnego__
w przypadku gdy po złożeniu deklaracji podatkowej, w której dokonano korekty, o której mowa w
ust. 1, należność zastała uregulowana lub zbyta w jakiejkolwiek formie.

JPK_V7 wymaga odrębnego pokazania tego typu korekt.

Aby zrealizować korektę wynikającą z par. 89a ust. 4 ustawy o VAT należy w systemie wykonać
analogiczne księgowanie ale z przeciwnymi wartościami (wartości ujemne zamieniamy na dodatnie,
a dodatnie na ujemne)

# Korekty związane z par. 89b ustawy o VAT
 
Par. 89b. ust 1 ustawy o VAT wymaga zmniejszenia __podatku naliczonego__ w przypadku
nieuregulowania należności wynikającej z faktury dokumentującej dostawę towarów lub świadczenie
usług na terytorium kraju w terminie 90 dni od dnia upływu terminu jej płatności określonego
w umowie lub na fakturze.

JPK_V7 wymaga odrębnego pokazania tego typu korekt.

Aby zrealizować korektę wynikającą z par. 89a ust. 1 ustawy o VAT należy w systemie wykonać
księgowanie:
- osobno dla każdej stawki VAT
  - __Konto dostawcy__ Ma
    - ```zerowa``` kwota burtto
    - stawka VAT
    - ```ujemna``` wartość korekty VAT
    - __opcja Korekta__: ```Korekta VAT art. 89b ust. 1, 4```
- łącznie
  - __Konto rozrachunkowe korekt VAT 89b__ Wn
    - ```dodatnia``` sumaryczna kwota VAT
    - stawka VAT ```ND```
    - __bez opcji Korekta__

### Korekty związane z par. 91 (oraz par. 90a - 90c) ustawy o VAT

Par. 91 ustawy o VAT wymaga rozliczenia współczynnika proporcji VAT za ubiegły rok
w deklaracji składanej za pierwszy okres rozliczeniowy roku następującego po roku podatkowym,
za który dokonuje się korekty.

JPK_V7 wymaga odrębnego pokazania tego typu korekt osobno dla środków trwałcyh oraz pozostałych
towarów i usług.

Aby zrealizować korektę wynikającą z par. 91 ustawy o VAT należy w systemie wykonać księgowanie:
- osobno dla każdej stawki VAT
  - __Konto rozrachunkowe korekt VAT 89b__ Wn
    - kwota korekty VAT (```dodatnia``` lub ```ujemna```)
    - stawka VAT 
    - __kwota VAT równa wartości pozycji__
    - __opcja Korekta__: ```Korekta VAT art. 90a-90c oraz art. 91```

# Księgowanie deklaracji VAT

W momencie księgowania deklaracji na koncie rozrachunków publiczno-prawnych z tytułu VAT
kwotę deklaracji trzeba domknąć po drugiej stronie:
 - kontami VAT należnego (zakupu)
 - kontami VAT naliczonego (sprzedaży)
 - kontami korekt VAT
   - kontem rozrachunkowym korekt VAT 89a
   - kontem rozrachunkowym korekt VAT 89b
   - kontem rozrachunkowym korekt VAT 91
 - przychody/koszty operacyjne - w przypadku groszowych końcówek
