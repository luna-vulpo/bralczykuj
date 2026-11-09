---
description: Wskaż wady polskiego tekstu bez przepisywania (tryb audytu)
argument-hint: "[styl=interfejs|instruktarz|urzędowy|dokumentacja] [ustawienia] <tekst albo ścieżka pliku>"
---

Użyj skilla `bralczykuj` w trybie **audytu** na: $ARGUMENTS

Gdy $ARGUMENTS zaczyna się od `styl=…` lub innych par `klucz=wartość` (`limit=`, `forma=`, `numeracja=`, `zdanie=`, `kropka=`, `terminy=`), potraktuj je jako wybór stylu i ustawienia według `references/style.md`, a resztę jako tekst. Bez `styl=` rozpoznaj styl według sekcji „Rozpoznawanie”.

Gdy pozostała część $ARGUMENTS to ścieżka pliku, przeczytaj plik. Gdy $ARGUMENTS jest puste, poproś o wklejenie tekstu.
Nie przepisuj tekstu. Dla każdej wady podaj nazwę wzorca albo numer reguły nadrzędnej, cytat, wagę (czerwona, żółta, zielona) i kierunek poprawki. Na końcu zaproponuj edycję.
