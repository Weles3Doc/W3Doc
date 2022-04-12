---
title: Automatyczne pobieranie wyciągów
---

# Automatyczne pobieranie wyciągów

## >>>>>>>> Instrukcja w przygotowaniu <<<<<<<<

## Wstęp

W systemie Weles3 udostępniliśmy Państwu nową funkcję, która pozwala na pobieranie operacji bankowych bez konieczności każdorazowego logowania się i pobierania plików wyciągów bankowych. Dzięki niej wystarczy jedno kliknięcie, aby pobrać pozycje do zaksięgowania w systemie. 

Usługa jest współrealizowana z naszym partnerem, firmą [Transactionlink sp. z o.o.](www.transactionlink.io), która jest wpisana do rejestru KNF jako dostawca świadczący wyłącznie usługę dostępu do informacji o rachunku (ang. Account Information Service Provider – AISP), to rozwiązanie wprowadzone jest nowelizacją ustawy o usługach płatniczych w związku ze wdrożeniem dyrektywy PSD2. Służy ono prowadzeniu działalności w zakresie świadczenia usług polegających na dostarczaniu posiadaczom rachunków płatniczych skonsolidowanych informacji o tych rachunkach.

Usługa jest dodatkowo płatna.

***

Wymagania początkowe:
- Każdy rachunek bankowy, dla którego będą pobierane operacje bankowe automatycznie, musi być dodany w:
    - Zakładka `Zasoby` > menu `Funkcje` > `Importuj wyciąg elektroniczny` > zakładka `Rachunki bankowe`.
- Saldo konta księgowego rachunku bankowego `13x` w programie Weles3 musi być zgodne ze saldem konta bankowego, aby import mógł się rozpocząć. Operacje bankowe będą importowane od ostatniego momentu (daty) dla którego salda Weles3 <-> Bank były zgodne.

Obsługiwane banki:
- Konta indywidualne > obsługujemy wszystkie banki.
- Konta biznesowe i korporacyjne > obecnie są obsługiwane ??????, pracujemy nad rozszerzeniem listy banków. Jeśli Państwa bankowe konto biznesowe lub korporacyjne nie znajduje się na liście, to prosimy o maila, sprawdzimy, co da się zrobić.

***

## Autoryzacja dostępu do banku

#### Zakładka Import.

Aby rozpocząć autoryzację do banku, należy przejść do:

- Menu `Funkcje` > Importuj wyciągi elektroniczne > zakładka `Import`.
- Kliknąć przycisk: `Autoryzacja dostępu do banku`.

![Autoryzacja dostępu](autowb01.png)

#### Link do autoryzacji.

W oknie pojawi się komunikat z widocznym linkiem do rozpoczęcia autoryzacji. Należy go otworzyć w nowej karcie przeglądarki lub przekazać osobie, która ma dostęp/uprawnienia do konta bankowego. Autoryzacja nie musi być przeprowadzana na tym samym komputerze. 

![Autoryzacja dostępu](autowb02.png)

#### Rozpocznij weryfikację.

Aby rozpocząć proces kliknij "Zezwól".

![Autoryzacja dostępu](autowb03.png)

#### Udziel zgody.

Prosimy zapoznać się z udzielanymi zgodami i regulaminem. Zaznaczyć checkboxy i następnie kliknąć przycisk "Zezwól".

![Autoryzacja dostępu](autowb04.png)

#### Wybierz typ konta.

Wybierz jeden z typów kont, właściwy dla dodawanego rachunku bankowego.

![Autoryzacja dostępu](autowb05.png)

#### Wybierz bank.

Wybierz właściwy bank z listy. Jeśli Twój bank nie znajduje się na liście, powiadom dział wsparcia Weles3, sprawdzimy, co da się z tym zrobić.

![Autoryzacja dostępu](autowb06.png)

#### Przejdź na stronę banku.

Kliknij przycisk "Przejdź na stronę banku", aby zostać przekierowany do wybranego banku w celu dokonania autoryzacji.

![Autoryzacja dostępu](autowb07.png)

#### Zaloguj się do banku.

Następnie należy się zalogować do strony banku. 

![Autoryzacja dostępu](autowb08.png)

#### Udziel zgody.

Bank może poprosić o zaznaczenie, dla których rachunków bankowych udzielamy zgód na przekazanie informacji o operacjach bankowych, zaznaczamy właściwe.

![Autoryzacja dostępu](autowb09.png)

#### Potwierdź zgody zgodnie z wymaganiami banku.

Bank może wymusić dodatkowe potwierdzenie operacji udzielania zgód, za pomocą dodatkowych środków, np. za pomocą SMS lub aplikacji bankowej na telefonie.

![Autoryzacja dostępu](autowb10.png)

#### Potwierdzenie udzielenia zgód.

Na stronie banku może zostać wyświetlone potwierdzenie udzielania zgód informacyjnych.

![Autoryzacja dostępu](autowb11.png)

#### Weryfikacja przez Transactionlink.

W tym momencie autoryzacja jest przetwarzana i weryfikowana przez zewnętrznego dostawcę, może to potrwać kilka sekund.

![Autoryzacja dostępu](autowb12.png)

#### Weryfikacja zakończona.

Gdy weryfikacja przebiegnie pomyślnie, wyświetli się poniższy komunikat. Zakładkę, w której dokonano autoryzacji, można zamknąć i wrócić do systemu Weles3.

![Autoryzacja dostępu](autowb13.png)

#### Zakładka Import z podłączonym kontem.

Gdy autoryzacja przebiegnie pomyślnie, połączony rachunek bankowy zostanie wyświetlony na liście w zakładce `Import`. Według powyższej instrukcji należy autoryzować każdy rachunek bankowy, dla którego wyciągi będą pobierane automatycznie.

![Autoryzacja dostępu](autowb14.png)

