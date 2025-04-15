---
title: Terminy płatności
---

# Terminy płatności

Podczas księgowania należności nie określamy bezpośrednio terminu płatności dokumentów. Docelowy termin płatności będzie sumą ustawionej daty w polu `Bazowy termin płatności` oraz ilości dni określonej w niżej opisywanej funkcji. Dodatkowo będzie zależał od ustawionych opcji. Aby ustawić ilość dni doliczanych podczas księgowania, należy przejść do:

- Zakładka `Administracja` > menu `Elementy` > `Terminy płatności`.
- Pole `Dokument` > wybrać typ dokumentu, dla którego ustawiamy termin.
- Pole `Właściciel` > można wybrać osobę, dla której określimy indywidualny termin. Jeśli pozostanie wybrane `Wszyscy`, pozycja będzie dotyczyła wszystkich.
- Pole `Dni` > określamy ilość dni, która doda się do daty bazowej określanej przy księgowaniu należności i następnym polu.
- Pole `Data bazowa` > określamy, co ma być datą podstawową, do której dodadzą się `Dni`:
  - `Bazowy termin płatności` > określany przy księgowaniu należności.
  - `Początek miesiąca` > pierwszy dzień miesiąca, który jest ustawiony w polu `Data` w menu `Funkcje` > `Księguj należności`.
  - `Początek następnego miesiąca` > pierwszy dzień miesiąca **po** miesiącu, który jest ustawiony w polu `Data` w menu `Funkcje` > `Księguj należności`.
- Pole `Dni wolne od pracy` > ustalamy czy system ma przesuwać docelowy termin płatności, jeśli wypada on w dzień wolny od pracy.
- Klikamy: `Dodaj`.
- Klikamy: `Zatwierdź`.

Przykład z animacji poniżej, poprawiamy dni z 14 na 9, dzięki temu docelowy termin płatności zaliczek będzie na dziesiątego dnia miesiąca. Bazowy termin płatności na 20RR-MM-**01** + **9** dni = 20RR-MM-**10**.

Jeśli zachodzi potrzeba ustawienia terminu płatności **zawsze** na koniec miesiąca, to pola definiujemy następująco:

 - Pole `Dni` > -1.
 - Pole `Data bazowa` > `Początek następnego miesiąca`.
 - Pole `Dni wolne od pracy` > `Nie przesuwaj`.

**Prosimy zawsze sprawdzać termin płatności po zaksięgowaniu obciążenia. Ma on bezpośredni wpływ na saldo i rozrachunki właściciela oraz na naliczające się odsetki.**

![Terminy płatności](terplatnosci.gif)