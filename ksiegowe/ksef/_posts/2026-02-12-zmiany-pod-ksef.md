---
title: 5. Zmiany pod KSeF
---

# Zmiany pod KSeF

W tej instrukcji opiszemy Państwu funkcje powiązane z wystawianiem faktur do KSeF, które należy wykonać przed pierwszym zaksięgowaniem obciążeń, a tym samym wysłaniem potencjalnych faktur do KSeF.

#### Dane podatkowe

Dla każdego zasobu należy uzupełnić `Dane podatkowe` - będą one używane jako dane sprzedawcy na fakturach `KSeF`.

- Zakładka `Zasoby` > menu `Funkcje` > `Podatki` > zakładka `Dane podatkowe`.

Zmianę danych opisuje instrukcja: **[Dane podatkowe](https://doc.weles3.pl/ksiegowe/eksportplikowpodatkowych/Dane-podatkowe.html)**.

#### Edycja zasobów

W oknie:

- Zakładka `Zasoby` > menu `Zasoby` > `Edytuj zasoby`.

Krytyczną rolę odgrywa tutaj pole `NIP` zasobu - prosimy sprawdzić lub uzupełnić NIPy nieruchomości.

Dodaliśmy dwie istotnie zmiany definiujące wysyłkę faktur do kSeF:

- Pole `Opcje` > `Wyłączony KSeF` > zaznaczenie tej opcji powoduje wyłączenie wysyłki `Faktur VAT` do `KSeF`. Wyłączenie obostrzeń związanych z księgowaniem naliczeń w systemie powiązanych z `KSeF`. Nadal będzie można odbierać faktury kosztowe z KSeF.
- Pole `Miesiąc rozpoczęcia wysyłek do KSeF` > definiuje miesiąc od którego rozpocznie się wysyłka potencjalnych `Faktur VAT` do `KSeF`. Domyślnie jest od `2026-04`, można ją przesunąć maksymalnie do `2027-01`. Jeśli w KSeF znajdują się faktury elektroniczne sprzedażowe, to system `Weles 3` będzie wymuszał wysyłkę faktur do KSeF, niezależnie jaki miesiąc w tym polu ustawimy.

![Edytuj zasoby](ksef-edytuj-zasoby01.png)

#### Nazwy dokumentów

W oknie:

- Zakładka `Administracja` > menu `Elementy` > `Nazwy dokumentów`.

Należy zadbać, aby systemowe `Faktury VAT` nie kolidowały nazewnictwem i numeracją z innymi typami dokumentów.

Tutaj należy zaznaczyć że do `KSeF` trafią tylko i wyłącznie systemowe dokumenty o nazwie `Faktura VAT`.

Wielu naszych klientów wystawia `Rachunki` ze zmienioną nazwą na `Faktura` - takie dokumenty nie trafią do `KSeF`. Właśnie w tych przypadkach należy sprawdzić ustawienia, aby nie wystawić dwóch dokumentów z identycznymi nazwami i numerami. Słowo `VAT` z `Faktura VAT` można usunąć w zasobach nievatowych oraz ustawić inną numerację w polu `Numer` - na przykład numeracja: F/20{ROK}/{MC}/{NR} - więcej szczegółów znajduje się w instrukcji: **[Nazwy dokumentów](https://doc.weles3.pl/administracyjne/system/Nazwy-dokumentow.html)**.

Można też zmienić nazwę dokumentu `Rachunek` z powrotem na `Rachunek` lub `Nota` lub `Nota obciążeniowa`, aby móc wystawiać inne dokumenty niż faktury. (można ale nie zawsze trzeba)

Prosimy pamiętać, że zmiana zachodzi z momentem kliknięcia `Zatwierdź` - każde ksiegowanie po tym, będzie już z nowym nazewnictwem, trzeba dobrze zaplanować moment zmiany.

![Nazwy dokumentów](ksef-nazwy-doku01.png)

#### Dane odbiorców

W oknie:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj dane właścicieli`.

Należy dopilnować poprawności uzupełnienia danych odbiorców, którzy będą otrzymywać faktury.

- Pole `NIP` > należy uzupełnić poprawnym NIPem podatnika, pole jest obowiązkowe jeśli odbiorca ma otrzymać fakturę przez KSeF. Inaczej mówiąc, to te pole decyduje czy faktura trafi do KSeF. Z programu można też wystawiać faktury na osoby fizyczne, takich faktury nie trzeba przesyłać do KSeF, w takich przypadkach pole `NIP` może pozostać puste. Zmiana NIPu po wystawieniu faktury nie będzie możliwa.
- Pole `Nazwa` > uzupełniamy nazwą odbiorcy (nabywcy), 
- Pole `Adres` > uzupełniamy pełnym adresem odbiorcy (nabywcy) (nazwa, imiona i nazwiska; ulica/numer domu; kod pocztowy i miejscowość). Poprawa adresu na wystawionych już dokumentach nie będzie możliwa, zmiana jest możliwa tylko od przyszłych > pole `Sprawdzaj strukturę` > `Nie aktualizuj adresów w zaksięgowanych fakturach, Nie sprawdzaj struktury`.
- Pole `Informacje do wydruku` > w tym polu można dodać informacje, które dołączą się na fakturze KSeFowej jako informacje dodatkowe, można tutaj na przykład zawrzeć numery umów lub inne informacje, których odbiorca domaga się umieszczenia na fakturze.
- Pole `KSeF adres` > uzupełniamy tylko wtedy, gdy adres na fakturach KSeFowych ma być inny niż w polu `Adres`.
- Pole `KSeF kod kraju` > podajemy dwuliterowy kod kraju odbiorcy (np. DE, EN). Dla polskich NIPów pozostawiamy puste pole.
- Pole `Rola podmiotu trzeciego` > stosujemy w przypadku wystawiania faktur jednocześnie na nabywcę i odbiorcę:
    - `Brak` > brak innego odbiorcy.
    - `Rola 8 - JST odbiorca` > wybieramy w przypadku jednostek samorządu terytorialnego (`JST`). W przypadkach gdy nabywcą jest Miasto/Gmina, a odbiorcą jednostka podległa obsługująca zasoby miasta/gminy. Przykład: nabywcą jest `Miasto Stołeczne Warszawa`, a odbiorcami są `Zakłady Gospodarowania Nieruchomościami` w poszczególnych dzielnicach.
    - `Rola 2 - Odbiorca jednostka wewnętrzna` > (`JW`) wybieramy w przypadku zakładu (oddziału) osoby prawnej lub innej wyodrębnionej jednostki wewnętrznej podatnika. (przykład ZUS, NFZ)
- Pole `NIP lub IDwew` > dla `JST` podajemy NIP jednostki podległej, dla `JW` wpisujemy `NIP-IDwew` podany przez nabywcę, przykład: `123456789-12345`.
- Pole `Nazwa podmiotu trzeciego` > uzupełniamy nazwę podmiotu trzeciego.
- Pole `Adres podmiotu trzeciego` > uzupełniamy adres podmiotu trzeciego.

Powyższe dane powinien wskazać nabywca/odbiorca - jeśli tego nie zrobił, najlepiej wysłać zapytanie przed rozpoczęciem wysyłania faktur do `KSeF`.

![Dane odbiorcy](ksef-dane-odbiorcy01.png)