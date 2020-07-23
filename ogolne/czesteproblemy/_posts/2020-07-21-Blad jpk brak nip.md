---
title: Błąd JPK brak NIPu
---
# Błąd JPK — brak NIP

Podczas generowania plików JPK możemy natrafić na błąd:

- ERR The 'http://jpk.mf.gov.pl/wzor/2017/11/13/1113/:NrKontrahenta' element is invalid

Przyczyny należy szukać w braku NIPu odbiorcy (właściciela) lub dostawcy (kontrahenta). Aby sprawdzić, komu brakuje numeru NIP, należy:

- Zamknąć komunikat o błędzie.
- W polu Weryfikacja schematu ustawić Nie weryfikuj.
- W polu Akcja wybrać Podgląd.
- Kliknąć: Pobierz.
- Otworzy się nowa zakładka z podglądem pozycji, lokalizujemy w niej odbiorców/dostawców, którzy nie mają numeru w kolumnie NIP.

Aby poprawić lub dodać NIP odbiorcy (właściciela) należy:

- Nie zamykając zakładki Podatki, przejść do głównego okna Weles.
- W zakładce Zasoby wybrać wspólnotę i przejść do zakładki Administracja.
- W zakładce przejść do menu Zasoby > Edytuj dane właścicieli.
- Na liście właścicieli odszukać odbiorcę, który ma wpisany błędny NIP lub nie ma go podanego.
- W Polu NIP wpisać poprawny numer.
- Kliknąć Dodaj.
- Wpisać hasło i zatwierdzić.
- Powrócić do zakładki Podatki.
- Kliknąć OK na okienku błędu i spróbować ponownie wygenerować plik JPK.

Aby poprawić lub dodać NIP dostawcy (kontrahenta) postępujemy podobnie, z tą różnicą, że poprawiamy go w:

- Zakładka Zasoby > Menu Zasoby > Edytuj kontrahentów.

![JPK brak NIPu](brakNIP.gif)

### Uwagi:

- NIP należy poprawić lub uzupełnić wszystkim odbiorcom, lub dostawcom w danym okresie, za który generujemy plik.
- Zwykłym właścicielom lokali można podać NIP o wartości 9999999999 - "Brak".
- Przy większych nieruchomościach można zwrócić się do zespołu pomocy Weles o nadanie wszystkim właścicielom NIPu "Brak".