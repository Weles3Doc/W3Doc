---
title: Podgląd dla członka zarządu
---

# Podgląd dla członka zarządu

Aby nadać członkowi Zarządu dostęp bierny — tylko do podglądu, bez możliwości zmian należy dodać nowe konto użytkownika oraz nadać uprawnienia do konkretnego budynku. W tym celu przechodzimy do:

- Zakładki `Zasoby` > menu `Funkcje` > `Administratorzy`.
- Kliknąć: `Nowy`.
- Pole `Administratorzy` > wpisujemy nazwę użytkownika. Nazwą może być imię i nazwisko, jednak sugerujemy tutaj stworzenie jej od nazwy nieruchomości. Nazwę nadajemy na zasadzie: Z + NazwaWM + Nr, przykładowo: Z-Wiatraczna-1.
- Pole `Końcówka` > wpisujemy krótką frazę, która doda się do loginu użytkownika. (patrz uwagi)
- Pole `Hasło` > podajemy hasło tymczasowe dla użytkownika.
- Pole `Uprawnienia` > **nie nadajemy żadnych uprawnień (WAŻNE!).**
- Pole `Hasło` > wpisujemy własne hasło.
- Klikamy: `Zapisz`.

Nie zamykamy okna, trzeba jeszcze nadać uprawnienia do budynku.

![Dodawanie użytkownika](zarzad1.gif)

- Przechodzimy do zakładki: `Uprawnienia`.
- Klikamy: `Edycja`.
- Pole `Administratorzy` > wybieramy nowo dodane konto członka zarządu. (można wybrać kilka).
- Pole `Wspólnota` > wybieramy budynek, do której wybrany użytkownik ma mieć podgląd.
- Pole `Dostęp` > wybieramy **Dostępny**.
- Pole `Uprawnienia` > **nie nadajemy żadnych uprawnień (WAŻNE!).**
- Pole `Hasło` > wpisujemy własne hasło.
- Klikamy: `Zapisz`.

![Dodawanie uprawnień](zarzad2.gif)

### Uwagi:

- Tak stworzony użytkownik będzie: 
  - Miał możliwość podglądu bazy tylko do odczytu, bez możliwości wprowadzania zmian. 
  - Widział nieruchomość tak jak normalny administrator. 
  - Mógł generować wydruki.
  - Widział plan kont (ogólny i wspólnoty) oraz dokumenty księgowe.
- Login użytkownika powstaje poprzez dodanie po kropce zawartości pola Końcówka do nazwy bazy. (kropki nie trzeba wpisywać w polu Końcówka)
  - Przykład: Z-Wiatraczna-1
  - Końcówka: zarz-1
  - Login: baza.zarz-1 co daje w przykładowej bazie: doc.zarz-1
- System wymusi zmianę hasła tymczasowego podczas pierwszego logowania do systemu.
- System wymusza zmianę hasła co 30 dni.