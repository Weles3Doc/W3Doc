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
- Konta zwykłe > obsługujemy większość banków (banki spółdzielcze nie są obsługiwane).
- Konta biznesowe i korporacyjne > potwierdziliśmy i przetestowaliśmy, że konta ING i Alior dla części korporacyjnej i biznesowej działają poprawnie. Prace nad uruchomieniem usługi dla PKO BP i mBank trwają. Mogą Państwo sprawdzić działanie dla innych banków. Jeśli będzie problem z pozyskaniem dany z rachunku lub zalogowaniem się, to prosimy o kontakt mailowy, wyślemy do banku prośbę o naprawę połączenia.

***

## 1. Autoryzacja dostępu do banku

##### 1.1 Zakładka Import.

Aby rozpocząć autoryzację do banku, należy przejść do:

- Menu `Funkcje` > `Importuj wyciągi elektroniczne` > zakładka `Import`.
- Kliknąć przycisk: `Autoryzacja dostępu do banku`.

![Autoryzacja dostępu](autowb01.png)

##### 1.2 Link do autoryzacji.

W oknie pojawi się komunikat z widocznym linkiem do rozpoczęcia autoryzacji. Należy go otworzyć w nowej karcie przeglądarki lub przekazać osobie, która ma dostęp/uprawnienia do konta bankowego. Autoryzacja nie musi być przeprowadzana na tym samym komputerze. 

![Autoryzacja dostępu](autowb02.png)

##### 1.3 Rozpocznij weryfikację.

Aby rozpocząć proces kliknij "Zezwól".

![Autoryzacja dostępu](autowb03.png)

##### 1.4 Udziel zgody.

Prosimy zapoznać się z udzielanymi zgodami i regulaminem. Zaznaczyć checkboxy i następnie kliknąć przycisk "Zezwól".

![Autoryzacja dostępu](autowb04.png)

##### 1.5 Wybierz typ konta.

Wybierz jeden z typów kont, właściwy dla dodawanego rachunku bankowego.

![Autoryzacja dostępu](autowb05.png)

##### 1.6 Wybierz bank.

Wybierz właściwy bank z listy. Jeśli Twój bank nie znajduje się na liście, powiadom dział wsparcia Weles3, sprawdzimy, co da się z tym zrobić.

![Autoryzacja dostępu](autowb06.png)

##### 1.7 Przejdź na stronę banku.

Kliknij przycisk "Przejdź na stronę banku", aby zostać przekierowany do wybranego banku w celu dokonania autoryzacji.

![Autoryzacja dostępu](autowb07.png)

##### 1.8 Zaloguj się do banku.

Następnie należy się zalogować do strony banku. 

![Autoryzacja dostępu](autowb08.png)

##### 1.9 Udziel zgody.

Bank może poprosić o zaznaczenie, dla których rachunków bankowych udzielamy zgód na przekazanie informacji o operacjach bankowych, zaznaczamy właściwe.

![Autoryzacja dostępu](autowb09.png)

##### 1.10 Potwierdź zgody zgodnie z wymaganiami banku.

Bank może wymusić dodatkowe potwierdzenie operacji udzielania zgód, za pomocą dodatkowych środków, np. za pomocą SMS lub aplikacji bankowej na telefonie.

![Autoryzacja dostępu](autowb10.png)

##### 1.11 Potwierdzenie udzielenia zgód.

Na stronie banku może zostać wyświetlone potwierdzenie udzielania zgód informacyjnych.

![Autoryzacja dostępu](autowb11.png)

##### 1.12 Weryfikacja przez Transactionlink.

W tym momencie autoryzacja jest przetwarzana i weryfikowana przez zewnętrznego dostawcę, może to potrwać kilka sekund.

![Autoryzacja dostępu](autowb12.png)

##### 1.13 Weryfikacja zakończona.

Gdy weryfikacja przebiegnie pomyślnie, wyświetli się poniższy komunikat. Zakładkę, w której dokonano autoryzacji, można zamknąć i wrócić do systemu Weles3.

![Autoryzacja dostępu](autowb13.png)

##### 1.14 Zakładka Import z podłączonym kontem.

