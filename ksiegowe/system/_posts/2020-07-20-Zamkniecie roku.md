---
title: Zamknięcie roku FK
---

# Zamknięcie roku FK

Poniższa instrukcja ma za zadanie opisać przykładową procedurę zamknięcia roku rozliczeniowego. Nie jest ona uniwersalna, należy ją dostosować do specyfiki danej nieruchomości.

#### Przygotowania

Przed przystąpieniem do zamykania roku trzeba:

- Zaksięgować wszystkie zaliczki w danym roku.
- Zaksięgować wszystkie wpłaty właścicieli.
- Zaksięgować wszystkie koszty.
- Zrobić inne potrzebne księgowania.

Warto tutaj też nadmienić, że nie muszą Państwo czekać z księgowaniami z bieżącego roku, należy wprowadzać je normalnie, system i tak zamknie pierwszy otwarty rok.

#### Rozliczenie liczników 

Jeśli w budynku znajdują się liczniki oraz ich termin rozliczenia wypada na koniec roku to w tym momencie, należy zrobić rozliczenie, więcej na ten temat znajduje się w dokumentacji:

- `Administracyjne` > `Rozliczenia liczników`

Rozliczenia liczników nie są obowiązkowe przy zamykaniu roku, z punktu widzenia systemu. Można je pominąć, ustawiając termin w następnym roku i sporządzając odpowiednie przeniesienia przychodów i kosztów.

#### Rozliczenie kosztów

Następnym etapem, choć nie obowiązkowym, są rozliczenia kosztów. Jeśli zachodzi potrzeba zrównania przychodów z poniesionymi kosztami (rozliczenie na zero), to trzeba wykonać systemowe rozliczenia kosztów, które są dokładnie opisane w dedykowanych instrukcjach:

- `Administracyjne` > `Rozliczenia kosztów`

Rozliczenia zazwyczaj księgujemy na koniec okresu rozliczeniowego, którego dotyczą, w ten sposób nie wpływają na przychody roku bieżącego.

#### Zamykanie miesięcy

Przed zaksięgowaniem odsetek lub zamknięciem roku, konieczne jest zamknięcie miesięcy FK, aby to zrobić, należy przejść do:

- Zakładka `Dekrety` > menu `Funkcje` > `Zamykanie miesiąca FK`.
- Pole `Data` > ustawiamy ostatni zamykany miesiąc roku **RRRR-12**.
- Klikamy: `Zatwierdź`.

Zamknąć można kilka miesięcy naraz. W zamkniętym miesiącu nie można dodawać nowych dokumentów, można edytować istniejące, ale nie można edytować pozycji na kontach 201. Jeśli mają Państwo w danym budynku zamknięte miesiące i naliczone odsetki już w bieżącym roku to ten krok należy pominąć.

![Zamykanie miesiąca](zamykaniemiesiaca.gif)

#### Odsetki

Jeśli wspólnota ma zamiar naliczyć odsetki od nieterminowych wpłat w minionym roku, to należy wykonać tę czynność przed programowym zakończeniem roku. Odsetki naliczamy po zamknięciu wszystkich miesięcy w minionym roku, natomiast miesiące nowego roku powinny pozostać otwarte, ponieważ odsetki są księgowane zawsze na koniec ostatniego zamkniętego miesiąca. Jeśli mają Państwo w danym budynku zamknięte miesiące i naliczone odsetki już w bieżącym roku (są na przykład księgowane na bieżąco co miesiąc) to ten krok należy pominąć. Więcej na temat odsetek znajduje się w dokumentacji:

- `Księgowe` > `Odsetki`

#### Księgowanie wynikowe (KW)

Jedną z ostatnich czynności przed zamknięciem roku księgowego jest zrobienie księgowań wynikowych. Aby je wykonać, należy przejść do:

- Zakładka `Dekrety` > menu `Dokumenty` > `Księgowania wynikowe`.

Następnie wybieramy wynik, który będziemy trwożyli.

- Pole `Konto wynikowe` > wybieramy konto, dla którego będziemy robić księgowanie wynikowe.

W niższej części okna możemy ręcznie dodawać pozycje i edytować kwoty, jakie zostaną przeksięgowane na wynik.(Pola `Składnik`, `Kwota Wn`, `Kwota Ma`)

W dolnej części okna, w tabelce są pokazane proponowane pozycje, podpowiedzą się tylko i wyłącznie konta `4xx` i `7xx`. Zawierają numer, nazwę oraz saldo Wn i Ma konta.

Zasada postępowania jest prosta:
- **Pozostawiamy** tutaj tylko konta, dla których ma zajść przeksięgowanie wynikowe na wskazany wynik w polu `Konto wynikowe`.
- Zbędne pozycje usuwamy ikonką [x]  po prawej stronie pozycji.

Na koniec klikamy:

- Klikamy: `Zatwierdź`. 

Po zamknięciu okna, na liście dokumentów powinien się pojawić dekret KW, zostanie dodany na ostatni dzień zamkniętego miesiąca. Do funkcji księgowanie wynikowe można powrócić i stworzyć następny wynik finansowy. Stworzone dokumenty KW można ręcznie edytować do własnych potrzeb lub całkowicie usunąć i zrobić jeszcze raz.

