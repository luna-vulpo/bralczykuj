# Style — profile redakcji zależne od przeznaczenia tekstu

Plik ustala, jak styl tekstu zmienia reguły nadrzędne 1–13 z `nadpisania.md`. Wprowadzony
w wersji 1.1.0.

## Pierwszeństwo

1. Ochrona treści (fakty, liczby, daty, nazwy, cytaty, kod, przywołania przepisów i norm,
   wstawki `$…`, nazwy pól w cudzysłowach). Żaden styl jej nie uchyla.
2. Ustawienia podane w wywołaniu (`limit=40`, `forma=państwo`).
3. Profil stylu z tego pliku.
4. Reguły 1–13 z `nadpisania.md`.
5. Pliki Miodkuja.

## Wybór stylu

- Argument: `styl=interfejs`, `styl=instruktarz`, `styl=urzędowy`, `styl=dokumentacja`,
  `styl=ogólny`.
- Słowo w prośbie: „jak interfejs”, „w stylu urzędowym”, „jako instruktarz”.
- Bez wskazania: rozpoznanie automatyczne (sekcja „Rozpoznawanie”).

Aliasy: `interfejs` = `ui`, `aplikacja`; `instruktarz` = `instrukcja`, `kroki`;
`urzędowy` = `urzedowy`, `pismo`, `oficjalny`; `dokumentacja` = `techniczny`, `docs`.

Styl `ogólny` odpowiada zachowaniu 1.0.0: reguły 1–13 w pełni, reszta według
`registers.md`.

## Macierz reguł

**tak** — reguła obowiązuje. **ostrzej** — reguła zaostrzona (opis w profilu).
**luźniej** — reguła stosowana tylko tam, gdzie nie psuje rejestru. **nie** — reguła
wyłączona.

| Reguła | interfejs | instruktarz | urzędowy | dokumentacja |
| --- | --- | --- | --- | --- |
| 1 rozkaźnik w poleceniu | tak | ostrzej | nie przy obowiązku strony | tak |
| 2 czasownik na początku | tak | ostrzej | luźniej | tak |
| 3 bierna / „należy” w opisie | luźniej | tak | tak, z „się” i „zobowiązany jest” | tak |
| 4 dokument nie działa | tak | tak | tak | luźniej |
| 5 bez „nikt” | tak | tak | tak | tak |
| 6 bez „po cichu” | tak | tak | tak | tak |
| 7 bez „stoi/stanie” | tak | tak | tak | tak |
| 8 zaimki wskazujące | ostrzej | tak | luźniej | tak |
| 9 „być” → równoważnik | ostrzej | tak | nie | luźniej |
| 10 podrzędne → fraza | ostrzej | tak | luźniej | tak |
| 11 bez „raz … dla” | tak | tak | tak | tak |
| 12 bez redundancji | ostrzej | tak | luźniej | tak |
| 13 okolicznik po czasowniku | tak | ostrzej | luźniej | tak |

## interfejs

Przeznaczenie: przyciski, etykiety pól, podpowiedzi, puste stany, komunikaty błędów
i potwierdzeń.

- Przycisk: rozkaźnik albo rzeczownik, bez kropki.
- Etykieta pola: rzeczownik albo fraza, bez czasownika.
- Komunikat błędu: najpierw co się stało, potem co zrobić; bez przeprosin i wykrzyknień.
- Potwierdzenie: równoważnik.
- Ta sama czynność nosi tę samą nazwę w całym tekście.
- Wielkość liter jak w źródle. Przycisk i nagłówek sekcji zapisane wersalikami zostają
  wersalikami także po poprawce („ZAPISZ DATY”); wersalików nie dodaje się ani nie usuwa.
- Wstawka (`%1$s`, `%2$d`, `{0}`) zostaje w tym samym miejscu względem słów, z którymi się
  uzgadnia. Wstawka wypełniana rzeczownikiem z `plurals` stoi po liczbie, a przypadek słów
  wokół niej musi pasować do każdej formy z `plurals`; gdy poprawka tego nie zapewnia,
  wstawka zostaje bez zmian, a wada zostaje zgłoszona.
- Reguła 3 luźniej: w opisie równoważnik ma pierwszeństwo przed „należy”.
- Reguły 8, 9, 10, 12 ostrzej: każde słowo bez treści zostaje usunięte.

Ustawienia: `forma=rozkaźnik` (albo `bezokolicznik`), `limit=brak` (liczba znaków na
tekst; przekroczenie → skrócić, a gdy skrót zmienia sens — zgłosić), `limit_opis=160`
(liczba znaków opisu pod przełącznikiem, kafelkiem albo nagłówkiem; przekroczenie to
ostrzeżenie w audycie, a w edycji — skrót tylko bez utraty warunku lub skutku),
`kropka=tylko-zdania`.

