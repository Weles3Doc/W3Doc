---
title: 3. Wysyłka e-mail - wysyłka dokumentu
---

# Wysyłka e-mail — wysyłka dokumentów

#### Stworzenie dokumentu do wysyłki

Wysyłanie wiadomości e-mail zaczynamy zawsze od stworzenia dokumentu, który będzie załącznikiem w wiadomości mailowej. Robimy to tak jak w przypadku zwyczajnych dokumentów:

- Zakładka `Administracja` > Menu `Funkcje` > `Wydruki`.
- Okno `Wydruki` > tworzymy dokument do rozesłania właścicielom.

Na liście właścicieli można określić, do kogo trafi wysyłka. **Zalecamy** też skorzystać z [Filtrów wydruków](https://doc.weles3.pl/ogolne/wydruki/Filtry-wydrukow.html).

Gdy dokument będzie już gotowy, przekierowujemy go do wysyłki:

- Menu `Funkcje` > wybieramy jedną z opcji:
    - `Przekaż do wysyłki (dane na dzień wysyłki)` > **nie zalecana**, wydruki dla właścicieli (PDFy) tworzą się w momencie wysyłania e-maila z systemu. Jeśli w systemie zaszły zmiany mające wpływ na zawartość wydruków, to zostaną one uwzględnione w wysyłanych wydrukach.
    - `Przekaż do wysyłki (dane na dzień wydruku)` > **zalecana**, wydruki dla właścicieli (PDFy) tworzą się w momencie klikania w tę opcję, pozostają niezmienne do czasu wyjścia wiadomości mailowej.

Zamykamy okno wydruków lub pozostawiamy otwarte. Po przekazaniu wydruków do wysyłki zalecamy też zapisanie ich jako plik PDF, klikając: `Podgląd wydruku`, dzięki temu będziemy mieli zapisaną kopię rozesłanych załączników. W tym momencie możemy też wygenerować dokumenty do przekazania inną drogą niż wysyłka mailowa, w filtrze `Dane kontaktowe` odwracamy zaznaczenie, w polu `Posiadanie` na `Nie posiada`, po kliknięciu `Podgląd wydruku` wygenerują się nam wydruki do rozniesienia do skrzynek lub wysłania drogą tradycyjną.

![Wysyłka e-mail](wysylkaemailwydruk.gif)

#### Wysyłka wiadomości e-mail

Przechodzimy do definiowania właściwej wysyłki, przechodzimy do:

- Zakładka `Administracja` > menu `Funkcje` > `Wysyłka e-mail`.
- W lewej stronie okna **klikamy** na wysyłkę `-- NOWY --`.

W środkowej części okna wyświetlą się parametry wydruków oraz lista właścicieli, dla których zostały one stworzone. Ustawienie mailingu robimy przez:

- Kliknięcie: `Edycja`.
- Pole `Wysyłka` > wybieramy `E-mail`.
- Pole `Nazwa wysyłki (tytuł e-mail)`> wpisujemy nazwę wysyłki, która będzie jednocześnie tytułem e-maila.
- Pole `Odpowiedz do` > pozostawiamy puste, jeśli chcemy, aby odpowiedzi właścicieli trafiały na tę samą skrzynkę, z której otrzymali wiadomość. Wpisując tutaj adres konkretnego pracownika, przekierujemy zapytania właścicieli na jego skrzynkę.
- Pole `Opóźnienie (godz.)` > pozostawiamy puste, jeśli opóźnienie wysyłki ma przyjąć wartość domyślną dla zasobu. Można podać własną wartość, na przykład od 0 do 4 godzin.
- Pole `Wyślij z` > pozostawiając `Domyślne`, powodujemy, że wiadomości e-mail zostaną wysłane z domyślnej skrzynki przypisanej do zasobu. Wybierając jedną z dostępnych na liście, możemy zadecydować na przykład, że sprawy księgowe lub windykacyjne będą wysyłane ze skrzynek mailowych do tego dedykowanych.
- Pole `Treść e-maila` > uzupełniamy zawartość wiadomości mailowej. Tytuły i treści e-maila możemy zapisać wcześniej jako szablon w menu `Funkcje` > `Treści na wydruku`.
- Pole `Pliki` > służy do załączania wspólnych załączników, które trafią jednakowe do wszystkich właścicieli w danej wysyłce.
- Klikamy: `Zapisz`.

Wysyłka zmieni tytuł, aby ją rozesłać, należy:

- Kliknąć: `Roześlij`.

Wysyłka zmieni grupę na `Zaplanowane`, obok nazwy zostanie określona data i godzina wysyłki. Wysyłkę można odwołać, klikając `Wstrzymaj rozsyłanie` oraz następnie usunąć, klikając `Usuń`.

Po prawej stronie okna, w polu `E-Mail` można wpisać swój mail, następnie kliknąć `Wyślij e-mail testowy`. Na wskazany adres zostanie wysłany przykład wiadomości, dzięki temu można sprawdzić treść, załącznik oraz czy ogólnie skrzynka jest poprawnie ustawiona.

Każdy z właścicieli otrzyma tylko swój załącznik. Wydruk do wysyłki tworzony jest w momencie faktycznej wysyłki, a nie w momencie jej definiowania. Jeżeli w międzyczasie dokonamy zmian w systemie, które wpłyną na wydruk, to może on ulec zmianie. Wysyłka zajdzie tylko dla właścicieli, którzy mają uzupełniony poprawnie adres e-mail w menu `Zasoby` > `Edytuj dane właścicieli` > Pole `E-mail`. Jeśli właściciel ma nie brać udziału w wysyłce, to jego adres należy usunąć z pola `E-mail` i wpisać w pole `Informacja`. Do wysyłki z programu nie można podpiąć zewnętrznych załączników.

![Wysyłka e-mail](wysylkaemail.gif)