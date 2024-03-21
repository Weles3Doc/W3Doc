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

#### Ustawienie parametrów wysyłki

Przechodzimy do definiowania właściwej wysyłki, przechodzimy do:

- Zakładka `Administracja` > menu `Funkcje` > `Wysyłka e-mail`.
- Po lewej stronie okna **klikamy** na wysyłkę `-- NOWY --`.

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

Okno edycji zamknie się, a wysyłka zmieni tytuł na ustawiony. Mailing już gotowy, sposób rozesłania omówimy w następnym punkcie instrukcji.

![Wysyłka e-mail](wysylkaemail.gif)

#### Rozesłanie e-mail

Gdy mamy ustawione parametry wysyłki można ją rozesłać, aby to zrobić, należy kliknąć:

- Przycisk `Roześlij`.

Wysyłka zmieni grupę na `Zaplanowane`, obok nazwy zostanie określona data i godzina wysyłki. Wysyłkę można odwołać, klikając `Wstrzymaj rozsyłanie` oraz następnie usunąć, klikając `Usuń`. Wysyłka e-mail następuje w sesjach co 1 godzinę, o najbliższych równych godzinach. Każdy z właścicieli otrzyma tylko swój załącznik. Wysyłka zajdzie tylko dla właścicieli, którzy mają uzupełniony poprawnie adres e-mail w menu `Zasoby` > `Edytuj dane właścicieli` > Pole `E-mail`. Jeśli właściciel ma nie brać udziału w wysyłce, to jego adres należy usunąć z pola `E-mail` i wpisać w pole `Informacja`.

![Wysyłka e-mail](wysylkaemailrozeslanie.gif)

#### Dodatkowe opcje

- Po prawej stronie okna, w polu `E-Mail` można wpisać swój mail, następnie kliknąć `Wyślij e-mail testowy`. Na wskazany adres zostanie wysłany przykład wiadomości, dzięki temu można sprawdzić treść, załącznik oraz ogólne, czy skrzynka jest poprawnie ustawiona. Zalecamy to zrobić przed kliknięciem `Roześlij`.

- Przycisk `Podgląd wydruku e-mail` > pozwala na pobranie załączników z danej wysyłki.

- Przycisk `Edycja wydruku` > TBA

- Przycisk `Raport z wysyłki` > umożliwia pobranie PDF ze statusami wysyłek dla każdego właściciela.

- Przycisk `Ponów niezrealizowane` > gdy w wysyłce pojawią się błędy, np. błędny adres e-mail, to po ich poprawieniu, można ponowić wysyłkę bez potrzeby definiowania jej ponownie.