| Źle | Dobrze |
| --- | --- |
| Kliknij tutaj, aby zapisać wprowadzone dane | Zapisz |
| Przepraszamy! Wystąpił błąd podczas zapisywania. | Nie zapisano pomiaru. Sprawdź połączenie i spróbuj ponownie. |
| Ten pomiar został pomyślnie zapisany. | Zapisano pomiar |
| Pole to jest wymagane | Pole wymagane |
| ZAPISZ wprowadzone daty | ZAPISZ DATY |

## instruktarz

Przeznaczenie: procedury, kroki, pomoc krok po kroku.

- Reguła 1 ostrzej: także pierwsze zdanie wstępu bez „należy”, gdy jest poleceniem.
- Reguła 2 ostrzej: każdy krok zaczyna się od czasownika w rozkaźniku.
- Reguła 13 ostrzej: bez wyjątku dla okoliczników czasu i kolejności.
- Jeden krok zawiera jedną czynność; krok z dwiema czynnościami należy rozdzielić.
- Ostrzeżenie stoi przed krokiem, którego dotyczy.
- Wynik kroku jako osobne zdanie opisowe (reguła 3).

Ustawienia: `forma=rozkaźnik`, `numeracja=tak`, `zdanie=20` (liczba słów; przekroczenie
to ostrzeżenie, nie twarda granica).

| Źle | Dobrze |
| --- | --- |
| Następnie należy otworzyć rozdzielnicę i odczytać oznaczenia. | 1. Otwórz rozdzielnicę. 2. Odczytaj oznaczenia aparatów. |
| Wyłącz zasilanie, bo inaczej grozi porażenie. | Uwaga: grozi porażenie. 1. Wyłącz zasilanie. |

## urzędowy

Przeznaczenie: pisma, wnioski, protokoły, regulaminy, korespondencja z urzędem.

- Reguła 1 wyłączona przy obowiązku strony: obowiązek przypisany nazwanemu podmiotowi,
  bez rozkaźnika („Wnioskodawca składa…”). Rozkaźnik zostaje w pouczeniach skierowanych
  wprost do adresata, gdy tak jest w źródle.
- Reguła 3: dopuszczalne „się” i „zobowiązany jest”; moc prawna bez zmian.
- Reguła 9 wyłączona: „jest”, „są” zostają.
- Reguły 2, 8, 10, 12, 13 luźniej: formuły wymagane procedurą zostają
  („Na podstawie art. …”, „W odpowiedzi na pismo z dnia …”, „niniejszym” w formule
  oświadczenia).
- Cięcia mgły urzędowej według `registers.md` poza formułami.

Ustawienia: `forma=państwo` (albo `pan-pani`, `bezosobowa`).

| Źle | Dobrze |
| --- | --- |
| Masz 14 dni na złożenie oświadczenia. | Wnioskodawca składa oświadczenie w terminie 14 dni. |
| W zakresie realizacji projektu dokonano zakupu serwera. | W ramach projektu kupiono serwer. |
| Wniosek kompletny. (równoważnik w piśmie) | Wniosek jest kompletny. |

## dokumentacja

Przeznaczenie: dokumentacja produktu i API, opisy zmian w wersjach, notatki techniczne.

- Reguła 4 luźniej: system, funkcja, API, moduł mogą być podmiotem („Funkcja zwraca
  listę”); dokument nadal nie.
- Reguła 9 luźniej: definicja zachowuje „jest”, gdy równoważnik zaciera definicję.
- Terminy, nazwy kluczy, komendy, komunikaty błędów i numery wersji zostają dosłownie.

Ustawienia: `forma=rozkaźnik`, `terminy=bez-zmian`.

| Źle | Dobrze |
| --- | --- |
| Ta metoda po cichu zwraca null. | Metoda zwraca `null` bez zgłoszenia błędu. |
| README mówi, jak to uruchomić. | Sposób uruchomienia opisano w `README`. |

## Rozpoznawanie

| Sygnał w źródle | Styl |
| --- | --- |
| `strings.xml`, plik `*.json` z kluczami tekstów, krótkie frazy bez kropek | interfejs |
| lista numerowana zaczynana czasownikami | instruktarz |
| „art.”, „ust.”, „Szanowni Państwo”, „wnioskodawca”, sygnatura pisma | urzędowy |
| bloki kodu, nazwy funkcji, `README`, `CHANGELOG` | dokumentacja |
| brak sygnału albo sygnały sprzeczne | ogólny |

W tekście mieszanym styl należy dobrać osobno dla każdego fragmentu.

## Lista kontrolna stylu

- Czy styl wybrano z argumentu, z prośby albo z rozpoznania i czy zgadza się z tekstem?
- Czy reguły wyłączone w stylu nie zostały mimo to zastosowane?
- Czy spełniono ustawienia (`limit`, `limit_opis`, `forma`, `numeracja`, `zdanie`)?
- Czy wielkość liter i położenie wstawek zgadzają się ze źródłem?
- Czy ochrona treści pozostała nienaruszona?
