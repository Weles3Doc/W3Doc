---
title: Przykład RK - wyłączenie lokalu z RK
---

# Przykład RK - wyłączenie lokalu z RK

Czasami zdarza się, że momencie rozliczenia kosztów należy pominąć pewien lokal lub pewną grupę lokali w budynku. Posłużymy się tutaj przykładem rozliczenia centralnego ogrzewania z innej instrukcji. Na potrzeby tej instrukcji załóżmy, że z różnych względów lokal użytkowy powinien być wykluczony z rozliczenia CO, cały koszt zostanie rozliczony na mieszkania. Aby zdefiniować taki sposób rozliczeń, należy przejść do:

- Przycisk `Naliczenia` > `K. bieżąca`.
- Menu `Obciążenia` > `Rozliczenia kosztów`.

W oknie definiujemy dwie pozycje, pierwsza:

- Pole `Element struktury` > ustawiamy strukturę lub lokal, które chcemy wyłączyć z rozliczenia. 
- Pole `Typ` > wybieramy:
  - Jeśli lokal miał naliczane zaliczki — wybieramy pozycję `Algorytm - różnica` lub `Obciążenia - różnica`.
  - Jeśli lokal nie miał naliczanych zaliczek — można wybrać dowolną pozycję.
- Wszystkie inne pola zależą od wybranego sposobu rozliczeń.
- Pole `Wartość` > wpisujemy kwotę kosztu (lub różnicy) równą **zero**.
- Klikamy: `Dodaj`.

Druga pozycja:

- Pole `Element` > struktury wybieramy całą WM (lub inną strukturę).
- Wszystkie inne pola zależą od wybranego sposobu rozliczeń.
- Pole `Wartość` > wpisujemy kwotę do rozliczenia.
- Klikamy: `Dodaj`.

Gdy wszystkie będą wprowadzone:

- Klikamy: `Zatwierdź`.

Udział w rozliczeniu kosztów zostanie obliczony z pominięciem wyłączonego lokalu. Jeśli lokalowi zostanie ustawiony typ pełnym kosztem oraz wartość = 0, to zaliczki zostaną mu zwrócone (jeśli miał je naliczane).

![Przykład RK - wyłączenie lokalu z RK](przykladRKwyllokalu.gif)