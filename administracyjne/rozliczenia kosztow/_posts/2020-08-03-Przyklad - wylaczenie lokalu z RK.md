---
title: Przykład RK - wyłączenie lokalu z RK
---
# Przykład RK - wyłączenie lokalu z RK

Czasami zdarza się, że momencie rozliczenia kosztów należy pominąć pewien lokal lub pewną grupę lokali w budynku. Posłużymy się tutaj przykładem rozliczenia centralnego ogrzewania z innej instrukcji.  Na potrzeby tej instrukcji załóżmy, że z różnych względów lokal użytkowy powinien być wykluczony z rozliczenia CO, cały koszt zostanie rozliczony na mieszkania. Aby zdefiniować taki sposób rozliczeń należy:
- Przejść do Naliczenia > K. bieżąca.
- Następnie Menu obciążenia > Rozliczenia kosztów.
- W oknie definiujemy dwie pozycje, pierwsza:
  - W polu Element struktury ustawiamy strukturę lub lokal, które chcemy wyłączyć z rozliczenia. 
  - W polu Typ wybieramy:
    - Jeśli lokal miał naliczane zaliczki - wybieramy pozycję Algorytm - różnica lub Obciążenia - różnica.
    - Jeśli lokal nie miał naliczanych zaliczek - można wybrać dowolną pozycje.
  - Wszystkie inne pola zależą od wybranego sposobu rozliczeń.
  - W polu Wartość wpisujemy kwotę kosztu (lub różnicy) równą zero.
- Druga:
  - W polu Element struktury wybieramy całą WM (lub inną strukturę).
  - Wszystkie inne pola zależą od wybranego sposobu rozliczeń.
  - W polu Wartość wpisujemy kwotę kosztu.
- Wpisujemy hasło i zatwierdzamy.
- Przeliczamy i sprawdzamy rozliczenie kosztów.

### Uwagi:
- Udział w rozliczeniu kosztów zostanie obliczony z pominięciem wyłączonej grupy.
- Jeśli lokalowi zostanie ustawiony typ pełnym kosztem oraz wartość = 0, to zaliczki zostaną mu zwrócone (jeśli miał je naliczane).

![Przykład RK - wyłączenie lokalu z RK](przykladRKwyllokalu.gif)