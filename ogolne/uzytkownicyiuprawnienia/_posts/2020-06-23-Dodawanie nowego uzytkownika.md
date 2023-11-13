---
title: Dodanie nowego użytkownika
---

# Dodanie nowego użytkownika

Dodanie nowego użytkownika systemu rozpoczynamy od przejścia do:

- Zakładka `Zasoby` > menu `Funkcje` > `Administratorzy`.
- Kliknąć: `Nowy`.
- Pole `Administratorzy` > wpisujemy nazwę, zazwyczaj podajemy imię i nazwisko.
- Pole `Końcówka` > wpisujemy krótką frazę, która doda się do loginu użytkownika. (**Patrz uwagi**)
- Pole `Hasło` > podajemy hasło tymczasowe dla nowego użytkownika.
- Pole `Uprawnienia` > przypisujemy użytkownikowi dostęp do funkcji systemu.
- Klikamy: `Utwórz`.

Użytkownik ma natychmiast dostęp do systemu, osobie trzeba przekazać login i hasło tymczasowe. Po dodaniu nowego użytkownika trzeba jeszcze dodać uprawnienia do poszczególnych budynków w systemie.

![Dodawanie użytkownika](dodawanie-administratora.gif)

### Uwagi:

- Administratorzy systemu logują się przez stronę: https://weles3.pl/logowanie/
- Nazwa użytkownika może być dowolna, zazwyczaj podajemy imię i nazwisko, maksymalnie 20 znaków. Nazwa musi być unikalna. W nazwie użytkownika można umieścić przedrostek, aby posegregować osoby ze względu na pełnione funkcje w firmie.
- W polu `Końcówka` wpisujemy inicjały użytkownika lub inną unikalną i krótką frazę. Doda się ona po kropce (czyli kropki nie wpisujemy w polu końcówka) do nazwy bazy klienta, co razem stworzy login użytkownika.
  - Przykład: Jan Kowalski
  - Końcówka: *jako*
  - Login: **baza**.jako            
  - Więc docelowym loginem będzie: **doc**.*jako*
- System wymusi zmianę hasła tymczasowego podczas pierwszego logowania do systemu.
- System wymusza zmianę hasła co 30 dni.