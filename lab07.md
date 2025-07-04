# Języki Programowania - Lab07 - TN

Prowadzący: [dr inż. Tomasz Kubik](http://tomasz.kubik.staff.iiar.pwr.wroc.pl/)

## Rozwiązania

- [Dominik Pokrzywa](https://github.com/Ite-2022-pwr/sem3-jp-lab07-dp)
- [Miłosz Bedryło](https://github.com/Ite-2022-pwr/sem3-jp-lab07-mb)
- [Artur Kręgiel](https://github.com/Ite-2022-pwr/sem3-jp-lab07-ak)
- [Dawid Jabłoński](https://github.com/Ite-2022-pwr/sem3-jp-lab-dj/tree/master/Labolatoria%207)

## Treść Zadania

Laboratorium 7, TN Podczas laboratorium należy zbudować aplikację działającą w środowisku rozproszonym, wykorzystującą technologię RMI. Dokładniej - należy zaimlementować mały systemu, w którego skład wejdą podsystemy uruchamiane równolegle.

Zakładamy, że system będzie pełnić podobną rolę jak w opisie z laboratorium 6. Będzie to symulator sklepu stacjonarnego, w którym klienci zamawiają towary za pośrednictwem terminali, zaś pracownicy sklepu zajmują się dostarczeniem i sprzedażą towarów według tych zamówień. Częściami tego systemu mają być podsystemy:

- Magazynier (Keeper) implementujący interfejs IKeeper
- Dostawca (Deliverer) implementujący interfejs Deliverer
- Sprzedawca (Seller) implementujący interfejs ISeller
- Klient (Client) implementujący interfejs IClient

Główna różnica w specyfikacji zadania w porównaniu z poprzednim laboratorium polega na tym, że wywołania metod register() i unregister() interfejsu IKeeper mają być synchroniczne (wcześniej były asynchroniczne). Ponadto zniesiono konieczność korzystania z metody getInfo().

Wykorzystywane interfejsy oraz typ wyliczeniowy zostały zdefiniowane w załączonym do zadania pliku jar. Plik ten należy wykorzystać jako obowiązkową zależność we własnym projekcie.

Pozostałe szczegóły mają być zgodne z ustaleniami poczynionymi na początku zajęć.
