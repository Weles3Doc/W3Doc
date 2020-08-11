# Terminy płatności

Podczas księgowania należności nie określamy bezpośrednio terminu płatności dokumentów. Docelowy termin płatności będzie sumą ustawionej daty Pole Bazowy termin płatności oraz ilości dni określonej w niżej opisywanej funkcji. Dodatkowo będzie zależał od ustawionych opcji.  Aby ustawić ilość dni doliczanych podczas księgowania, należy przejść do:

- Zakładka `Administracja` > menu `Elementy` > `Terminy płatności`.
- Pole `Dokument` > wybrać typ dokumentu, dla którego ustawiamy termin.
- Pole `Właściciel` > można wybrać osobę, dla której określimy indywidualny termin. Jeśli pozostanie wybrane BRAK, pozycja będzie dotyczyła wszystkich.
- Pole `Dni` > określamy ilość dni, która doda się do daty bazowej określanej przy księgowaniu należności i następnym polu.
- Pole `Data bazowa` > określamy, co ma być datą podstawową:
  - `Bazowy termin płatności` > określany przy księgowaniu należności.
  - `Początek miesiąca` > pierwszy dzień miesiąca, w którym są księgowane należności.
  - `Początek następnego miesiąca` > Pierwszy dzień miesiąca po miesiącu, w którym są księgowane należności.
- Pole `Dni wolne od pracy` > ustalamy czy system ma przesuwać docelowy termin płatności, jeśli wypada on w dzień wolny od pracy.
- Klikamy: `Dodaj`.
- Wpisujemy hasło i zatwierdzamy.

Przykład z animacji poniżej, poprawiamy dni z 14 na 9, dzięki temu docelowy termin płatności zaliczek lipcowych będzie na dziesiątego dnia miesiąca. (bazowy termin płatności na 2012-07-01 + 9 dni)

![Terminy płatności](tp.gif)