![Księgowanie wynikowe](robieniekw.gif)

#### Wydruki sprawdzające

Po przejściu przez wymienione wyżej czynności, zmierzające ku formalnemu zakończeniu roku w programie, warto zapoznać się z niektórymi raportami sprawozdawczymi dla całej wspólnoty dostępnymi w wydrukach (zakładka `Zasób`). Poniżej przedstawiono te najważniejsze, na które powinno się zwrócić szczególną uwagę.

**Naliczenia** — Wydruk prezentuje sumaryczne obciążenia związane z zamykanym rokiem na całej nieruchomości bez podziału na właścicieli. Jest szczególnie przydatny przy analizowaniu poprawności kwot wynikających z rozliczenia, gdyż przy domyślnych ustawieniach pokazuje (wyszczególnia) podstawę obciążenia oraz sposób wykonania naliczenia (R, LR, LP, LZ, RKL, RKR) nawet w ramach tego samego algorytmu/składnika. Od razu widoczne są więc błędy wynikające z indywidualnych odstępstw od założonego scenariusza rozliczania (np. kwoty naliczone z ryczałtu przy rozliczeniu liczników "R" — sugerujące brak aktywnego licznika). Przykładowy wydruk:

![Zakończenie roku](zakrok14.png)

![Zakończenie roku](zakrok15.png)

**Rozliczenie** — Na wydruku mamy przedstawione zestawienie przychodów (konta 700) i kosztów (konta 400) oraz wynikające z nich salda obrotów związane z poszczególnymi składnikami naliczeń. Wydruk ten jest szczególnie przydatny do wprowadzania kwot przy rozliczeniach kosztów, jak również sprawdzenia/weryfikacji zaksięgowanego rozliczenia — po zaksięgowaniu rozliczenia salda dla rozliczanych składników powinny się zerować. Przykładowy wydruk:

![Zakończenie roku](zakrok16.png)

![Zakończenie roku](zakrok17.png)

**Plan rozliczenia kosztów** — Wydruk pokazuje wprowadzone kwoty oraz sposób wykonania rozliczenia kosztów. Przykładowy wydruk:

![Zakończenie roku](zakrok18.png)

![Zakończenie roku](zakrok19.png)

**Sprawozdanie finansowe** — Na wydruku sprawozdania finansowego widoczne są:

- Stan środków pieniężnych (100- Kasa, 131- Rachunki)
- Stan rozrachunków (201- właściciele, 202- dostawcy)
- Zestawienie przychodów (700-) i kosztów (400-), bez KW
- Rozliczenie międzyokresowe (640-)
- Konta wynikowe (856- Fundusz remontowy, 860- Wynik finansowy), po KW

Jest to niezwykle przydatny wydruk sprawozdawczo-kontrolny, pozwala w szybki i czytelny sposób zapoznać się ze stanem księgowym prowadzonej nieruchomości/wspólnoty. Przykładowy wydruk:

![Zakończenie roku](zakrok20.png)

![Zakończenie roku](zakrok21.png)

**Obroty na kontach** — Wydruk (tzw. obrotówka, szczególnie przydatny w swojej poziomej formie, Pole `Strona` > `A4 Poziomy`) pokazuje dla poszczególnych kont syntetycznych salda i obroty narastająco po obu stronach księgowania (możliwe jest zejście niżej z poziomem analityki przy szukaniu nieprawidłowości). Szczególnie szybko pozwala wyłapać brak bilansowania się kont przychodów i kosztów 400/700 oraz prawidłowego wykonania księgowania wynikowego (KW). Przykładowy wydruk:

![Zakończenie roku](zakrok22.png)

![Zakończenie roku](zakrok23.png)

#### Zamknięcie roku

Po wykonaniu wszystkich poprzedzających czynności i sprawdzeniu podstawowych wydruków sprawozdawczych dla wspólnoty/nieruchomości możemy formalnie zakończyć rok — wykonać przejście roczne. Gdyby któraś z czynności poprzedzających nie została wykonana do końca, to system może nie pozwolić na zakończenie roku. Aby zamknąć rok, należy przejść do:

- Zakładka `Dekrety` > menu `Funkcje` > `Zamykanie roku FK`.
- Pole `Zakończenie roku` > `Zakończ rok`.

Pola w środkowej części okna odpowiadają za sposób liczenia sald na podkontach rozrachunkowych właścicieli. Można w tym momencie wprowadzić zmiany na przyszły rok, więcej na temat w dedykowanej instrukcji `Sposób liczenia sald 201`, ew. pozostawić bez zmian.

- Klikamy: `Zatwierdź`.

Zamknięty rok będzie dostępny do podglądu w zakładce `Zasoby`, po kliknięciu `>` przy nazwie wspólnoty. Rok zostanie zamknięty zawsze pojedynczo, zaczynając od najstarszego, niezależnie od ilości otwartych lat.

![Zamykanie roku](zamykanieroku.gif)