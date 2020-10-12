---
title: Edycja danych właścicieli
---

# Edycja danych właścicieli

System pozwala na gromadzenie i przechowywanie użytecznych danych teleadresowych oraz dodatkowych informacji na temat właścicieli. Dane te są łatwo odstępne z poziomu zakładki `Administracja` > przycisk `Informacje`. Można też ich użyć przy wydrukach, wysyłce e-mail lub SMS. Poniżej przedstawiamy sposób edycji wraz z opisem, za co odpowiada każde z pól. Aby edytować dane właściciela, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj dane właścicieli`.
- Na liście z lewej strony okna zaznaczamy właściciela do edycji.
- Klikamy: `Edycja`.
- Pole `NIP` > jeśli właściciel/odbiorca jest firmą, to uzupełniamy NIP. Ewentualnie pole może pozostać puste. Jeśli dla zasobu jest generowany plik JPK, to NIPy nie mogą pozostać puste, firmom obowiązkowo podajemy NIP, zwykłym właścicielom można wpisać wartość 9999999999.
- Przycisk: `Pobierz z REGON` > gdy podaliśmy NIP to nazwę i adres można pobrać z bazy REGON.
- Pole `Nazwa` > wpisujemy imiona i nazwiska właścicieli, nazwę firmy. Nazwa ta będzie wyświetlana w systemie w oknie `Wydruki` i przy nazwie konta 201 w zakładce `Konta FK` oraz na niektórych wydrukach zbiorczych. Zgodnie z zasadami języka polskiego jako pierwsze piszemy imię, potem nazwisko.
- Pole `Klucz` > skrócona nazwa, dla właściciela może być to samo nazwisko, dla firmy krótka jej nazwa. Klucz jest wyświetlany w zakładce `Administracja` w polu `Struktura` przy numerze lokalu. Pojawia się na wybranych wydrukach, dodatkowo niektóre wydruki posiadają opcje segregowania po kluczu właściciela.
- Pole `Adres` > wpisujemy pełen adres właściciela (adresata). Adres ten pojawia się na każdym wydruku dla właściciela. Wpisujemy go w odpowiednim formacie:

```   
Jan Kowalski
ul. Przykładowa 13 m. 6
00-000 Warszawa

Czyli:

<nazwa lub osoba>
ul. <ulica> <nr budynku> m. <nr mieszkania>
<Kod pocztowy> <Miejscowość>
```

- Pole `Sprawdzaj strukturę` > sprawdzanie struktury adresu, musi on spełniać powyższe założenia. Jeśli nie spełni, to nie da się zaakceptować zmian. Poprawny adres wymagany jest przy wysyłce dokumentów przez usługę Poczty Polskiej Envelo. Ewentualnie można pominąć sprawdzanie.
- Pole `Informacje` > uzupełniamy dowolne informacje o właścicielu. Można je wydrukować za pomocą: `Wydruki` > `Zasób` > `Inf. osób/mieszkań`.
- Pole `Informacje na wydruku` > pole tekstowe, w którym można wpisać informacje, które następnie można wywołać przy wydrukach dokumentów dla właścicieli, dodając wydruk: `Informacje na wydruku`.
- Pole `E-mail` > podajemy adres poczty elektronicznej właściciela, który będzie wykorzystywany przy wysyłaniu wiadomości e-mail za pomocą systemu. Jeśli jest dwa lub więcej adresów, to każdy z nich wpisujemy w nowej linii. Na każdy podany adres trafi osobna wiadomość. Jeśli osoba nie wyraziła zgody na korespondencję elektroniczną, to adres e-mail należy wpisać w pole `Informacje`. W tej samej linii, po e-mailu można dodać krótki opis.
- Pole `Telefon` > podajemy numer telefonu, który będzie wykorzystywany przy wysyłaniu wiadomości SMS za pomocą systemu. Numer telefonu wpisujemy w formacie 123456789, bez myślników i kierunkowego +48. Najlepiej tylko numery komórkowe. Jeśli jest dwa lub więcej telefonów, to każdy z nich wpisujemy w nowej linii. Na każdy podany numer trafi osobna wiadomość SMS. Jeśli osoba nie wyraziła zgody na kontakt telefoniczny, to nr telefonu należy wpisać w pole `Informacje`.  W tej samej linii, po numerze można dodać krótki opis. W polu nie wpisujemy numerów zagranicznych.
- Klikamy: `Zapisz`.

![Dane właścicieli](danewlascicieli.gif)