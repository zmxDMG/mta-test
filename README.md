# Wybuch czerwonego auta — prototyp MTA

Mały eksperyment w Lua dla Multi Theft Auto: skrypt klienta szuka elementu o ID `redCar`, sprawdza odległość lokalnego gracza i przy dystansie mniejszym niż 5 jednostek wywołuje zdarzenie, które ma uruchomić wybuch auta.

## Zawartość

- `.idea/wybuch.lua` — skrypt klienta: sprawdzanie odległości co 100 ms i obsługa zdarzenia wybuchu.
- `.idea/meta.xml` — szkic manifestu zasobu, który deklaruje skrypt jako klientowy.

## Ważny stan projektu

To nie jest obecnie gotowy zasób MTA. Oba pliki zasobu znajdują się w `.idea/`, a `meta.xml` odwołuje się do `wybuch.lua` ścieżką względną. Przed testem w MTA trzeba przenieść pliki do katalogu zasobu i poprawnie rozdzielić logikę klienta i serwera. W obecnym manifeście nie ma osobnego skryptu serwerowego, mimo że kod wywołuje zdarzenie sieciowe.

Projekt nie zawiera skryptu instalacyjnego ani testów.

## Licencja

Zobacz [LICENSE.txt](LICENSE.txt).
