# Bralczykuj

Plugin Claude Code do redakcji polskiego tekstu. Rdzeniem jest [Miodkuj](https://github.com/bartekpucek/miodkuj) Bartka Pucka; na wierzchu leży trzynaście reguł nadrzędnych, które wygrywają z Miodkujem przy każdej sprzeczności.

Reguły powstały przy redakcji tekstów interfejsu, pomocy i dokumentów aplikacji technicznej, stąd przykłady z instalacji elektrycznych. Przy liście, felietonie czy tekście naukowym działają tylko tam, gdzie nie łamią rejestru źródła.

## Instalacja

```
/plugin marketplace add luna-vulpo/bralczykuj
/plugin install bralczykuj@bralczykuj
```

## Użycie

- `/bralczykuj <tekst albo plik>`: poprawiony tekst, bez listy zmian.
- `/bralczykuj-audyt <tekst albo plik>`: wady z cytatem, wagą i kierunkiem poprawki, bez przepisywania.
- Albo zwykła prośba: „bralczykuj”, „popraw styl”, „usuń slop”.

## Reguły nadrzędne w skrócie

1. Polecenie dla czytelnika w trybie rozkazującym.
2. W poleceniu wielozdaniowym każde zdanie zaczyna się od czasownika.
3. Opis: strona bierna albo „należy” przed formą z „się”; bez drugiej osoby.
4. Dokument, ekran ani plik nie wykonuje czynności człowieka.
5. Bez „nikt”.
6. Bez „po cichu”, „cicho”, „cichy sukces”.
7. Bez „stoi”, „stanie” w znaczeniu położenia.
8. Zaimek wskazujący tylko wtedy, gdy coś odróżnia.
9. Zdanie z „być” zamienione na równoważnik albo inny czasownik, o ile się da.
10. Zdanie podrzędne skrócone do frazy.
11. Bez konstrukcji „Zrób raz … dla …”.
12. Bez redundancji.
13. Okolicznik zaraz po czasowniku.

Przykłady, wyjątki i lista kontrolna znajdują się w `references/nadpisania.md`.

## Układ

```
.claude-plugin/marketplace.json
plugins/bralczykuj/
  .claude-plugin/plugin.json
  commands/bralczykuj.md, bralczykuj-audyt.md
  skills/bralczykuj/SKILL.md
  skills/bralczykuj/references/nadpisania.md     reguły nadrzędne
  skills/bralczykuj/references/*.md              pliki Miodkuja 2.1.1 bez zmian
```

## Licencja

MIT. Pliki `eval.md`, `examples.md`, `plain-polish.md`, `polish-patterns.md`, `registers.md` i `voice-calibration.md` pochodzą bez zmian z Miodkuja 2.1.1 (MIT, Bartek Pucek).

Plugin współpracuje z [stop-slop-plus](https://github.com/luna-vulpo/stop-slop-plus), który przy polskim tekście oddaje pracę Bralczykujowi.
