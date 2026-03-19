---
title: Dodatkowe informacje
---

# Dodatkowe informacje

#### Struktura logiczna faktury FA(3)

Broszura opracowana przez Ministerstwo Finansów, opisująca strukturę pliku xml faktury elektronicznej w `KSeF`.

Plik: [Broszura informacyjna dotycząca struktury logicznej FA(3)](broszura-informacyjna-dotyczaca-struktury-fa-3.pdf)

#### Wystawianie i otrzymywanie faktur w KSeF

Podręcznik KSeF 2.0 opisujący wystawianie faktur, stworzony przez Ministerstwo Finansów.

Plik: [Podręcznik KSeF 2.0 Cz. II Wystawianie i otrzymywanie faktur w KSeF](podrecznik-ksef-20-cz-ii-wystawianie-i-otrzymywanie-faktur-w-ksef-20260209.pdf)

#### Tryby szczególne wystawiania faktur

Informacja ogólna od Ministerstwa Finansów na temat trybów wystawiania faktur.

Link: [https://ksef.podatki.gov.pl/informacje-ogolne-ksef-20/tryby-szczegolne-wystawiania-faktur](https://ksef.podatki.gov.pl/informacje-ogolne-ksef-20/tryby-szczegolne-wystawiania-faktur)

Plik: [Tryby wystawiania - tabela](tabela-tryby-wystawiania-faktur-24022026.pdf)

#### Latarnia KSeF

Latarnia KSeF to system informowania o awariach i planowanych niedostępnościach Krajowego Systemu e-Faktur, uruchomiony przez Ministerstwo Finansów. Dostarcza publiczne API oraz komunikaty o statusie działania KSeF.

Opis: [https://github.com/CIRFMF/ksef-latarnia/blob/main/README.md](https://github.com/CIRFMF/ksef-latarnia/blob/main/README.md)

Status: [https://api-latarnia.ksef.mf.gov.pl/status](https://api-latarnia.ksef.mf.gov.pl/status)

Komunikat: [https://api-latarnia.ksef.mf.gov.pl/messages](https://api-latarnia.ksef.mf.gov.pl/messages)

#### KSeF - wersja przedprodukcyjna (Demo)

Testowanie integracji `KSeF 2.0` można zrobić w bazie testowej Weles 3.

- Menu `Pomoc` > `Przełącz tryb testowy`.

Baza testowa Weles 3 łączy się z `KSeF 2.0 - wersja przedprodukcyjna (Demo)`.

W wersji testowej systemu musisz ponownie autoryzować zasoby.

Do środowiska przedprodukcyjnego, zalogujesz się za pomocą prawdziwych danych uwierzytelniających. Autoryzacje zasobów z wersji głównej Weles 3 obowiązują też w wersji testowej. Żadna z czynności nie niesie za sobą skutków prawnych. Dane w wersji demo będą okresowo usuwane. Aplikacja Podatnika w środowisku przedprodukcyjnym (Demo) daje możliwość wystawiania i otrzymywania faktur w warunkach zbliżonych do tych, które są w wersji produkcyjnej.

Zaloguj się na swój kontekst firmowy KSeF - wystaw fakturę na jedną lub klika wspólnot - w ten sposób przetestujesz odbieranie faktur w Weles 3.

Zaksięguj naliczenia w wersji testowej Weles 3, aby wystawić faktury do KSeF danej wspólnoty. Następnie zaloguj się na kontekst wspólnoty i sprawdź jak one wyglądają.

Link do logowania:

- [https://ap-demo.ksef.mf.gov.pl/web/](https://ap-demo.ksef.mf.gov.pl/web/)

#### KSeF - wersja testowa

Jeśli chcesz przetestować KSeF 2.0 korzystając jedynie z **fikcyjnych danych na fakturach** oraz **fikcyjnych danych uwierzytelniających** – użyj środowiska testowego KSeF. W środowisku testowym użytkownik może posługiwać się dowolnymi, fikcyjnymi danymi. Żadna z czynności nie niesie za sobą skutków prawnych. Dane w wersji testowej będą okresowo usuwane.

Weles 3 nie posiada połączenia do wersji testowej KSeF.

**Pamiętaj przechodząc do środowiska testowego posługuj się fikcyjnymi danymi.**

Link do strony logowania:

- [https://ap-test.ksef.mf.gov.pl/web/](https://ap-test.ksef.mf.gov.pl/web/)
