---
title: 2. Naliczenie i sprawdzenie korekty
---

# Naliczenie i sprawdzenie korekty

Jeśli zmiana wsteczna jednego ze składników naliczeń/opłat spowoduje zmianę jej wysokości, to system automatycznie to wykryje i stworzy korektę opłaty. Aby zobaczyć naliczone korekty opłat, należy przejść do: 

- Zakładka `Administracja` > przycisk `Naliczenia` > `K. bieżąca` — fioletowa pozycja.
- Pole `Struktura` > zaznaczyć cały budynek, przeliczenie na całym budynku powoduje przeliczenie na wszystkich lokalach podrzędnych.
- Menu `Obciążenia` > `Nalicz korekty`.

Samo naliczanie korekty nie jest równoznaczne z jej zaksięgowaniem. Właściciele nie widzą naliczonych korekt — widzą je dopiero po zaksięgowaniu. Korekta nie aktualizuje się automatycznie, aby zapoznać się z jej aktualnym stanem, należy ją ponownie naliczyć. Próbne księgowania korekt/rozliczeń prosimy przeprowadzać w bazie testowej. Gdy mamy wprowadzone korekty bieżące to prosimy nie cofać naliczeń — usunie to wprowadzone zmiany.

System zaprezentuje tabelkę. W jej kolumnach pokaże nam odpowiednio:

- `Nazwa` > nazwa korygowanej pozycji.
- `ID` > ID algorytmu.
- `Ilość` > skumulowana, prawidłowa ilość po korekcie.
- `JM` > jednostka miary prezentowanej wartości w kolumnie Ilość.
- `Stawka` > wartość stawki użyta do obliczenia nowego obciążenia lokalu.
- `Wartość` > różnica między wartościami z kolumn: `Ma być Wartość` a `Było Wartość`. Kwota z plusem to obciążenie właściciela, a z minusem to zwrot.
- `Ma być Wartość` > skorygowane, nowe obciążenie za dany składnik w korygowanym okresie, które równa się: `Ilość` * `Stawka`.
- `Było Wartość` > zaksięgowana dotychczas kwota za dany składnik naliczeń — tzw. Wcześniejsze obciążenia — suma zaliczek lub/i korekt lub/i rozliczeń, na które wprowadzona korekta ma wpływ.

Na przykładzie poniżej przeliczamy korektę liczby osób dla lokalu M03 oraz korektę stawki za eksploatację dla całego budynku.

![Naliczenie korekty](naliczeniekorekty1.gif)

#### Sprawdzenie korekty

Sugerujemy zawsze po naliczeniu korekty, sprawdzenie których lokali ona dotyczy i na jakie wcześniejsze obciążenia ma wpływ. Aby to wykonać, należy:

- Zakładka `Administracja` > kliknąć najwyższą strukturę na drzewku (nazwę nieruchomości).
- Kliknąć `Naliczenia`.
- Kliknąć `K. bieżąca` — fioletowa pozycja.
- Wpośród naliczonych korekt, klikamy na interesującą nas pozycję (zaznaczamy ją).
- Menu `Widok` > `Struktura naliczeń w lokalach`.

W nowym oknie system zaprezentuje wartości `Ma być Wartość` oraz rozłożenie korekty na lokale.

System ponadto umożliwia podgląd struktury korekty w pojedynczym lokalu. Sprawdzą tam Państwo dokładnie których naliczeń korekta dotyczy (`Było Wartość`) oraz na jaką wartość są one korygowane (`Ma być Wartość`). Aby to wykonać, należy:

- Pole `Struktura` > wybrać lokal.
- Kliknąć `K. bieżąca` — fioletowa pozycja.
- Wpośród naliczonych korekt, klikamy na interesującą nas pozycję (zaznaczamy ją).
- Menu `Widok` > `Struktura naliczeń`.

![Sprawdzenie korekty](naliczeniekorekt2.gif)