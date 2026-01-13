---
title: Dodanie algorytmu do systemu
---

# Dodanie algorytmu do systemu

Zazwyczaj algorytmy są od razu zdefiniowane w systemie, więc nie ma potrzeby ich dodawania. Jednak gdy trzeba dodać nową opłatę, to stosujemy niżej przedstawioną instrukcje. Algorytmy są wspólne dla wszystkich budynków w systemie. W polu ID sugerujemy wpisywać czterocyfrowy numer algorytmu. Na podstawie jego są tworzone domyślnie konta przychodów i kosztów. Dla zasady stosujemy numerację:

- 1xxx > opłaty z grupy Media.
- 2xxx > opłaty z grupy Eksploatacja.
- 3xxx > opłaty z grupy Fundusz remontowy.

Powyższa zasada nie zawsze znajdzie zastosowanie w Państwa bazie danych, prosimy uważać na ID i konta algorytmów. Sprawdź najbardziej typowe algorytmy na końcu instrukcji. Aby dodać nowy algorytm, należy przejść do:

- Zakładka `Zasoby` > menu `Elementy` > `Nazwy algorytmów`.
- Klikamy: `Nowy`.
- Pole `ID` > wpisujemy unikalny numer algorytmu.
- Pole `Nazwa` > wpisujemy nazwę opłaty. Maksymalnie 50 znaków. Nazwę sugerujemy wpisywać jak najbardziej uniwersalną, tak aby algorytm mógł być wykorzystywany w wielu wspólnotach.
- Pole `Grupa należności` > wybieramy grupę należności.
- Pole `Konto przychodów` > tworzy się automatycznie na podstawie ID, można wpisać własne.
- Pole `Konto kosztów` > tworzy się automatycznie na podstawie ID, można wpisać własne.
- Pole `Stawka VAT` > można pozostawić ND lub wybrać inną wartość, istotne tylko przy naliczeniach z VAT-em.
- Pole `PKWiU` > wpisujemy kod Polska Klasyfikacja Wyrobów i Usług lub może pozostać puste.
- Pole `Typ` > dotyczy opłat z VATem:
    - `Podzielona płatności` > oznacza opłaty z tym parametrem jako Podzielone płatności w plikach JPK.
    - `GTU_12` > oznacza opłaty z tym parametrem jako GTU 12 w plikach JPK.
- Pole `Podstawa zwolnienia` > pole umożliwiające określenie podstawy zwolnienia od podatku (pod JPK i KSeF).
- Klikamy: `Utwórz`.

W podobny sposób można edytować już istniejący algorytm. Przy edycji sugerujemy nie zmieniać konta przychodów i kosztów oraz stawki VAT, nieumiejętne zmiany mogą mieć poważne konsekwencje. Algorytm dodajemy raz, będzie można go użyć we wszystkich nieruchomościach w bazie.

![Dodanie algorytmu](dodaniealgosys.gif)

Poniżej podajemy typowe algorytmy.

![Typowe algorytmy](typowealgo.png)