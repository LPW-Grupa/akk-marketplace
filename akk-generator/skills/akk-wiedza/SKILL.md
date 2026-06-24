---
name: akk-wiedza
description: Wspólna baza wiedzy o procesie Analizy Kosztów i Korzyści (AKK/CBA) dla projektów UE 2021–2027 — proces krok po kroku (Fazy 0–9), osie decyzyjne (punkty krytyczne), podstawy prawne. Używana przez orkiestrator i subagentów AKK jako referencja merytoryczna.
---

# Wiedza referencyjna: proces AKK

Ta umiejętność dostarcza wspólnej, niezmiennej bazy merytorycznej dla wszystkich agentów paczki `akk-generator`. Treść opisuje „co i dlaczego", nie „ile" — wartości liczbowe (progi, stopy dyskontowe, horyzonty sektorowe, stawki) zawsze pochodzą z dokumentacji konkretnego naboru i nie są tu podawane.

## Zasada przewodnia

Jeden proces, skończona liczba wariantów strukturalnych. To, co „inne w każdym wniosku", to dane (liczby) — nie szkielet procesu. Zmienne strukturalne (osie decyzyjne) zmieniają etykiety i parametry kroków, nigdy sam szkielet. Konkretyzację osiągasz, przechodząc przez pytania kontrolne (część A) i drzewo decyzyjne (część B).

**Dla kogo.** Pracownik samorządu, spółki komunalnej lub zakładu budżetowego, także bez wykształcenia ekonomicznego.

## Najważniejsze dokumenty źródłowe

- **Wytyczne MFiPR/2021-2027/15(1)** dotyczące zagadnień związanych z przygotowaniem projektów inwestycyjnych, w tym hybrydowych, na lata 2021–2027 (M.P. 2023 poz. 292) — podstawowy dokument krajowy. Zawiera m.in. załącznik z kategoriami przepływów i wzorami wskaźników oraz załącznik z zakresem studium wykonalności.
- **Rozporządzenie (UE) 2021/1060** (tzw. rozporządzenie ogólne / CPR), w szczególności **art. 67** dotyczący operacji generujących dochód po ukończeniu.
- **Przewodnik KE do AKK** (Guide to Cost-Benefit Analysis of Investment Projects) oraz **Economic Appraisal Vademecum 2021–2027** — metodyka unijna.
- **Niebieskie Księgi (CUPT)** — metodyki sektorowe dla transportu (drogi, kolej).
- **Instrukcja wypełniania wniosku (SWI)** i **regulamin wyboru projektów** danego naboru — to one ostatecznie decydują o wymaganym zakresie i formacie analizy.

> ⚠️ **Zmiana wobec perspektywy 2014–2020.** Zniknęła odrębna unijna procedura zatwierdzania „dużych projektów" (dawny próg 50 mln EUR / 75 mln EUR z rozp. 1303/2013 i 2015/207). W okresie 2021–2027 to **program i instrukcja naboru** określają, dla jakich projektów wymagana jest pełna AKK, a dla jakich wersja uproszczona. Nie zakładaj automatycznie dawnych progów — **[do weryfikacji w SWI danego naboru]**.

Materiały uzupełniające w repozytorium projektu (poza paczką): `AKK_definicje_krokow.docx` (słownikowe definicje kroków), `AKK_jeden_proces.html` (interaktywna wizualizacja procesu i osi decyzyjnych).

---

# A. Proces krok po kroku

Każda faza kończy się **pytaniem kontrolnym** — odpowiedz na nie, zanim przejdziesz dalej, bo odpowiedź często wyznacza inną gałąź modelu (szczegóły w części B).

### Faza 0. Ustal wymagany zakres i format analizy

Zanim cokolwiek policzysz, sprawdź w regulaminie naboru i w instrukcji wypełniania wniosku (SWI), **jakiego dokumentu instytucja w ogóle oczekuje**: pełnej AKK, uproszczonej analizy, studium wykonalności z elementami AKK, czy tylko analizy finansowej. Sprawdź też, czy instytucja narzuca własny wzór arkusza, wymagany horyzont, stopy dyskontowe i metodę ustalania dofinansowania. Ten krok decyduje o nakładzie pracy w całym procesie.

> **Pytanie kontrolne:** *Jakiego dokumentu i jakiego zakresu analizy wymaga regulamin tego konkretnego naboru — pełnej AKK czy wersji uproszczonej?* Jeśli nie wiesz — to pierwsza rzecz do wyjaśnienia z instytucją; reszta procesu od tego zależy.

### Faza 1. Zdefiniuj projekt, cele i kontekst (analiza popytu)

