---
title: Import wyciągu zwykłego
---
# Import wyciągu zwykłego

- Wyciągi zwykłe/elektroniczne importujemy poprzez: zakładka Zasoby -> menu Funkcje -> Importuj wyciąg elektroniczny
- Identyfikacja, następuje tutaj poprzez bankowe KONTO ŹRÓDŁOWE, z którego jest przykładowa transakcja.
- Wymagana jest wcześniejsza konfiguracja głównych parametrów rachunku, w zakładce Rachunki bankowe.
- Wymagane są też, przypisania rozpoznanych kont bankowych, do kont księgowych w systemie Weles, na których to mają nastąpić poszczególne księgowania. Każde konto przypisuje się tylko raz, a system pamięta jego ustawienia (zakładka [Edycja])
- Po imporcie, jeśli nie będzie błędów i okno zamknie się samo, można odświeżyć i ponownie przejść w okno importu i na jej zakładkę [Podgląd], gdzie można podejrzeć zaimportowany plik i jego pozycje.
- Plik eWB powinien też być widoczny na zakładce Dekrety danej WM, do której był import.
- Dekret eWB jest edytowalny.

![Import wyciągu](importwbzwyklego.gif)

### Importuj wyciąg elektroniczny

Funkcja służy do importowania wyciągów elektronicznych bez udziału płatności masowych. Na podstawie wygenerowanego z systemu bankowego pliku (prawidłowe formaty plików to np csv, txt, mt-940; system nie rozpozna plików w formacie pdf), możemy zaksięgować poszczególne pozycje z rachunku bankowego. Program identyfikuje pozycje w pliku na podstawie numeru konta bankowego wpłacającego i przypisuje je do odpowiedniego konta w systemie. 

### Rachunki bankowe

Pierwszym niezbędnym krokiem jest określenie Numeru konta bankowego nieruchomości, z którego wykonywane są transakcje (wpłaty/wypłaty) - jest to wspólne ustawienie dla Eksportu zapłat elektronicznych (polecenie zapłaty) oraz dla Importu wyciągów elektronicznych (zwykłych — bez płatności masowych).

- W zakładce Zasoby wybieramy menu Funkcje i Importuj wyciąg elektroniczny.

![Import WB](impwb1.png)

- Po chwili otworzy się nowe okno dialogowe. Przechodzimy do zakładki Rachunki bankowe.

![Import WB](impwb2.png)

- Wybieramy Zasób (nieruchomość/wspólnotę), której będziemy przypisywać numer rachunku bankowego.

![Import WB](impwb3.png)

- Wskazujemy Konto, na które księgowane będą obroty — system pokaże tutaj wszystkie konta analityczne dla syntetyki określonej typem Rachunek bankowy (zwykle 13x).

![Import WB](impwb4.png)

- Wskazujemy Konto pozycji nierozpoznanych. Plik wyciągu bankowego zawiera także takie pozycje jak prowizje bankowe, wpłaty w kasie w banku/poczcie itp. — są to pozycje, których nie da się przypisać do konta, dlatego wpłaty takie domyślnie będą trafiały na wskazane tutaj konto (np. 149-1 Wpłaty do wyjaśnienia).

![Import WB](impwb5.png)

- Wskazujemy Bank, z którym mamy podpisaną umowę — jest to potrzebne do określenia odpowiedniego formatu kodowania (tak, żeby pliki systemu bankowego zostały poprawnie zinterpretowane oraz, żeby Weles generował właściwie polecenia zapłaty). W przypadku, gdyby na liście brakowało Państwa banku, prosimy o kontakt mailowy z danymi kontaktowymi do opiekuna — postaramy się jak najszybciej zaktualizować listę, o ile będzie taka możliwość.

![Import WB](impwb6.png)

- Wprowadzamy Numer rachunku bankowego. Cyfry mogą być oddzielone spacją lub wprowadzone ciągiem (bez odstępów).

![Import WB](impwb7.png)

- Klikamy: Dodaj.

![Import WB](impwb8.png)

- Możemy od razu uzupełnić dane dla pozostałych nieruchomości.

![Import WB](impwb9.png)

- Całość zatwierdzamy Hasłem.

![Import WB](impwb10.png)

### Import wyciągów elektronicznych

Sam import sprowadza się do wygenerowania w banku zestawienia operacji na rachunku i zaimportowania takiego zestawienia w wersji elektronicznej (plik) do programu Weles. Program na podstawie numeru konta wpłacającego identyfikuje daną pozycję i przypisuje do konkretnego konta w systemie Weles. Operacje typu wpłata w kasie banku/poczty są traktowane jako niezidentyfikowane i będą księgowane na wskazanym wcześniej koncie pozycji nierozpoznanych.

- W zakładce Zasoby wybieramy menu Funkcje i Importuj wyciąg elektroniczny.

![Import WB](impwb11.png)

- Po chwili otworzy się nowe okno dialogowe. W zakładce Dodawanie wskazujemy pobrany z banku raport, wpisujemy Hasło i klikamy Zatwierdź.

![Import WB](impwb12.png)

- System sprawdza, czy dany numer konta bankowego jest przypisany do konta w programie. Jeżeli wszystkie pozycje są przypisane, system zamknie okno, a wyciąg się zaimportuje. Jeżeli w pliku będą jakieś pozycje bez przypisanych kont, program wyświetli komunikat o błędzie — konieczne jest przypisanie tych pozycji. 

![Import WB](impwb13.png)

- Przechodzimy do zakładki Edycja i wskazujemy Rachunek zasobu, dla którego chcemy przypisać nieznane wpłaty.

![Import WB](impwb14.png)

- Wpłaty, które system rozpoznaje, mają przypisane konta.

![Import WB](impwb15.png)

- Nierozpoznane pozycje z wyciągu bankowego przypisujemy, klikając znak lupy po prawej stronie. System podstawi dane z wyciągu do powyższych formularzy.

- ![Import WB](impwb16.png)

- Przechodzimy do pola Konta i wskazujemy konto w planie kont, gdzie system ma księgować daną pozycję z wyciągu (parujemy numer rachunku wpłacającego z kontem w systemie).

![Import WB](impwb17.png)

- Klikamy: Dodaj. Uzupełniamy tak WSZYSTKIE nierozpoznane pozycje.

![Import WB](impwb18.png)

- Na koniec wpisujemy Hasło i klikamy Zatwierdź. System powinien zamknąć okno.

![Import WB](impwb19.png)

- Ponownie wybieramy menu Funkcje i Importuj wyciąg elektroniczny.

![Import WB](impwb20.png)

- Wskazujemy nasz wyciąg, wpisujemy Hasło i Zatwierdzamy. Okno powinno się zamknąć. 

![Import WB](impwb21.png)

- Ponownie przechodzimy do menu Funkcje i Importuj wyciąg elektroniczny.

![Import WB](impwb22.png)

- Przechodząc do zakładki Podgląd, możemy podejrzeć zaimportowane wyciągi elektroniczne.

![Import WB](impwb23.png)