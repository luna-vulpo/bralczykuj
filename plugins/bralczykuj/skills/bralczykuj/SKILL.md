---
name: bralczykuj
description: Redakcja polskiego tekstu według Miodkuja, uzupełniona o reguły użytkownika — rozkaźnik w poleceniach, strona bierna i „należy” w opisach, bez zbędnych zaimków wskazujących, bez „być”, „nikt” i „po cichu”, dokument nigdy jako podmiot czynności. Używać przy każdym polskim tekście interfejsu, pomocy, komunikatów, dokumentów i protokołów; przy prośbach „bralczykuj”, „popraw styl”, „napisz po ludzku”, „usuń slop”, „uprość”.
---

# Bralczykuj

Bralczykuj to Miodkuj z regułami użytkownika położonymi na wierzch. Rdzeń, tryby, przebieg
pracy i kontrola jakości pochodzą z Miodkuja (`references/`). Reguły z sekcji „Reguły
nadrzędne” i plik `references/nadpisania.md` **wygrywają z każdym plikiem Miodkuja**, gdy
mówią co innego.

## Zasada główna

Poprawka ma być najmniejsza z wystarczających. Myśl autora, jego głos, układ i celowe
nieregularności zostają; usuwane są wzorce sztucznej polszczyzny, mgła urzędowa, kalki,
powtórzenia i miejsca niejasne.

Bez zmian zostają: sens, fakty, zastrzeżenia, nazwy, liczby, daty, odnośniki, przywołania
przepisów i norm, cytaty, kod, wstawki w rodzaju `$zmienna` i `${…}`, nazwy produktów, nazwy
pól interfejsu w cudzysłowach. Niczego się nie dopisuje: ani przykładu, ani liczby, ani
skutku, którego nie ma w źródle.

## Reguły nadrzędne

Kolejność odpowiada wadze. Szczegóły, przykłady i wyjątki: `references/nadpisania.md`.

1. **Polecenie dla czytelnika — tryb rozkazujący.** „Wpisz numer z tabliczki”, nie „numer
   wpisuje się”.
2. **W poleceniu wielozdaniowym każde zdanie zaczyna się od czasownika.** „Przepisz numer
   budynku z tabliczki”, nie „Numer budynku przepisz z tabliczki”.
3. **Opis (nie polecenie) — strona bierna albo „należy” przed formą z „się”.** „Parametry
   należy potwierdzić”, nie „parametry potwierdza się”. Bez drugiej osoby w opisach:
   „Twoje” → „wykonującego”. Bez ciężkich łańcuchów w rodzaju „zostaje dokonane”.
4. **Martwy obiekt nie wykonuje czynności.** Dokument, protokół, książka, artykuł, ustawa,
   norma, tablica, przepis, ekran ani plik nie pisze, nie czyta, nie podaje, nie mówi, nie
   wskazuje, nie każe, nie przewiduje, nie dopuszcza, nie wymaga — zawsze strona bierna:
   „jest napisane”, „podano”, „w normie wymagane jest”. Złożona maszyna (aplikacja, komputer,
   miernik, urządzenie) może działać: „komputer policzył”, ale „na ekranie komputera jest
   napisane”. Części aplikacji (terminarz, biblioteka, ścieżka pomiarowa, pole, lista, sekcja)
   nie są maszyną. W razie wątpliwości — strona bierna. Zamiast „X daje wpis” — „X powoduje
   wpis”; zamiast „wpis informuje” — „brak zalecenia oznacza, że…”. Czasowniki relacji („zawiera”, „obejmuje”, „dotyczy”) dopuszczalne; w stylu
   urzędowym strona bierna: „Nie jest objęte zakresem kontroli”.
5. **Bez „nikt”.** „Nie potwierdzono go” albo „nie został potwierdzony”, nie „nikt go nie
   potwierdził”.
6. **Bez „po cichu”, „cicho”, „cichy sukces”.** Opisuje się wprost, co się dzieje albo czego
   brakuje.
7. **Bez „stoi”, „stanie”, „staną”, „leży”, „leżą” w znaczeniu położenia.** „Jest”, „znajduje się”,
   „widnieje”, „pojawi się”, „zostanie wpisane” — według kontekstu.
8. **Zaimki wskazujące tylko wtedy, gdy coś odróżniają.** „W kontroli”, nie „w tej kontroli”;
   „na ekranie”, nie „na tym ekranie”. Zaimek zostaje, gdy bez niego zmienia się znaczenie.
9. **Zdanie z „być” — równoważnik albo inny czasownik, o ile się da.** „Brak wskazania powoduje
   wpis »nie wskazano«”, nie „bez wskazania będzie wpisane »nie wskazano«”; „Pole
   nieobowiązkowe”, nie „Pole jest nieobowiązkowe”.
10. **Zdanie podrzędne skrócone do frazy.** „Mierniki użyte do wykonania kontroli”, nie
    „mierniki, którymi wykonano tę kontrolę”.
11. **Bez konstrukcji „Zrób raz … dla …”.** „Stan gruntu wskazany nad listą elementów
    obowiązuje całą kontrolę”, nie „Wskaż go raz, dla całej kontroli, nad listą”.
12. **Bez redundancji** — ani dopisanej, ani zostawionej ze źródła: „dzisiaj” bez treści,
    „tego, co jest…” zamiast rzeczownika, powtórzenie tej samej myśli w dwóch zdaniach,
    „właśnie”, „po prostu”, „w ogóle”, „wcale”, oczywistości. Treść merytoryczna, warunki
    i skutki zostają.
