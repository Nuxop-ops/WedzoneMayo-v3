# Wędzone Mayo v3

Klikalna aplikacja w czerni i złocie. Bez Replit i bez instalowania zależności.

## Uruchomienie w Codex

Wybierz repozytorium `Nuxop-ops/WedzoneMayo-v3` w środowisku Codex. W katalogu repozytorium uruchom:

```sh
python3 -m http.server 3000 --bind 0.0.0.0
```

Otwórz podgląd portu 3000. Można również pobrać `index.html` i otworzyć go bezpośrednio w przeglądarce.

## Funkcje

- Pulpit, Zamówienia, Etykiety, Klienci, Produkty, Ustawienia.
- Nowe / Zamówione → W realizacji (Poczta / Dowóz) → Zrealizowane; wyszukiwanie po kliencie, numerze i telefonie.
- Poczta: wymagane potwierdzenie Zapłacone przed ważeniem. Próba ważenia otwiera komunikat.
- Ważenie i realizacja w jednej karcie. Każdy produkt wymaga dodatniej rzeczywistej wagi przed zatwierdzeniem.
- Kiełbasa: pętka lub kg. Pozostałe produkty, w tym polędwiczka: sztuki lub kg. Rozliczenie według wagi i ceny za kg. Cena jest zapamiętana przy złożeniu nowego zamówienia.
- Zatwierdzenie dodaje etykietę dla każdej pozycji zamówienia do kolejki. Nagłówki i treść są edytowalne.
- Arkusz A4: 2 kolumny i 4 wiersze, marginesy 10 mm. Zaznacz już zużyte miejsca. Druk w skali 100%, bez nagłówków i stopek. Po udanym druku osobno potwierdź zużycie pól. Anulowanie druku nie usuwa etykiet.
- Dodawanie i edycja klientów oraz produktów; historia zamówień klienta.
- Zapis w localStorage i eksport kopii JSON w Ustawieniach.

## Dane i ograniczenia

Dane startowe są demonstracyjne. To wersja lokalna: dane pozostają w bieżącej przeglądarce, bez synchronizacji i serwera bazy danych. Usunięcie danych witryny usuwa lokalne zamówienia. Pobieraj kopie JSON. Aplikacja nie zawiera importera kopii.

Napis marki jest odtworzony typograficznie. Oryginalny plik logo z rozmowy nie był dostępny do wgrania w środowisku.

## Weryfikacja

Składnia JavaScript sprawdzona podczas tworzenia. Testy interakcji i wydruku w przeglądarce pozostają do wykonania: środowisko Codex zgłaszało `repository_access_denied` i nie uruchomiło podglądu.
