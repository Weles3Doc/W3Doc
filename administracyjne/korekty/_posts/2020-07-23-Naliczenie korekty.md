---
title: 2. Naliczenie korekty
---

# Naliczenie korekty

Jeśli zmiana wsteczna jednego ze składników naliczeń/opłat spowoduje zmianę jej wysokości, to system automatycznie to wykryje i stworzy korektę opłaty. Korekty bieżące są dostępne i widoczne tylko dla administratorów, właściciele ich nie widzą. Aby zobaczyć naliczone korekty opłat, należy przejść do: 

- Zakładka `Administracja` > przycisk `Naliczenia` > `K. bieżąca — fioletowa pozycja.
- Pole `Struktura` > zaznaczyć cały budynek.
- Menu `Obciążenia` > `Nalicz korekty`.

System zaprezentuje tabelkę. W jej kolumnach pokaże nam odpowiednio:

- `Nazwa` > nazwa korygowanej pozycji.
- `ID` > ID algorytmu.
- `Ilość` > Skumulowana, prawidłowa ilość po korekcie.
- `JM` > jednostka miary prezentowanej wartości w kolumnie Ilość.
- `Stawka` > wartość stawki użyta do obliczenia nowe obciążenia lokalu.
- `Wartość` > różnica między wartościami z kolumn: `Ma być Wartość` a `Było Wartość`.
- `Ma być Wartość` > skorygowane, nowe obciążenie za dany składnik w korygowanym okresie, które równa się: `Ilość` * `Stawka`.
- `Było Wartość` > zaksięgowana dotychczas kwota za dany składnik naliczeń — tzw. Wcześniejsze obciążenia — suma zaliczek lub/i korekt lub/i rozliczeń, na które wprowadzona korekta ma wpływ.

![Naliczeniekorekty1](naliczeniekorekty1.gif)

Sugerujemy zawsze po naliczeniu korekty, sprawdzenie których lokali ona dotyczy. Aby to wykonać należy:

- Zakładka Administracja > kliknąć na najwyższą strukturę na drzewku (nazwę nieruchomości).
- Przycisk Naliczenia > kliknąć na korektę bieżącą (K. bieżąca - fioletowa pozycja).
- Wpośród naliczonych korekt, klikamy na interesującą nas pozycję (zaznaczamy ją).
- Menu Widok > Struktura naliczeń w lokalach.

W nowym oknie, system zaprezentuje rozłożenie danego naliczenia w lokalach, w funkcji czasu (instrukcja dot. tego narzędzia).

![Naliczeniekorekty2](naliczeniekorekt2.gif)

System ponadto umożliwia podgląd struktury korekty w pojedynczym lokalu. Sprawdzą tam Państwo dokładnie których naliczeń korekta dotyczy (Było Wartość) oraz na jaką wartość są one korygowane (Ma być Wartość). Aby to wykonać należy:
- Pole Struktura > wybrać lokal.
- Przycisk Naliczenia > kliknąć na korektę bieżącą (K. bieżąca - fioletowa pozycja).
- Wpośród naliczonych korekt, klikamy na interesującą nas pozycję (zaznaczamy ją).
- Menu Widok > Struktura naliczeń.

W nowym oknie system pokaże rozłożenie danego naliczenia w lokalu, w funkcji czasu (instrukcja dot. tego narzędzia).

### Uwagi:
- Samo naliczanie korekty nie jest równoznaczne z jej zaksięgowaniem.
- Właściciele nie widzą naliczonych korekt - widzą je dopiero po zaksięgowaniu.
- Korekta nie aktualizuje się automatycznie, aby zapoznać się z jej aktualnym stanem należy ją ponownie naliczyć.
- Próbne ksiegowania korekt/rozliczeń prosimy przeprowadzać w bazie testowej.
- Gdy mamy wprowadzone korekty bieżące to prosimy nie cofać naliczeń - usunie to wprowadzone zmiany.