Opisz problem, który projekt rozwiązuje, jego cele, lokalizację i obszar oddziaływania, oraz to, kto i w jakiej skali będzie korzystał z efektów (analiza popytu/potrzeb). Najważniejsze jest rzetelne opisanie **stanu „bez projektu"** — co się stanie, jeśli inwestycji nie będzie. To punkt odniesienia dla wszystkich dalszych obliczeń; zawyżony albo zaniżony stan bazowy zniekształca cały wynik.

> **Pytanie kontrolne:** *Czy jednoznacznie opisałem stan „bez projektu" (wariant bazowy), do którego będę porównywał efekty inwestycji?*

### Faza 2. Przeanalizuj warianty (analiza opcji)

Porównaj realistyczne sposoby osiągnięcia celu — minimum wariant bazowy „bez inwestycji" oraz przynajmniej dwa warianty inwestycyjne różniące się zakresem lub technologią. Celem jest **uzasadnienie wyboru wariantu rekomendowanego**: nie najtańszego i nie najdroższego, lecz najlepiej godzącego nakłady z efektami. Jeśli korzyści da się wyrazić w pieniądzu, warianty porównuje się metodą AKK; jeśli nie — metodą efektywności kosztowej (CEA), czyli kosztem na jednostkę efektu (patrz Faza 6 i oś nr 8 w części B).

> **Pytanie kontrolne:** *Czy porównałem co najmniej dwa warianty inwestycyjne ze stanem bazowym i potrafię obronić, dlaczego rekomenduję właśnie ten?*

### Faza 3. Przyjmij założenia ogólne analizy

Ustal wspólne dla całego modelu założenia: okres odniesienia (horyzont analizy — różny dla różnych sektorów), ceny stałe czy bieżące, stopy dyskontowe (finansową i — jeśli robisz analizę ekonomiczną — społeczną), oraz sposób traktowania VAT. Wartości tych parametrów bierz z wytycznych MFiPR i instrukcji naboru, nie wymyślaj ich **[konkretne wartości do weryfikacji w aktualnych wytycznych]**. Kluczowe rozstrzygnięcie na tym etapie dotyczy VAT.

> **Pytanie kontrolne:** *Czy podmiot ma prawo odzyskać VAT?* Jeśli **tak** — w analizie posługujesz się kwotami netto, a VAT jest kosztem niekwalifikowalnym. Jeśli **nie** — VAT może być kosztem kwalifikowalnym i wchodzi do nakładów. Błąd tu zmienia zarówno koszt projektu, jak i kwotę dofinansowania.

### Faza 4. Zbuduj analizę finansową

Zestaw nakłady inwestycyjne (CAPEX), koszty operacyjne i odtworzeniowe (OPEX) oraz ewentualne przychody w całym okresie odniesienia, a następnie wylicz przepływy pieniężne i finansowe wskaźniki efektywności. Najważniejsze rozstrzygnięcie: czy projekt **generuje dochód** (przychody netto), bo to wyznacza dalszą ścieżkę ustalania dofinansowania.

> **Pytanie kontrolne:** *Czy z infrastruktury lub usług powstałych w projekcie będą pobierane opłaty od użytkowników albo inne przychody (bilety, taryfy, czynsze, sprzedaż energii, oszczędności)?* „Tak" prowadzi do projektu generującego dochód (Faza 5, wariant z luką lub stawką zryczałtowaną); „nie" — do ścieżki bez korekty dochodu.

### Faza 5. Ustal poziom dofinansowania (dochód i pomoc publiczna)

To węzeł, w którym schodzą się dwie osie: dochodowość i pomoc publiczna. Jeśli projekt generuje dochód i **nie** jest objęty pomocą publiczną, dofinansowanie ustala się zwykle metodą **luki w finansowaniu** albo — jeśli regulamin dopuszcza — przy użyciu **stawek zryczałtowanych dochodu** dla danego sektora (art. 67 rozp. 2021/1060). Jeśli natomiast wsparcie stanowi **pomoc publiczną**, logika luki finansowej zwykle **nie ma zastosowania** — intensywność wsparcia wynika z właściwego programu pomocowego, a nie z rachunku luki.

> **Pytanie kontrolne:** *Czy wsparcie stanowi pomoc publiczną?* „Tak" — pomijasz lukę finansową i stosujesz limity z odpowiedniego rozporządzenia pomocowego. „Nie" + projekt dochodowy — stosujesz lukę finansową lub stawki zryczałtowane. „Nie" + projekt bezdochodowy — dofinansowanie do wysokości kosztów kwalifikowalnych wg stopy z programu. *(Ocena wystąpienia pomocy publicznej to odrębna analiza prawna — w razie wątpliwości skonsultuj.)*

