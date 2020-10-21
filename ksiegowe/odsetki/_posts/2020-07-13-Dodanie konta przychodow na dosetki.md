---
title: 1. Dodanie konta przychodów na odsetki
---

# Dodanie konta przychodów na odsetki

Pierwszym krokiem przed naliczeniem odsetek jest dodanie konta przychów, na którym system będzie księgował je automatycznie. Aby to zrobić, należy przejść do:

- Zakładka `Zasoby` > menu `Plan kont` > `Plan kont`.
- Kliknąć: `Dodaj konto syntetyczne`.
- Pole `Numer` > podać numer konta syntetycznego, na przykład 720.
- Pole `Nazwa` > podać nazwę konta, na przykład: Odsetki naliczone od zaległości właścicieli.
- Pole `Analityka` > wpisać 11, co oznacza konto o poziomach SSS-x-z.
- Pole `Konto` > wybrać `Wynikowe`.
- Pole `Typ` > wybrać `Odsetki właścicieli`.
- Kliknąć: `Utwórz`.

![Konto przychodów na odsetki](7xxodsetki.gif)

#### Uwagi:

- Konto musi mieć analitykę równą 11.
- Konto musi mieć typ Odsetki właścicieli.
- Konta analityczne (podkonta) system stworzy automatycznie podczas księgowania pierwszych odsetek.
- Odsetki po stronie konta 201 są księgowane na tym samym koncie właściciela, na podstawie którego zostały naliczone.
- Odsetki po stronie przychodów 7xx są księgowane z podziałem na pod konta rozrachunkowe i opcjonalnie na typ właściciela (opcja do ustawienia w zakładka `Zasoby` > menu `Zasoby` > `Edytuj zasoby` > pole `Opcje` > `Rozszerzona analityka odsetek`.
- Konto dodajemy tylko raz. Jest ono wspólne dla wszystkich nieruchomości w systemie.