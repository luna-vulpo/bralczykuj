---
description: Popraw polski tekst według Bralczykuja (tryb edycji)
argument-hint: "[styl=interfejs|instruktarz|urzędowy|dokumentacja] [ustawienia] <tekst albo ścieżka pliku>"
---

Użyj skilla `bralczykuj` w trybie **edycji** na: $ARGUMENTS

Gdy $ARGUMENTS zaczyna się od `styl=…` lub innych par `klucz=wartość` (`limit=`, `forma=`, `numeracja=`, `zdanie=`, `kropka=`, `terminy=`), potraktuj je jako wybór stylu i ustawienia według `references/style.md`, a resztę jako tekst. Bez `styl=` rozpoznaj styl według sekcji „Rozpoznawanie”.

Gdy pozostała część $ARGUMENTS to ścieżka pliku, przeczytaj plik i popraw go na miejscu, z nagłówkami YAML, kodem i tabelami nietkniętymi. Gdy $ARGUMENTS jest puste, poproś o wklejenie tekstu.
Przed oddaniem wyniku przejdź `references/eval.md` i listę kontrolną z `references/nadpisania.md`.
