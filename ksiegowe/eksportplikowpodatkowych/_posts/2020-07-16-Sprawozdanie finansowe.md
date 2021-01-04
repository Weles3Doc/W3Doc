---
title: Sprawozdanie finansowe
---

# Sprawozdania finansowe

W celu sporządzenia elektronicznego sprawozdania finansowego należy:

- Pobrać i zainstalować aplikację Ministerstwa Finansów.
- W aplikacji utworzyć sprawozdanie.
  - Konieczne jest prawidłowe podanie NIPu — po nim system będzie odnajdywał nieruchomość, której dotyczy sprawozdanie.
  - W aplikacji trzeba potwierdzić, że jest się osobą fizyczną — nie będzie to mieć znaczenia dla działania sprawozdań.
  - W aplikacji wypełniamy przymusowe pola bilansu i rachunku zysków i strat kwotami 0 - będzie to potem nadpisane przez Weles3.
- Do działania konieczne jest przypisanie specyfikacji raportów dowolnych dla odpowiedniego bilansu i rachunku zysków i strat.
- Przygotowany przez aplikację plik (zip lub xml) trzeba dodać do systemu za pomocą:
  - Zakłada `Zasoby` > menu `Funkcje` > `Podatki` > zakładka `Sprawozdania finansowe`.
- Po zatwierdzeniu zostanie pobrany plik sprawozdania, będący kopią przesłanego pliku ze zmianami:
  - Ustawionymi datami początkowymi i końcowymi.
  - Ustawioną datą sporządzenia.
  - Wypełnionymi bilansem i rachunkiem zysków i strat.
- Pobierany plik jest sprawdzany pod względem zgodności z definicjami struktur dostarczanymi przez Ministerstwo Finansów — jeżeli wystąpi niezgodność, plik się nie pobierze i zostanie wyświetlony komunikat o błędzie.
- Pobrany plik można otworzyć w aplikacji, aby podejrzeć jego zawartość.