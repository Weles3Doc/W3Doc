---
title: 4. Akceptacja dokumentów
---

# Akceptacja dokumentów

Z wykorzystaniem opisywanej funkcji można wprowadzić wieloetapowe sprawdzanie dokumentów przed ich zaksięgowaniem w systemie Weles3. Udostępniliśmy na to moduł akceptacji, który udostępnia pięć statusów możliwych do nadania dokumentowi:

- `Nowa` > każdy nowy plik zyskuje ten status automatycznie.
- `Oczekująca` > etap z myślą na dalszą weryfikację dokumentu.
- `Zaakceptowana` > faktura jest sprawdzona i gotowa do zaksięgowania/opłacenia.
- `Odrzucona` > ten status oznacza wykluczenie pliku.
- `Zapłacona` > faktura została opłacona i czeka na księgowanie.

Znaczenie tych punktów jest umowne i nie narzucone, każdemu z statusów mogą Państwo nadać dowolne znaczenie i czynności z nim związane. Odrzucone pliki nie są domyślnie wyświetlane na liście. Księgować faktury można na dowolnym etapie. Zaksięgowane dokumenty nie są wyświetlane na liście.

Korzystanie z tej funkcji jest bardzo proste i intuicyjne, aby nadawać statusy dokumentom należy przejść do:

- Zakładka `Zasoby` > menu `Funkcje` > `Akceptacja dokumentów`.

Zaraz po przejściu do okna możemy:

- Pole `Konto` > domyślnie jest podpowiadany system `KSeF` można go przełączyć na połączone konto `Google Drive`.
- Pole `Typ podglądu` > tylko dla `Google Drive`, odpowiada za podgląd pliku w prawej części okna:
    - `Bezpośredni` > podgląd pliku pochodzi bezpośrednio z dysku Google.
    - `Pośredni` > podgląd pliku pochodzi z serwerów Weles 3, wybieramy tą opcję gdy nie mamy dostępu lub nie jesteśmy zalogowani w przeglądarce do konta Google na którym znajdują się pliki.
- Przycisk `Odśwież` > klikamy gdy chcemy odświeżyć listę plików do zaksięgowania.
- Pole `Zasób` > tylko dla `KSeF`, pozwala na odfiltrowanie faktur dla jednego zasobu.
- Pole `Faktury` > pozwala na filtrowanie plików pod względem statusu.
- Pole `Przypisanie` > pozwala na filtrowanie plików pod względem przypisanej osoby.
- Przycisk `Następne` i `Poprzednie` > gdy plików/faktur jest bardzo dużo pozwala na przełączanie pomiędzy widocznymi pozycjami na liście.

Aby nadać lub zmienić status fakturze, należy:

- Wybrać pozycję na liście po lewej stronie.
- Pole `Status` > wybrać pożądany status.
- Pole `Osoba odpowiedzialna` > można wyznaczyć osobę skojarzoną z fakturą.
- Pole `Komentarz` > można uzupełnić informację tekstową, będzie ona widoczna podczas księgowania.
- Kliknąć: `Zapisz`.

Wszystkie czynności przedstawiamy na ponizszym filmiku.

![Akceptacja dokumentów](akceptacja-doku01.gif)