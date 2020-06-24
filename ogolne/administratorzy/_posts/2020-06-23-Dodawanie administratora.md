# Dodanie nowego użytkownika
Dodanie nowego użytkownika systemu rozpoczynamy od przejścia do:
- Zakładka Zasoby > menu Funkcje > Administratorzy.
- W nowo otwartym oknie klikamy na przycisk Nowy.
- Pole Administratorzy > wpisujemy nazwę, zazwyczaj podajemy imię i nazwisko.
- Pole Końcówka > wpisujemy krótką frazę, która doda się do loginu użytkownika. (patrz uwagi)
- Pole Hasło > podajemy hasło tymczasowe dla użytkownika.
- Pole Uprawnienia > przypisujemy użytkownikowi dostęp do funkcji systemu.
- Wpisujemy hasło.
- Klikamy przycisk Utwórz.

Po dodaniu nowego użytkownika trzeba jeszcze dodać uprawnienia do poszczególnych budynków w systemie.

![Dodawanie użytkownika](dodawanie-administratora.gif)

## Uwagi:
- Nazwa użytkownika może być dowolna, zazwyczaj podajemy imię i nazwisko, maksymalnie 20 znaków. Pole musi być unikalne.
- W polu Końcówka wpisujemy inicjały użytkownika lub inną unikalną i krótką frazę. Doda się ona po kropce (czyli kropki nie wpisujemy w polu końcówka) do nazwy bazy klienta, co razem stworzy login użytkownika. Maksymalnie 20 znaków.
  - Przykład: Jan Kowalski
  - Końcówka: *jako*
  - Login: **baza**.jako            
  - Więc docelowym loginem będzie: **doc**.*jako*
- System wymusi zmianę hasła tymczasowego podczas pierwszego logowania do systemu.
- System wymusza zmianę hasła co 30 dni.