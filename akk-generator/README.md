# akk-generator — paczka agentów AKK

Zespół agentów do **Analizy Kosztów i Korzyści (AKK/CBA)** dla projektów dofinansowanych z funduszy UE 2021–2027.

> ## 🧪 WERSJA ALPHA — zakres testów
>
> **Ta paczka jest w trakcie budowy. Służy WYŁĄCZNIE do testowania przepływu i UX — NIE do przygotowania realnych wniosków o dofinansowanie.**
>
> **Co testujemy na tym etapie (Etapy 0 → 1b):**
> - inicjalizację sesji i dialog orkiestratora (Etap 0),
> - zakładkę „Dane wejściowe i założenia" (Etap 0a, `input-assumptions-analyst`),
> - klasyfikację budżetu (Etap 1a, `budget-classifier`),
> - model amortyzacji (Etap 1b, `depreciation-model-agent`).
>
> **Czego NIE testujemy (jeszcze nie zbudowane):** Etapy 1c–4 (przychody/koszty, wskaźniki finansowe, analiza ekonomiczna, wrażliwość/ryzyko, trwałość). Po punkcie kontrolnym **PK-1b proces należy zatrzymać** — kolejne subagenty to szkielety bez metodyki i nie wygenerują poprawnych zakładek.
>
> **Czego oczekujemy od testerów:** uwag o czytelności dialogu, punktach kontrolnych, jakości 3 pierwszych zakładek i ergonomii pracy z orkiestratorem. ⚠️ Nie używaj wyników w realnej dokumentacji konkursowej.

## Jak to działa

`akk-konfigurator` (orkiestrator) prowadzi Analityka przez cały proces (Etapy 0–5), wywołuje subagentów wykonawczych i zatrzymuje się na każdym punkcie kontrolnym do decyzji Analityka. Każdy subagent pisze jedną zakładkę modelu Excel.

## Zawartość

| Plik agenta | Etap | Zakładka Excel | Status |
|-------------|------|----------------|--------|
| `agents/akk-konfigurator.md` | orkiestrator | Etap 0 i 5 / Zestawienie zbiorcze | ✅ Gotowy |
| `agents/input-assumptions-analyst.md` | 0a | Dane wejściowe i założenia | ✅ Gotowy |
| `agents/budget-classifier.md` | 1a | Budżet | 🟡 Wersja robocza |
| `agents/depreciation-model-agent.md` | 1b | Majątek i amortyzacja | 🟡 Wersja robocza |
| `agents/revenue-opex-agent.md` | 1c | Przychody i koszty | 🔲 Szkielet do napisania |
| `agents/financial-indicators-agent.md` | 1d | Wskaźniki finansowe | 🔲 Szkielet do napisania |
| `agents/economic-analysis-agent.md` | 2 | Analiza ekonomiczna | 🔲 Szkielet do napisania |
| `agents/sensitivity-risk-agent.md` | 3 | Wrażliwość i ryzyko | 🔲 Szkielet do napisania |
| `agents/sustainability-agent.md` | 4 | Trwałość finansowa | 🔲 Szkielet do napisania |
| `skills/akk-wiedza/SKILL.md` | — | wspólna baza wiedzy | ✅ Gotowy (samowystarczalny) |

## Instalacja (dla zespołu)

```
/plugin marketplace add LPW-Grupa/akk-marketplace
/plugin install akk-generator@akk-marketplace
```

## Aktualizacja

W fazie alpha `version` w `plugin.json` jest pominięte (lub stałe) — Claude Code używa wtedy commit SHA jako wersji, więc **każdy `git push` do repo udostępnia testerom aktualizację**.

1. Wgraj zmiany do repozytorium `LPW-Grupa/akk-marketplace`.
2. Zespół: `/plugin update akk-generator` (lub `--force` przy wymuszeniu).

> Gdy paczka dojrzeje, przejdź na jawne wersjonowanie: ustaw `version` w `plugin.json` i podnoś je zgodnie z semver — wtedy testerzy dostają aktualizacje tylko po bumpie wersji.

## Status

Wersja `0.1.0` (alpha) — szkielet wdrożeniowy do testów przepływu. Dwa agenty gotowe (orkiestrator, `input-assumptions-analyst`), dwa w wersji roboczej (`budget-classifier`, `depreciation-model-agent`), pięć jako szkielety do napisania (Etapy 1c–4). Baza wiedzy `akk-wiedza` — gotowa i samowystarczalna. Testowalny zakres end-to-end: Etapy 0 → 1b (patrz banner u góry). Szczegóły i plan w `Plan_wdrozenia_AKK_marketplace.md` (folder projektu).