13. **Okolicznik zaraz po czasowniku, nie na końcu zdania.** „Bez zmian”, „od razu”,
    „potem”, „wtedy”, „najpierw”, „ponownie” i podobne stoją tuż za czasownikiem, przed
    dopełnieniem: „Zapisz od razu wynik”, nie „Zapisz wynik od razu”. Reguła przesuwa sam
    okolicznik — szyk podmiot–orzeczenie zostaje: „Poprzednie kontrole zostają bez zmian”
    jest poprawne i nie przechodzi w „Zostają bez zmian poprzednie kontrole”.
14. **Bez zbędnych zaimków osobowych.** „Go”, „jej”, „jego”, „ono”, „ich”, „je”, „niego”
    i podobne znikają, gdy z poprzedniego zdania albo członu jasno wynika, o co chodzi:
    „Pole daty puste. Uzupełnij w karcie”, nie „Uzupełnij je w karcie”. Zaimek zostaje, gdy
    bez niego zdanie jest niegramatyczne albo ma dwa możliwe odniesienia.

Przy tekście interfejsu, pomocy i dokumentów reguły 1–14 stosuje się zawsze, z wyjątkami
ustalonymi przez styl. Przy innym gatunku (list, felieton, tekst naukowy) — tylko tam, gdzie
nie łamią rejestru źródła (`references/registers.md`).

## Styl

Styl dopasowuje reguły 1–14 do przeznaczenia tekstu: `interfejs`, `instruktarz`, `urzędowy`,
`dokumentacja` albo `ogólny` (zachowanie 1.0.0). Wybór: argument `styl=…` z ustawieniami
(`limit=40`, `forma=państwo`), słowo w prośbie („w stylu urzędowym”) albo rozpoznanie
automatyczne. Styl może regułę wyłączyć, złagodzić albo zaostrzyć; ochrony treści nie
uchyla. Macierz reguł, profile, ustawienia i przykłady: `references/style.md`.

## Tryby

- **Edycja** (domyślnie): najpierw cały poprawiony tekst. Notatka o zmianach tylko na prośbę
  albo gdy brak danych uniemożliwia bezpieczną poprawkę. Tekst bez wad wraca bez zmian, bez
  komentarza.
- **Audyt** („tylko audyt”, „wskaż problemy”): dla każdej wady nazwa wzorca, cytat, waga
  (czerwona, żółta, zielona) i kierunek poprawki. Bez przepisywania i bez zgadywania, czy tekst
  napisała maszyna.
- **Tryb wbudowany albo plikowy**: gdy skill pracuje na rzecz innego zadania, cały proces
  przebiega wewnętrznie, a wynikiem jest wyłącznie gotowy tekst. Nagłówki YAML, bloki kodu,
  tabele i cele odnośników zostają nietknięte.

## Przebieg

1. Przeczytać całe źródło; ustalić zadanie tekstu, odbiorcę, rejestr i styl
   (`references/style.md`) wraz z ustawieniami z wywołania.
2. Ustalić trzy–pięć cech głosu autora (słownictwo, rytm, formalność, bezpośredniość).
3. Oznaczyć fragmenty chronione (kod, liczby, przywołania, cytaty, nazwy pól).
4. Rozstrzygnąć, które zdania są poleceniem, a które opisem — od tego zależą reguły 1–3.
5. Przejść reguły nadrzędne 1–14 w wersji ustalonej przez styl, potem wzorce Miodkuja (`references/polish-patterns.md`).
6. Drugie przejście: rytm generowany, mgła urzędowa, kalki, ogólniki, nadmiar półpauz.
7. Kontrola jakości: `references/eval.md`, lista kontrolna z `references/nadpisania.md`
   i lista kontrolna stylu z `references/style.md`.
   Wada → jedna poprawka i ponowna kontrola.

## Drabina konkretu (z Miodkuja)

Ogólnik bez oparcia w źródle: (1) użyć faktu ze źródła; (2) złożyć go z informacji ze źródła
bez podnoszenia pewności; (3) zmniejszyć twierdzenie albo je usunąć; (4) gdy brak danych
blokuje poprawkę, zgłosić lukę. Wymyślona liczba, przykład czy skutek jest zakazany, także
gdy brzmi wiarygodnie.

## Materiały

- `references/style.md` — style, macierz reguł 1–14, ustawienia, rozpoznawanie. **Czytać
  zawsze**, także gdy styl nie został wskazany.
- `references/nadpisania.md` — reguły nadrzędne z przykładami, wyjątki, sprzeczności
  z Miodkujem i lista kontrolna. **Czytać zawsze.**
- `references/polish-patterns.md` — wzorce sztucznej polszczyzny i zabezpieczenia przed
  fałszywym alarmem.
- `references/eval.md` — kontrola jakości po każdej edycji i audycie.
- `references/registers.md` — zachowanie zależne od gatunku.
- `references/plain-polish.md` — prosta polszczyzna; **dwie jej zasady uchyla
  `nadpisania.md`** (zwracanie się wprost, ograniczanie strony biernej).
- `references/voice-calibration.md` — przy tekstach osobistych, marketingowych i publicystyce.
- `references/examples.md` — pary przed/po z Miodkuja.

## Częste błędy

- Spłaszczanie każdego tekstu do jednego, wygładzonego tonu.
- Zamiana polecenia na formę z „się” albo bierną (reguła 1 wygrywa z regułą 3).
- Usuwanie zaimka, który odróżnia jedną rzecz od drugiej.
- Zastępowanie terminu technicznego albo prawnego luźnym synonimem.
- Dopisywanie przykładów, danych albo skutków, których nie ma w źródle.
- Półpauza jako domyślny łącznik zdań.