### Faza 6. Wykonaj analizę ekonomiczną (AKK właściwą) albo CEA

Analiza ekonomiczna patrzy szerzej niż finansowa: uwzględnia korzyści i koszty dla całego społeczeństwa (np. oszczędność czasu, redukcja emisji i wypadków, poprawa dostępu do usług), po wcześniejszym oczyszczeniu cen z transferów (podatki, dotacje). Wynik mówi, czy projekt jest opłacalny społecznie. Jeśli głównych korzyści **nie da się wiarygodnie wycenić w pieniądzu** (typowe w zdrowiu, edukacji, kulturze), zamiast pełnej AKK stosuje się **analizę efektywności kosztowej (CEA)** — koszt na jednostkę efektu. Zakres tej fazy zależy od progu/wymogu z naboru.

> **Pytanie kontrolne:** *Czy najważniejsze korzyści projektu da się rzetelnie przeliczyć na pieniądze?* „Tak" → pełna analiza ekonomiczna (ENPV/ERR/wskaźnik korzyści do kosztów). „Nie" → CEA. *(Czy analiza ekonomiczna jest w ogóle wymagana — [do weryfikacji w SWI naboru].)*

### Faza 7. Sprawdź trwałość finansową

Zweryfikuj, czy w każdym roku okresu odniesienia podmiot będzie miał dość środków na pokrycie wszystkich wydatków (saldo skumulowane nieujemne) — tak, by projekt nie wymagał później dodatkowego ratowania z budżetu. Tu duże znaczenie ma **typ wnioskodawcy**: inaczej liczy się trwałość dla gminy, inaczej dla spółki komunalnej, a inaczej dla zakładu budżetowego (kwestia konsolidacji z budżetem JST i źródeł pokrycia ewentualnych deficytów).

> **Pytanie kontrolne:** *Czy w każdym roku saldo skumulowane jest nieujemne, a jeśli gdzieś jest ujemne — czy jasno wskazałem, kto i z jakich środków je pokryje?*

### Faza 8. Przeprowadź analizę wrażliwości i ryzyka

Sprawdź, jak wynik (zwłaszcza wskaźniki ekonomiczne i trwałość) reaguje na zmianę kluczowych założeń — kosztów inwestycji, kosztów eksploatacji, popytu, przychodów. Zidentyfikuj zmienne krytyczne, opisz scenariusze oraz główne ryzyka i sposoby ich ograniczania.

> **Pytanie kontrolne:** *Które założenie, jeśli się nie sprawdzi, najmocniej zagraża opłacalności lub trwałości projektu — i co z tym robię?*

### Faza 9. Sformułuj wnioski i zapewnij spójność z wnioskiem

Zbierz wyniki w rekomendację i upewnij się, że liczby w AKK są **zgodne** z budżetem, harmonogramem, wskaźnikami i opisem we wniosku o dofinansowanie oraz w studium wykonalności. Rozbieżności między AKK a wnioskiem to jedna z najczęstszych przyczyn wezwań do uzupełnień.

> **Pytanie kontrolne:** *Czy kwoty i założenia w AKK pokrywają się co do grosza z wnioskiem i pozostałą dokumentacją?*

---

# B. Osie decyzyjne (punkty krytyczne — drzewo decyzyjne)

Kanoniczny zestaw ośmiu osi. Dla każdej: **cecha → pytanie rozstrzygające → możliwe warianty → co konkretnie zmienia się w zawartości modelu** (bez liczb).

### Oś 1. Program i instytucja zarządzająca

- **Pytanie rozstrzygające:** *Z którego programu i od której instytucji pochodzi dofinansowanie?*
- **Warianty:** program krajowy (np. FEnIKS, FERS, FERC, Polska Wschodnia) / program regionalny (FE dla danego województwa, zarządzany przez Urząd Marszałkowski) / inny.
- **Co zmienia:** obowiązujący wzór i zakres analizy, wymagany format studium wykonalności, narzucone parametry (horyzont, stopy, metoda dochodu), a często gotowy arkusz kalkulacyjny. Te same Wytyczne MFiPR są wspólne, ale **instrukcja naboru (SWI)** każdej instytucji doprecyzowuje je inaczej. Zawsze pracuj na dokumentach konkretnego naboru.

### Oś 2. Sektor / przedmiot projektu

