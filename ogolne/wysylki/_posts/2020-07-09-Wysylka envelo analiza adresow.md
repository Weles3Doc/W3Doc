---
title: Wysyłka Envelo - analiza adresów
---

# Wysyłka Envelo — analiza adresów

#### Adres właściciela

Do poprawnej wysyłki listów przez `Envelo` potrzebny nam jest poprawny adres właściciela lokalu wpisany w polu `Adres`. Układ linii adresu powinien wyglądać następująco:


Nazwa firmy  
Imię Nazwisko  
ul. Ulica Nr budynku/Lokalu  
Kod pocztowy Miasto  


A dokładniej:

`Pierwsza linia adresu`  
`Druga linia adresu`  
`ul. _ Nazwa ulicy _ nr budynku / nr lokalu` (lub zamiast / można użyć m.)  
`Kod pocztowy _ Miejscowość`  

Jeśli na wydruku chcemy zawrzeć adres nieruchomości, której dokument dotyczy oraz adres korespondencyjny, to konstrukcja pola adresowego powinna wyglądać następująco:

Tomasz Nowak  
ul. Wiatraczna 1 m. 1  
04-365 Warszawa  

Adres do korespondencji:  
Tomasz Nowak  
ul. Berka Joselewicza 2  
07-400 Ostrołęka  

Adresy do usługi Envelo są rozpoznawane od ostatniej linii.

#### Analiza adresów

Program zawsze sprawdza, czy da się z adresu wprowadzonego w systemie, uzyskać powyższe dane. Bez tego, list nie zostanie wysłany, aby sprawdzić poprawność adresów, należy przejść do:

- Zakładka `Administracja` > menu `Funkcje` > `Wysyłka e-mail`.
- Zakładka `Analiza adresów`.

W tej zakładce mamy odpowiednio, zaczynając od lewej, nazwę właściciela, numer lokalu i adres dodany w systemie. W dalszych polach są prezentowane dane rozpoznane z adresów właścicieli. Dane adresowe rozpoznane poprawnie są prezentowane na zielono, więc szukamy pozycji, w których widnieje kolor czerwony. W przykładzie poniżej widzimy, że dane adresowe lokalu użytkowego nie zostały rozpoznane.

![Analiza adresów](enveloadresy1.gif)

#### Poprawienie adresu właściciela

Aby poprawić adres właściciela, należy przejść do:

- Zakładka `Administracja` > menu `Zasoby` > `Edytuj dane właścicieli`.
- Na liście z lewej strony okna zaznaczamy właściciela do edycji.
- Klikamy: `Edycja`.
- Pole `Adres` > poprawić na adres rozpoznawany przez system.
- Pole `Weryfikacja adresu` > `Sprawdzaj strukturę`, opcja ta odpowiada za sprawdzanie adresu, pod kątem wysyłki przez Envelo.
- Pozostałe pola nie są istotne, jeśli chodzi o wysyłkę dokumentów.
- Klikamy: `Zapisz`.

Jeśli okno się nie zamknęło i pojawił się błąd w pozycji, to oznacza, że system nie rozpoznał poprawnie adresu, adres trzeba jeszcze raz poprawić.

![Analiza adresów](enveloadresy2.gif)