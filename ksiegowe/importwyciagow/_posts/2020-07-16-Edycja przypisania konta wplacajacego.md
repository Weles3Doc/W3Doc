# Edycja przypisania konta wpłacającego

Przy importach wyciągów elektronicznych zwykłych, system Weles3 sczytuje z kolejno wczytywanych plików, źródłowe konta bankowe wpłacających i tworzy z nich tzw. tablicę przypisań. W tablicy, są również widoczne Tytuły wpłat, ale tylko z pierwszych, rozpoznanych transakcji. Są one pomocne w identyfikacji wpłacającego.

 Tworzona jest odrębna tablica dla każdego, zdefiniowanego rachunku WM.

Przypisania te, można edytować i będą one obowiązywać od kolejnych, importowanych plików.

W tym, celu:

- Przechodzimy do okna importów elektronicznych: zakładka Zasoby -> menu Funkcje -> Importuj wyciąg elektroniczny.
- W oknie importu przechodzimy na zakładkę Edycji i wskazujemy zasób/rachunek danej WM.
- W tablicy przypisań zasobu należy odszukać wybrane przypisanie i przejść do jego edycji, klikając na ikonkę lupy.
- W polu Konta FK wskazujemy inne PODKONTO właścicielskie lub inne konto FK z planu kont do księgowania.
- Dodajemy pozycję (powinna ona nadpisać tę poprzednią w tablicy) i akceptujemy hasłem.

Poniżej, film instruktażowy z tej operacji.

![Edycja przypisanego konta](edycjaprzypisania.gif)