- **Pytanie rozstrzygające:** *Czego dotyczy inwestycja?*
- **Warianty:** transport drogowy, kolejowy, transport publiczny, woda–kanalizacja, odpady, energetyka/OZE/efektywność energetyczna, kultura, zdrowie, edukacja, rewitalizacja, cyfryzacja/TIK.
- **Co zmienia:** długość okresu odniesienia (horyzontu), katalog i sposób wyceny korzyści ekonomicznych (np. oszczędność czasu i redukcja wypadków w transporcie, efekty środowiskowe w wod-kan i odpadach, efekty zdrowotne w ochronie zdrowia), obowiązującą metodykę sektorową (np. Niebieskie Księgi CUPT dla dróg i kolei) oraz to, czy realny jest pomiar korzyści w pieniądzu, czy raczej CEA. Sektor decyduje też, czy projekt typowo generuje dochód (wod-kan, odpady, energia — zwykle tak; drogi publiczne bez opłat — zwykle nie).

### Oś 3. Typ wnioskodawcy

- **Pytanie rozstrzygające:** *Kto składa wniosek i jak jest powiązany z budżetem publicznym?*
- **Warianty:** JST (gmina, powiat, województwo) / związek lub porozumienie JST / spółka komunalna / zakład lub jednostka budżetowa.
- **Co zmienia:** sposób analizy trwałości finansowej (czy patrzymy na samodzielny podmiot, czy konsolidujemy z budżetem JST), zakres podmiotowy przepływów, kwestię odzyskiwania VAT (różna sytuacja gminy i spółki — patrz oś 5), a w związkach/porozumieniach — podział nakładów, przychodów i odpowiedzialności między uczestników. Dla spółki komunalnej dochodzi też ryzyko pomocy publicznej (patrz oś 7).
- **Przykład.** Ten sam projekt — np. infrastruktura transportu publicznego — inaczej wygląda w analizie, gdy beneficjentem jest **miasto (JST)**, a inaczej, gdy jest nim **spółka komunikacji miejskiej** należąca do tego miasta. Proces jest identyczny (te same kroki 0–9), ale w kroku 7 (trwałość) dla miasta przepływy konsoliduje się w budżecie JST, a dla spółki bada się jej **samodzielny bilans** i zdolność do spięcia się bez ratowania z budżetu; równolegle dla spółki znacząco rośnie prawdopodobieństwo, że wsparcie stanowi **pomoc publiczną** (oś 7), co z kolei wyłącza metodę luki finansowej (oś 6). To jedna z najczęściej mylonych różnic — i klasyczny dowód, że „inny wniosek" oznacza tu inne *ustawienie* tych samych kroków, a nie inny proces.

### Oś 4. Wartość i skala projektu (próg pełnej AKK)

- **Pytanie rozstrzygające:** *Czy projekt przekracza próg uruchamiający pełną AKK określony w naborze?*
- **Warianty:** poniżej progu (analiza uproszczona) / powyżej progu (pełna AKK).
- **Co zmienia:** wymaganą głębokość analizy — od uproszczonej analizy finansowej po pełną AKK z analizą ekonomiczną, wrażliwości i ryzyka. **Uwaga:** dawny unijny próg „dużego projektu" (50/75 mln EUR) **nie obowiązuje** w 2021–2027; progi i uproszczenia ustala program. **[Konkretne progi — do weryfikacji w SWI danego naboru.]**

### Oś 5. Odzyskiwalność VAT

- **Pytanie rozstrzygające:** *Czy podmiot ma prawo odzyskać VAT?*
- **Warianty:** VAT odzyskiwalny (kwoty netto, VAT niekwalifikowalny) / VAT nieodzyskiwalny (VAT może być kosztem kwalifikowalnym i wchodzi do nakładów).
- **Co zmienia:** przesuwa zarówno koszt kwalifikowalny, jak i kwotę dotacji. Rozstrzygnięcie zależy od typu wnioskodawcy (oś 3) i charakteru działalności. Częsty błąd: przyjęcie kwot brutto przez podmiot, który VAT odzyskuje (lub odwrotnie).

### Oś 6. Czy projekt generuje dochód (przychody netto)

- **Pytanie rozstrzygające:** *Czy z efektów projektu będą pobierane opłaty od użytkowników lub inne przychody?*
- **Warianty:** projekt dochodowy → metoda **luki w finansowaniu** albo **stawki zryczałtowane** dochodu (art. 67 rozp. 2021/1060) / projekt bezdochodowy → brak korekty o dochód.
- **Co zmienia:** sam fakt liczenia (lub nie) luki finansowej, a w konsekwencji **maksymalną kwotę dofinansowania**. W projekcie dochodowym trzeba prognozować przychody i koszty operacyjne na cały horyzont; pominięcie istniejących przychodów zawyża dotację i grozi korektą.