Gdy autoryzacja przebiegnie pomyślnie, połączony rachunek bankowy zostanie wyświetlony na liście w zakładce `Import`. Według powyższej instrukcji należy autoryzować każdy rachunek bankowy, dla którego wyciągi będą pobierane automatycznie.

![Autoryzacja dostępu](autowb14.png)

***

## 2. Import operacji

Import operacji jest bardzo podobny do klasycznego, z tym że pomijamy całkowicie logowanie się do banku oraz generowanie i pobieranie wyciągu bankowego. 

##### 2.1 Pobranie operacji

Import zaczynamy od przejścia do:

- Menu `Funkcje` > `Importuj wyciągi elektroniczne` > zakładka `Import`.
- Kliknąć przycisk: `Analizuj z banku`. 

![Import automatyczny](autoimpwb01.png)

##### 2.2 Import

W tym momencie są możliwe dwie sytuacje:

- Jeśli wszystkie operacje mają przypisane konta księgowe, importowany wyciąg będzie miał status `Poprawne pliki`. Po kliknięciu na wyciąg będzie można sprawdzić jego zawartość, poprawne pozycje będą zaznaczone na zielono. Pole `Hasło` oraz przycisk `Importuj poprawne` są aktywne, można od razu przeprowadzić import.
- Natomiast jeśli w pobranych operacjach bankowych trafi się nowa operacja, która nie była wcześniej importowana, to wyciąg będzie miał status `Błędne pliki`. Po kliknięciu na wyciąg można sprawdzić jego zawartość, błędne pozycje będą zaznaczone na czerwono. Import takiego wyciągu nie jest możliwy, aby go zaimportować, należy podjąć dodatkowy krok, trzeba stworzyć przypisanie numeru konta bankowego do konta księgowego. W tym celu należy kliknąć przycisk `Powrót` i przejść do zakładki `Przypisanie kont`.

![Import automatyczny](autoimpwb02.png)

##### 2.3 Przypisanie kont

W zakładce `Przypisanie kont`, w polu `Rachunek bankowy` wybieramy wspólnotę i rachunek, dla którego występowały błędy podczas importu. W dolnej części okna załaduje się zestawienie rachunków oraz przypisanych im kont księgowych. Dla pozycji, które mają:

```
--- BRAK ---
--- BRAK ---
```

Należy określić konto księgowe, w tym celu klikamy:

- Po prawej stronie pozycji na ikonę rysika ![Rysik](rysik.png), pozycja załaduje się do górnej części okna.
- Pole `Nazwa podmiotu` > będzie uzupełnione danymi nadawcy/odbiorcy przelewu.
- Pole `Treść` > będzie uzupełnione tytułem przelewu, można zmienić na własny opis.
- Pole `Rachunek podmiotu` > pomijamy.
- Pole `Konto FK` > na podstawie wcześniejszych pól ustawiamy konto księgowe właściciela lub kontrahenta, ew. inne dowolne np. `2xx-.. Pozycje do wyjaśnienia`.
- Pole `Konto FK zapłat` > podajemy tutaj konto do zapłat, jeżeli mają być one księgowane na innym koncie niż w polu `Konto FK`, można w ten sposób rozdzielić wpłaty i zapłaty. Może pozostać puste: `BRAK`.
- Kliknąć: `Dodaj`.

Powyższe czynności powtarzamy dla każdego rachunku obcego, który nie ma przypisanego konta księgowego. Gdy pozycje będą uzupełnione, należy:

- Kliknąć: `Zatwierdź`.

Cały ten profes został przedstawiony na obrazku poniżej.

![Import automatyczny](autoimpwb03.png)

##### 2.4 Import

Po przypisaniu wszystkich operacji do kont księgowych wracamy do zakładki `Import`, następnie jeszcze raz klikamy `Analizuj z banku`. Importowany wyciąg będzie miał status `Poprawne pliki`. Po kliknięciu na wyciąg będzie można sprawdzić jego zawartość, poprawne pozycje będą zaznaczone na zielono. Pole `Hasło` oraz przycisk `Importuj poprawne` są aktywne, można od razu przeprowadzić import. W zakładce `Dekrety` zostaną utworzone adekwatne dokumenty WB na każdy dzień osobno, w którym występuje operacja bankowa.

![Import automatyczny](autoimpwb04.png)