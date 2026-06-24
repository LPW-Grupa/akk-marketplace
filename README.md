# akk-marketplace — wspólny katalog paczek AKK

To jest **marketplace** (spis paczek), z którego zespół instaluje narzędzia AKK. W praktyce to osobne repozytorium Git zawierające plik `.claude-plugin/marketplace.json`.

## Co tu jest

- `.claude-plugin/marketplace.json` — spis paczek i adresy ich repozytoriów (`source`).

## Jak używać (zespół)

```
/plugin marketplace add LPW-Grupa/akk-marketplace
/plugin install akk-generator@akk-marketplace
```

## Jak dodać/zmienić paczkę

Edytujesz `marketplace.json` — dopisujesz wpis `{ "name": ..., "source": <adres repo paczki> }`. Każda paczka ma własne repozytorium z plikiem `.claude-plugin/plugin.json`.

> Układ docelowy: **jedno repo `LPW-Grupa/akk-marketplace`** zawierające ten plik oraz paczkę w podfolderze `akk-generator/`. Dlatego `source` to ścieżka względna `./akk-generator` (a nie osobny adres repo). Jeśli w przyszłości paczka dostanie własne repozytorium, zmień `source` na `LPW-Grupa/akk-generator`.