### Oś 7. Wystąpienie pomocy publicznej

- **Pytanie rozstrzygające:** *Czy wsparcie stanowi pomoc publiczną?*
- **Warianty:** wsparcie bez pomocy publicznej / wsparcie objęte pomocą publiczną (np. wyłączenia GBER, pomoc de minimis, rekompensata UOIG).
- **Co zmienia:** **wyłącza logikę luki finansowej** — przy pomocy publicznej intensywność wsparcia wynika z właściwego programu pomocowego, nie z rachunku luki. Zmienia też maksymalny poziom dofinansowania i katalog kosztów kwalifikowalnych. To jedno z najtrudniejszych rozstrzygnięć — wymaga oceny prawnej. **[Zasady i wyłączenia — do weryfikacji wg aktualnych przepisów o pomocy publicznej.]**

### Oś 8. Pełna AKK vs analiza efektywności kosztowej (CEA)

- **Pytanie rozstrzygające:** *Czy główne korzyści projektu da się wiarygodnie wyrazić w pieniądzu?*
- **Warianty:** korzyści wyceniane pieniężnie → pełna analiza ekonomiczna (AKK) / korzyści trudne do wyceny → CEA (koszt na jednostkę efektu).
- **Co zmienia:** zestaw wskaźników i logikę dowodzenia zasadności. AKK kończy się wskaźnikami społecznej opłacalności (ENPV/ERR/B/C); CEA — porównaniem kosztu uzyskania jednostki efektu między wariantami. Typowo CEA bywa właściwa w zdrowiu, edukacji i części projektów kultury, gdzie wycena korzyści w pieniądzu jest wątpliwa.

> **Uwaga o formule realizacji (PPP/hybryda).** Jeśli projekt realizowany jest w partnerstwie publiczno-prywatnym (projekt hybrydowy, PPP/EPC) zamiast w formule klasycznej, zmienia się struktura przepływów i podział ryzyk między partnera publicznego i prywatnego, sposób ujęcia wynagrodzenia partnera prywatnego oraz analiza „value for money"; Wytyczne MFiPR mają osobny załącznik dla projektów hybrydowych. Traktuj to jako modyfikator nakładaną na powyższe osie, a nie odrębny proces.

---

# C. Podsumowanie — najczęstsze i najkosztowniejsze rozgałęzienia

Cztery węzły najczęściej decydują o powodzeniu i najwięcej kosztują w razie błędu:

1. **Czy projekt generuje dochód (oś 6).** Błędne uznanie projektu za bezdochodowy — albo pominięcie istniejących opłat — zawyża dofinansowanie i jest klasyczną przyczyną korekt finansowych. To rozgałęzienie pojawia się niemal w każdym projekcie infrastrukturalnym.

2. **Pomoc publiczna (oś 7).** Najtrudniejsze i najbardziej brzemienne w skutki rozstrzygnięcie. Przeoczenie pomocy publicznej oznacza, że cała logika luki finansowej i poziomu dofinansowania jest błędna — z ryzykiem zwrotu środków. Wymaga oceny prawnej, nie tylko finansowej.

3. **Odzyskiwanie VAT (oś 5 / Faza 3).** Pozornie techniczny szczegół, który przesuwa zarówno koszt kwalifikowalny, jak i kwotę dotacji. Częsty błąd: przyjęcie kwot brutto przez podmiot, który VAT odzyskuje (lub odwrotnie).

4. **Wybór AKK vs CEA i poprawny stan bazowy (oś 8, Faza 1–2).** Próba „na siłę" wyceniania korzyści, których wiarygodnie wycenić się nie da, albo źle zdefiniowany wariant „bez projektu" — podważają cały wynik analizy i bywają kwestionowane przez oceniających.

Praktyczna kolejność rozstrzygania na starcie: najpierw **wymóg i format z naboru** (Faza 0), potem **VAT**, **dochodowość** i **pomoc publiczna** — bo te trzy razem wyznaczają, którą ścieżką w ogóle pójdzie model finansowy.

---

> **Uwaga końcowa.** Wszystkie progi kwotowe, stopy dyskontowe, horyzonty sektorowe i metody ustalania dochodu należy każdorazowo potwierdzić w **aktualnych Wytycznych MFiPR/2021-2027/15(1)** oraz w **instrukcji i regulaminie konkretnego naboru** — to one są wiążące i mogą się różnić między programami. Elementy oznaczone **[do weryfikacji]** wymagają takiego potwierdzenia przed użyciem w realnym wniosku.
