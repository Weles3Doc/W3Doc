---
title: Wysyłka SMS - windykacja
---

# Wysyłka SMS — windykacja

Aby wysłać właścicielom SMS z informacją o saldzie lub wzywającego do zapłaty, należy przejść do:

- Zakładka `Administracja` > menu `Funkcje` > `Wysyłka SMS`.
- Zakładka `W przygotowaniu`.
- Pole `Wysyłka` > ustawiamy jedno z:
  - `Tylko do zalegających (zbiorczo)` - do filtrowania będzie brane sumaryczne zadłużenie z kont właściciela.
  - `Tylko do zalegających (indywidualnie)` - warunki filtrowania zostaną zastosowane osobno dla każdego konta właściciela.
- Pole `Zakres dat` > ustawiamy czy saldo ma być brane wg `Terminów płatności` lub `Daty księgowania`.
- Pole `Zaległość na dzień` > ustawiamy datę salda właściciela, która zostanie poddana filtrowaniu.
- Pole `Min zaległość` > wpisujemy kwotę minimalnej zaległości (opcjonalnie).
- Pole `Maks zaległość` > wpisujemy kwotę maksymalnej zaległości (opcjonalnie).
- Pole `Min procent` > podajemy minimalną wartość procentową. Na przykład, jeśli podamy 200%, to będzie to dwu krotność miesięcznego czynszu (opcjonalnie).
- Pole `Maks procent` > podajemy maksymalną wartość procentową. Na przykład, jeśli podamy 400%, to będzie to 4 krotność miesięcznego czynszu (opcjonalnie).
- Klikamy: `Filtruj`.

W lewej części okna pojawią się właściciele, dla których zostały spełnione wcześniej warunki filtrowania. Można tutaj jeszcze dokonać dokładniejszej selekcji — wybierając jednego, kilku lub wszystkich właścicieli, odpowiednio ich zaznaczając. W prawej części okna uzupełniamy:

- Pole `Nazwa wysyłki` > podajemy, czego dotyczy wysyłka.
- Pole `Wysyłka` > `SMS`.
- Pole `Podgląd` > można w nim sprawdzić finalną postać SMS-a.
- Pole `Treść SMS` > wpisujemy treść SMS przypominającą o saldzie lub wzywającą do zapłaty.
- Pole `Informacja o saldzie` > ustawiamy parametry, które mają dodać się do treści SMS.
- Pole `Pula płatności` > określamy, z którego wykupionego pakietu SMS ma zostać potrącona ilość wysłanych wiadomości.
- Pole `Priorytet` > ustawiamy opóźnienie wysyłki.
- Pole `GSM` > zostanie pokazana ilość SMS-ów do wysłania.
- Klikamy: `Wyślij`.

Po zatwierdzeniu system przeniesie nas do zakładki Wysyłka. Można w niej ostatecznie sprawdzić wysyłkę lub ewentualnie ją zatrzymać klikając `Zatrzymaj wysyłkę`.

![SMS windykacja](smswindykacja.gif)