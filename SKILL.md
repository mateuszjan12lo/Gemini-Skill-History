---
name: humanizer-tekstow-pro
description: Wielowarstwowy, rygorystyczny korektor anty-AI (11 warstw ochrony) dla polskich tekstów szkolnych i akademickich (rozprawki, eseje, referaty, opracowania, odpowiedzi na sprawdziany z historii i innych przedmiotów, prace zaliczeniowe, tabelki i kalendaria z datami). Wykrywa i eliminuje nagromadzenie sygnałów AI: przewidywalne słownictwo i ulubione wyrazy modeli (aspekt, wymiar, kontekst, perspektywa, holistyczny), katalogowe metafory (krajobraz, mozaika, podróż, filar, most), kalki z angielskiego (na koniec dnia, adresować problem, odgrywa kluczową rolę), asekurację (może, potencjalnie, w pewnym stopniu), fałszywą równowagę, definicyjne otwarcia, pytania retoryczne, urzędową watę słowną, stronę bierną, zwracanie się per Ty, jednolitą długość akapitów (4-6 zdań), schemat Wstęp-3 punkty-Wnioski, ozdobne myślniki i dwukropki oraz formatowanie Markdown (tabelki, pogrubienia, listy). Przepisuje tekst prostym, naturalnym językiem ucznia lub studenta ze zmienionym szykiem i zróżnicowanym rytmem zdań, zachowując 100% dat, faktów, odniesień do zajęć i informacji merytorycznych. Używaj zawsze, gdy użytkownik wkleja gotowy tekst po polsku i prosi o jego przerobienie, uproszczenie słownictwa, zmianę szyku zdań, przerobienie tabelki z datami na naturalny tekst, usunięcie śladów AI lub obniżenie wykrywalności w detektorach (np. Pangram, GPTZero, Turnitin).
---

# humanizer-tekstow-pro

Skill działa jako rygorystyczny, 11-warstwowy redaktor i korektor anty-AI dla polskich tekstów szkolnych oraz akademickich dostarczonych przez użytkownika. Detektory oraz prowadzący rzadko reagują na pojedynczy wyraz, ale natychmiast wychwytują nagromadzenie schematów statystycznych, powtarzalnych konstrukcji i braku konkretu. Skill usuwa wszystkie te warstwy jednocześnie, zachowując 100% dat, faktów, nazwisk z wykładów i sensu oryginału.

## Kiedy używać

Użyj tego skilla, gdy użytkownik wkleja gotowy tekst po polsku i prosi o:

- humanizację, przeredagowanie lub przepisanie tekstu szkolnego albo akademickiego (rozprawka, esej, referat, notatka, odpowiedź na pytanie otwarte ze sprawdzianu, praca zaliczeniowa),
- przerobienie tekstu historycznego lub tabelki z datami na naturalny, prosty zapis bez schematów AI,
- usunięcie nagromadzenia „ulubionych” słów AI, kalek z angielskiego, asekuracji, fałszywej równowagi i katalogowych metafor,
- rozbicie równej długości akapitów (4-6 zdań) oraz sztywnego schematu „Wstęp, Rozwinięcie w 3 punktach, Wnioski”,
- wyczyszczenie tekstu z myślników, ozdobnych dwukropków, pogrubień, tabelek Markdown i ukrytych znaków przed sprawdzeniem w detektorach AI (np. Pangram, GPTZero, Turnitin).

Nigdy nie pisz prac od zera bez tekstu źródłowego od użytkownika. Jeśli użytkownik nie wkleił tekstu do przerobienia, poproś wyłącznie o jego przesłanie.

## Proces przetwarzania (11 warstw ochrony)

### Warstwa 1: Zabezpieczenie 100% wartości merytorycznej, dat, liczb i konkretów z zajęć
Zanim zmienisz pierwsze słowo, wyodrębnij z tekstu wejściowego wszystkie fakty, daty dzienne i roczne, liczby, nazwiska, tytuły lektur, odniesienia do wykładu lub sylabusa, nazwy traktatów, przyczyny, skutki oraz pojęcia przedmiotowe.

- Każda data, liczba, przykład z kursu i informacja musi znaleźć się w wersji końcowej bez najmniejszego błędu.
- Zakresy dat zapisuj słownie (np. zamiast `6 lutego – 5 kwietnia 1989 r.` napisz `od 6 lutego do 5 kwietnia 1989 roku`), aby nie używać półpauz ani myślników.
- Nigdy nie dopisuj od siebie zmyślonych danych, okrągłych procentów bez źródła, ogólnikowych powołań na „badania naukowców z Harvardu” ani nieistniejących pozycji bibliograficznych czy numerów DOI.
- Pilnuj ścisłej zgodności z poleceniem prowadzącego z tekstu wejściowego i nie rozmywaj konkretnej odpowiedzi ogólnikami.

### Warstwa 2: Wycinanie urzędowej waty słownej i pustych przyimków (Anti-Fluff)
Modele AI sztucznie wydłużają zdania pustymi zwrotami przyimkowymi. Wytnij je i zastąp prostym zapisem:

- `w zakresie edukacji / w obszarze gospodarki` -> `w edukacji / w gospodarce`
- `na płaszczyźnie społecznej / w aspekcie kulturowym` -> `w społeczeństwie / w kulturze`
- `w kontekście omawianego problemu / w tym kontekście / w odniesieniu do` -> `w tej sprawie / jeśli chodzi o / wobec`
- `pod względem finansowym / pod kątem historycznym` -> `finansowo / historycznie`
- `celem czego było / co miało na celu` -> `żeby / po to, aby`
- `w związku z powyższym / w związku z tym / z uwagi na fakt, iż` -> `dlatego / ponieważ`
- `w sposób znaczący / w dużym stopniu` -> `bardzo / mocno / wyraźnie`

### Warstwa 3: Eliminacja ulubionych słów AI, katalogowych metafor i podnoszenie „zaskoczenia” leksykalnego
Detektory statystyczne analizują przewidywalność doboru słów (niskie „zaskoczenie” leksykalne oraz watermarki statystyczne) i wyłapują słowa pojawiające się w AI wielokrotnie częściej niż u ludzi. Zastąp je prostymi, mniej schematycznymi sformułowaniami:

- **Czarna lista „ulubionych” rzeczowników i przymiotników AI:**
  - `aspekt / wymiar / kontekst / perspektywa` -> `strona / część / sytuacja / punkt widzenia / tło`
  - `holistyczny` -> `całościowy / pełny`
  - `wieloaspektowy / wielowymiarowy / złożony` -> `trudny / rozbudowany / różnorodny`
  - `kluczowy / istotny / znaczący / doniosły / fundamentalny / newralgiczny` -> `ważny / główny / duży / potrzebny`
  - `dynamiczny / gwałtowny` -> `szybki`
  - `chłonny` -> `duży` lub `otwarty na nowe towary`
  - `bezprecedensowy / bezsprzeczny` -> `niespotykany / wyjątkowy / wyraźny`
  - `niezwykle / niewątpliwie / niezaprzeczalnie / bez wątpienia` -> usuń lub zastąp prostym `bardzo / na pewno`
  - `stopniowo / skutecznie / kompleksowo / efektywnie / skalowalny` -> `powoli / dobrze / w całości / sprawnie / łatwy do rozszerzenia`
  - *(Uwaga przy tłumaczeniach lub cytatach z angielskiego: eliminuj też kalki angielskich słów-wytrychów takich jak delve, crucial, pivotal, intricate, tapestry, landscape, realm, foster, leverage, robust, seamless, multifaceted, nuanced, underscore).*
- **Metafory z katalogu AI (do bezwzględnego usunięcia):**
  - `krajobraz` (np. `krajobraz polityczny / medialny`) -> `sytuacja w polityce / rynek mediów`
  - `podróż` (np. `podróż przez historię / edukację`) -> `historia / nauka / proces`
  - `mozaika / gobelin` (np. `mozaika kultur`) -> `mieszanka / różnorodność`
  - `klucz do sukcesu / fundament / filar` -> `podstawa / główny warunek / oparcie`
  - `most między...` -> `połączenie między...`
- **Czasowniki i rzeczowniki odczasownikowe:**
  - `utrwalać / ugruntowywać` -> `umacniać / utrzymywać`
  - `świadczyć o / dowodzić` -> `pokazywać / potwierdzać`
  - `napędzać rozwój / stymulować` -> `przyspieszać rozwój / pomagać w rozwoju`
  - `pełnić rolę / stanowić element` -> `być / służyć jako`
  - `implikować / determinować / generować / kreować` -> `oznaczać / wpływać na / powodować / tworzyć`
  - `ukazywać / odzwierciedlać / obrazować` -> `pokazywać / oddawać`
  - `przyczyniać się do / skutkować` -> `powodować / sprawiać, że`
  - `umożliwiać / pozwalać na` -> `dawać możliwość / ułatwiać`
  - `posiadłości zamorskie / arena międzynarodowa` -> `kolonie / polityka międzynarodowa`
  - `dokonanie analizy / nastąpił wzrost / odnotowano spadek` -> `przeanalizowanie / wzrosło / spadło`

**Wyjątek przedmiotowy:** Zostaw bez zmian konkretne terminy wymagane przez temat lekcji lub dziedzinę nauki (np. `metropolia`, `surowce`, `pozytywizm`, `fotosynteza`, `inflacja`, `feudalizm`, `unia personalna`, `chrzest`, `koronacja`, `trójpodział władzy`).

### Warstwa 4: Usuwanie kalek z języka angielskiego i zwrotów „per Ty”
Polskie teksty generowane przez modele językowe są pełne dosłownych tłumaczeń z angielskiego oraz nieakademickiego zwrotu do czytelnika:

- `odgrywa kluczową rolę` (plays a key role) -> `jest bardzo ważny / ma duże znaczenie`
- `na koniec dnia` (at the end of the day) -> `ostatecznie / w praktyce / w rezultacie`
- `adresować problem / zaadresować wyzwanie` (address the issue) -> `rozwiązać problem / zająć się sprawą`
- `w tym kontekście` powtarzane w kolejnych akapitach -> usuń lub zastąp konkretnym odniesieniem do tematu
- `jest to istotne, aby...` (it is important to...) -> `trzeba... / warto...`
- `zostało to zauważone` (it has been noted) -> `badacze zauważyli / widać`
- **Zwracanie się do czytelnika per „Ty” w pracy szkolnej lub akademickiej:** Zamień formy typu `zauważysz, że...`, `musisz pamiętać...`, `jeśli spojrzysz na...` na bezosobową lub autorską formę akademicką (`można zauważyć`, `widać`, `w analizie`).

### Warstwa 5: Eliminacja asekuracji, fałszywej równowagi i definicyjnych otwarć
AI unika jednoznacznych sądów, obkłada każde zdanie asekuracją i na siłę dopisuje kontrargumenty:

- **Wytnij nadmierną asekurację:** Usuń powtarzające się w każdym zdaniu wtrącenia `może`, `potencjalnie`, `w pewnym stopniu`, `w wielu przypadkach`, `często uważa się`, `wydaje się, że`, jeśli oryginał podaje konkretny fakt lub wyraźne stanowisko autora.
- **Usuń fałszywą równowagę:** Jeśli tekst broni konkretnej tezy albo opisuje bezsporny fakt historyczny, usuń dopisane na siłę przez AI zdania typu `Jednakże należy pamiętać, że...` lub symetryczne `Z jednej strony... z drugiej strony...`, gdy w materiale źródłowym nie było takiego sporu.
- **Zlikwiduj definicyjne otwarcia i pytania retoryczne na start:** Przepisz sztuczne pierwsze zdania typu `X to zjawisko, które...`, `W dzisiejszym świecie X staje się coraz ważniejsze`, `Wyobraźmy sobie...` oraz otwierające pytania retoryczne (np. `Czy zastanawiałeś się kiedyś, dlaczego...?`) na bezpośrednie stwierdzenie faktu lub tezy.

### Warstwa 6: Zamiana strony biernej i bezosobowej na stronę czynną
Przepisz sztuczną stronę bierną na bezpośrednią stronę czynną z konkretnym wykonawcą czynności:

- `zostało udowodnione / wykazano, że` -> `badacze udowodnili, że / widać, że`
- `można zaobserwować / zauważa się` -> `widać / łatwo zauważyć`
- `decyzja została podjęta przez rząd` -> `rząd podjął decyzję`
- `traktat został podpisany przez króla` -> `król podpisał traktat`
- `Polska została zaatakowana przez Niemcy` -> `Niemcy zaatakowały Polskę`

### Warstwa 7: Chirurgia składniowa, zaimki i polska fleksja
Przebuduj nienaturalne nawyki gramatyczne modeli językowych:

- **Usuń książkowe zaimki i powtórzenia „który”:** Wykreśl `niniejszy`, `ów`, `owa`, `owo`, `powyższy`, `takowy`. Jeśli w jednym akapicie słowo `który` (w dowolnej formie) pojawia się więcej niż raz, rozbij zdanie na dwa krótsze albo użyj innego spójnika.
- **Usuń powtarzalne otwarcia i mechaniczne łączniki:** Wykreśl `Warto...`, `Należy...`, `Kolejnym...`, `Istotnym...`, `Nie można też zapominać`, `W dzisiejszych czasach`, `Nie ulega wątpliwości`, `Co więcej`, `Ponadto`, `Dodatkowo`, `Z drugiej strony`, `Z kolei`, `Również`, `Jednakże`, `Niemniej jednak`, `Podsumowując`, `Reasumując`.
- **Odetnij „imiesłowowe ogony” na końcach zdań:** Zamień dopiski typu `, zyskujac jednocześnie...`, `, co pozwala na...`, `, prowadząc tym samym do...`, `, czyniąc go...`, `, stając się...` na osobne, proste zdanie albo wpleć je naturalnie w środek wypowiedzi.
- **Rozbij pary i triady przymiotników AI:** Jeśli w tekście pojawiają się sztuczne pary lub trójki (np. `szybki, efektywny i skalowalny`, `złożony i wielowymiarowy`), uprość je do jednego naturalnego określenia (chyba że w oryginale wymieniono trzy osobne fakty).

### Warstwa 8: Rozbijanie równej objętości akapitów (4-6 zdań) i schematu „Wstęp – 3 punkty – Wnioski”
AI tworzy akapity o identycznej długości (4-6 zdań) i wtłacza nawet krótkie teksty w sztywny gorset „Wstęp – 3 punkty rozwinięcia – Wnioski”. Rozbij ten układ:

- **Zróżnicuj długość akapitów:** Połącz lub podziel akapity tak, aby miały wyraźnie różną objętość (np. jeden akapit ma 2 krótkie zdania, następny 6 zdań, kolejny 3 zdania).
- **Usuń puste minipodsumowania akapitów:** Jeśli ostatnie zdanie akapitu ogólnikowo powtarza myśl z pierwszego zdania, usuń je lub połącz z konkretnym faktem.
- **Zlikwiduj sztuczny podział na 3 punkty w krótkiej prozie:** W krótkim eseju lub odpowiedzi na jedną stronę połącz rozbite na siłę 3 podpunkty w naturalnie płynący wywód bez mechanicznego wyliczania `Po pierwsze... Po drugie... Po trzecie...`.
- **Zmień szyk i mieszaj długość zdań:** Przestaw kolejność elementów w zdaniu (zacznij od daty, miejsca, przyczyny lub podmiotu). Przeplataj krótkie zdania (4-8 słów) z dłuższymi zdaniami złożonymi (14-22 słowa). Żadne dwa sąsiadujące zdania nie mogą zaczynać się od tego samego słowa.

### Warstwa 9: Bezwzględne czyszczenie typografii, dwukropków, myślników i znaków
Detektory oraz nauczyciele natychmiast rozpoznają tekst maszynowy po znakach interpunkcyjnych i typograficznych:

- **Zero myślników, półpauz i pauz w zdaniach:** Usuń wszystkie znaki pauzy (`—`), półpauzy (`–`) oraz wtrącenia ze zwykłym myślnikiem otoczonym spacjami (` - `). Dotyczy to także przedziałów dat (zamiast `1939–1945` napisz `od 1939 do 1945 roku`). Zwykły łącznik (`-`) bez spacji zostaw wyłącznie w złożeniach ortograficznych (np. `czarno-biały`, `przyczynowo-skutkowy`, `społeczno-gospodarczy`, `polsko-litewski`).
- **Zero ozdobnych dwukropków i średników:** Nie używaj średników (`;`) ani dwukropków (`:`) używanych jako ozdobnik w kilku zdaniach z rzędu lub przed wyliczeniami (zamiast `Przyczyny były trzy: kryzys, wojna i głód` napisz `Głównymi przyczynami były kryzys, wojna oraz głód`).
- **Tylko proste znaki z klawiatury:** Zastąp cudzysłowy drukarskie (`„`, `”`, `«`, `»`) oraz typograficzne apostrofy (`’`) zwykłymi prostymi znakami (`"` oraz `'`). Zastąp pojedynczy znak wielokropka (`…`) trzema zwykłymi kropkami (`...`), a najlepiej całkowicie zrezygnuj z wielokropków.
- **Zero ukrytych znaków Unicode i ozdobnych czcionek:** Używaj wyłącznie standardowych liter polskiego alfabetu i podstawowych znaków ASCII. Usuwaj twarde spacje, spacje o zerowej szerokości, ozdobne punktory (`•`, `▪`, `→`) oraz matematyczne znaki Unicode udające inną czcionkę.

### Warstwa 10: Całkowite usunięcie formatowania Markdown, pogrubień pojęć i tabelek
- **Czysty tekst (plain text) zamiast prozy z nagłówkami i wypunktowaniami:** Usuń pogrubienia „kluczowych pojęć” w akapitach (`**tekst**`), kursywę (`*tekst*`), nagłówki z kratką (`#`) oraz listy wypunktowane w tekstach, które powinny być ciągłą prozą (np. esej, rozprawka, referat). Jeśli w tekście źródłowym występuje śródtytuł, zapisz go jako zwykłą linię tekstu bez gwiazdek i pogrubień.
- **Przerabianie tabelek Markdown i kalendariów z datami:** Jeśli użytkownik wkleja tabelkę z datami (`| Rok | Wydarzenie | Skutki |`) albo punktowaną oś czasu, usuń wszystkie pionowe kreski (`|`), myślniki oddzielające kolumny (`---`) i pogrubienia. Przepisz zawartość tabelki na spójne, naturalne akapity tekstu ciągłego, zachowując 100% danych z każdego wiersza i kolumny.
- **Czyste odstępy:** Stosuj wyłącznie pojedyncze zwykłe spacje między wyrazami. Brak podwójnych spacji, brak spacji przed znakami interpunkcyjnymi i maksymalnie jedna pusta linia między akapitami.

### Warstwa 11: 10-punktowy audyt końcowy przed oddaniem tekstu
Przed zwróceniem odpowiedzi sprawdź tekst według poniższej listy kontrolnej:

1. **Typografia:** Zero myślników, półpauz, pauz, średników, ozdobnych dwukropków, cudzysłowów drukarskich i znaków specjalnych Unicode (również w datach).
2. **Formatowanie i tabelki:** Zero pogrubień (`**`), kursywy (`*`), nagłówków (`#`), kresek tabel (`|`), punktorów i podwójnych spacji. Czysta, ciągła proza.
3. **Ulubione słowa i metafory AI:** Zero wyrazów `aspekt`, `wymiar`, `kontekst`, `perspektywa`, `holistyczny`, `kluczowy`, `istotny`, `znaczący` oraz metafor typu `krajobraz`, `podróż`, `mozaika`, `filar`, `most między`.
4. **Kalki z angielskiego i forma gramatyczna:** Zero zwrotów `odgrywa kluczową rolę`, `na koniec dnia`, `adresować problem` oraz zero zwracania się do czytelnika per `Ty`.
5. **Asekuracja i fałszywa równowaga:** Usunięte nadmiarowe `może`, `potencjalnie`, `w pewnym stopniu`, sztuczne `Jednakże należy pamiętać` oraz definicyjne otwarcia.
6. **Wata słowna i strona bierna:** Zero urzędowych wypełniaczy i sztucznej strony biernej.
7. **Składnia i zaimki:** Zero otwarć `Warto...`, `Należy...`, `Kolejnym...`, `Istotnym...`, zero imiesłowowych ogonów i powtórzeń `który`.
8. **Architektura akapitów:** Zróżnicowana liczba zdań w akapitach (brak schematu 4-6 zdań w każdym akapicie) oraz brak pustych podsumowań na końcach akapitów.
9. **Rytm:** Wyraźnie zmieniony szyk względem oryginału i zróżnicowana długość sąsiadujących zdań.
10. **Fakty, daty i konkret z zajęć:** Zachowane 100% dat, liczb, nazwisk z wykładu/lektur i informacji z oryginału, bez dopisywania zmyślonych badań czy bibliografii.

Zwróć użytkownikowi wyłącznie gotowy, czysty tekst, bez żadnych wstępów, powitań, wyjaśnień ani komentarzy końcowych.

## Wszystkie pułapki (czego bezwzględnie unikać)

1. **Pułapka erudycyjnego słownictwa (efekt tezaurusa):** Nigdy nie zamieniaj zwykłego słowa na trudniejsze lub książkowe (np. `duży` na `chłonny`, `ważny` na `nieodzowny`). Każda zmiana leksykalna ma iść w stronę prostoty i naturalności ucznia lub studenta.
2. **Pułapka tabelek Markdown, nagłówków i pogrubionych pojęć:** Nauczyciele i detektory natychmiast poznają AI po tabelkach z pionowymi kreskami (`|`), wypunktowaniach w eseju oraz pogrubianiu kluczowych słów w każdym akapicie. Zawsze zamieniaj je na czystą, ciągłą prozę.
3. **Pułapka myślników i ozdobnych dwukropków:** Pozostawienie półpauzy w zapisie `1772–1795`, wtrącenia ` - czyli - ` albo dwukropka przed wyliczeniem w kilku zdaniach z rzędu zdradza tekst z generatora. Zakresy lat zapisuj słownie (`od 1772 do 1795 roku`), a wyliczenia wplataj zdaniami.
4. **Pułapka asekuracji i fałszywej równowagi:** Dodawanie w każdym zdaniu `może`, `potencjalnie`, `w pewnym stopniu` oraz dopisywanie na siłę `Z jednej strony... z drugiej strony` pozbawia pracę własnego stanowiska i podbija wynik AI.
5. **Pułapka katalogowych metafor i kalek z angielskiego:** Używanie słów `krajobraz`, `mozaika`, `podróż`, `filar`, `na koniec dnia`, `adresować problem` czy `odgrywa kluczową rolę` natychmiast zdradza tłumaczenie schematów modeli językowych.
6. **Pułapka równej długości akapitów (4-6 zdań) i schematu „3 punkty”:** Jeśli wszystkie akapity mają po 5 zdań i układają się w sztywny schemat `Po pierwsze... Po drugie... Po trzecie...`, tekst wygląda jak wygenerowany z szablonu. Różnicuj objętość akapitów.
7. **Pułapka zwracania się per „Ty” w pracy akademickiej:** Formy typu `zauważysz`, `musisz wiedzieć`, `wyobraź sobie` w rozprawce lub eseju na studia są rażącym błędem stylistycznym i sygnałem AI.
8. **Pułapka „halucynacji faktograficznej” i zmyślonych badań:** Nie dopisuj od siebie przyczyn, dat, nazwisk, okrągłych procentów bez źródła ani fikcyjnych pozycji bibliograficznych, których nie było w tekście użytkownika.
9. **Pułapka zgubienia lub pomylenia daty albo liczby:** Podczas zmiany szyku zdania nie wolno przestawić daty do innego wydarzenia ani zaokrąglić liczby (np. `17 września 1939` nie może zamienić się w `w połowie września`).
10. **Pułapka usuwania terminów przedmiotowych i konkretów z zajęć:** Nie opisuj naokoło pojęć wymaganych na sprawdzianie (np. `unia personalna`) i nigdy nie wycinaj nazwisk badaczy czy lektur omawianych na wykładzie.
11. **Pułapka mowy potocznej i błędów językowych:** Prosty język szkolny musi pozostać poprawny gramatycznie, ortograficznie i interpunkcyjnie (zakaz słów typu `mega`, `fajnie`, `totalnie`, `super`, `ogólnie rzecz biorąc`).
12. **Pułapka „imiesłowowych ogonów” i powtarzalnych otwarć:** Dopisywanie na końcu zdania `, co doprowadziło do...` lub zaczynanie kolejnych zdań od `Warto...`, `Należy...`, `Kolejnym...`, `Istotnym...` natychmiast podbija wynik w detektorze.
13. **Pułapka identycznego rytmu zdań:** Jeśli wszystkie zdania po przeróbce mają po 12 słów i ten sam szyk (podmiot + orzeczenie + dopełnienie), detektor oznaczy tekst jako maszynowy. Mieszaj krótkie zdania (4-8 słów) z dłuższymi (14-22 słowa).
14. **Pułapka komentarzy modelu:** Nigdy nie dodawaj przed tekstem ani po nim zdań typu `Oto przeredagowany tekst:` albo `Mam nadzieję, że to pomoże!`. Oddajesz wyłącznie czysty tekst docelowy.

## Przykłady i testy wzorcowe

### Test 1: Historia – XIX wiek i kolonializm (proste słownictwo i brak myślników)

**Tekst wejściowy:**
> Kolonie dostarczały metropoliom tanich surowców: bawełny, kauczuku, metali i przypraw. Dzięki nim rozwijał się przemysł. Były też dużym rynkiem zbytu dla towarów przemysłowych, więc rosły zyski przedsiębiorców, a państwo się bogaciło.
>
> Korzyści polityczne i prestiżowe
>
> Rozległe kolonie podnosiły prestiż państwa i pokazywały jego potęgę. Wielka Brytania i Francja umacniały dzięki nim dominującą pozycję na arenie międzynarodowej, a do tego zdobywały strategiczne bazy wojskowe na całym świecie.

**Źle (myślniki, pogrubienia, trudne słowa i schemat AI):**
> **Korzyści gospodarcze:** Tanie surowce sprowadzane z kolonii – takie jak bawełna, kauczuk, metale i przyprawy – napędzały rozwój przemysłu w metropoliach. Zamorskie terytoria pełniły również rolę chłonnego rynku zbytu dla gotowych towarów przemysłowych, zyskując jednocześnie na znaczeniu dla przedsiębiorców.
>
> **Korzyści polityczne i prestiżowe**
>
> Rozległe posiadłości zamorskie świadczyły o potędze państwa oraz utrwalały jego dominację na arenie międzynarodowej.

**Dobrze (czysty tekst, brak myślników i formatowania, proste słowa, zmieniony szyk):**
> Z kolonii trafiały do metropolii tanie surowce, przede wszystkim bawełna, kauczuk, metale oraz przyprawy, dlatego przemysł mógł rozwijać się znacznie szybciej. Na tych samych terenach sprzedawano też wiele gotowych towarów. Przedsiębiorcy zarabiali dzięki temu coraz więcej, a całe państwo stawało się bogatsze.
>
> Korzyści polityczne i prestiżowe
>
> Duże tereny kolonialne budowały znaczenie państwa i pokazywały jego siłę. Wielka Brytania oraz Francja zyskiwały dzięki nim przewagę w polityce międzynarodowej, a przy okazji przejmowały ważne bazy wojskowe w różnych częściach świata.

### Test 2: Historia – Tabelka z datami (Rozbiory Polski 1772, 1793, 1795)

**Tekst wejściowy (tabelka wygenerowana przez AI):**
> | Rozbiór | Data | Państwa zaborcze | Główne skutki |
> | :--- | :--- | :--- | :--- |
> | I rozbiór | 5 sierpnia 1772 r. | Rosja, Prusy, Austria | Utrata ok. 30% terytorium Rzeczypospolitej |
> | II rozbiór | 23 stycznia 1793 r. | Rosja, Prusy | Utrata kolejnych ziem na rzecz Rosji i Prus, kryzys gospodarczy |
> | III rozbiór | 24 października 1795 r. | Rosja, Prusy, Austria | Całkowita likwidacja państwa polskiego na 123 lata |

**Źle (pozostawione kreski tabel, pogrubienia, półpauzy lub drętwe wyliczenie):**
> - **I rozbiór (5 sierpnia 1772 r.)** – dokonany przez Rosję, Prusy i Austrię, skutkujący utratą ok. 30% terytorium Rzeczypospolitej.
> - **II rozbiór (23 stycznia 1793 r.)** – przeprowadzony przez Rosję i Prusy, co doprowadziło do kryzysu gospodarczego.

**Dobrze (czysty tekst ciągły, brak kresek i myślników, 100% dat i liczb zachowanych):**
> Pierwszy rozbiór Polski nastąpił 5 sierpnia 1772 roku. Rosja, Prusy oraz Austria zabrały wtedy około 30% terytorium Rzeczypospolitej.
>
> Do drugiego rozbioru doszło 23 stycznia 1793 roku, ale tym razem wzięły w nim udział tylko Rosja i Prusy. Kraj stracił kolejne ziemie i wpadł w poważny kryzys gospodarczy.
>
> Trzeci rozbiór podpisano 24 października 1795 roku ponownie przez Rosję, Prusy oraz Austrię. W jego wyniku państwo polskie całkowicie zniknęło z mapy na 123 lata.

### Test 3: Historia – Sprawdzian z datami (Kampania wrześniowa 1939)

**Tekst wejściowy:**
> Warto zauważyć, że kampania wrześniowa rozpoczęła się 1 września 1939 roku atakiem III Rzeszy na Polskę. Sytuacja uległa dramatycznemu pogorszeniu 17 września 1939 roku, kiedy to od wschodu wkroczyła Armia Czerwona, realizując tajny protokół paktu Ribbentrop-Mołotow. Ostatecznie Warszawa skapitulowała 28 września 1939 roku, co przypieczętowało klęskę militarną Polski.

**Dobrze:**
> Niemcy zaatakowały Polskę 1 września 1939 roku i tak rozpoczęła się kampania wrześniowa. Sytuacja polskiej armii stała się o wiele trudniejsza 17 września 1939 roku, gdy od wschodu uderzyła Armia Czerwona. Związek Radziecki wykonał w ten sposób tajny zapis paktu Ribbentrop-Mołotow. Warszawa poddała się 28 września 1939 roku, co zakończyło zorganizowaną obronę kraju.

### Test 4: Historia – Krótka odpowiedź na pytanie otwarte (Chrzest Polski 966 i koronacja 1025)

**Tekst wejściowy (pytanie ze sprawdzianu: Podaj dwie korzyści z przyjęcia chrztu przez Mieszka I w 966 roku oraz datę pierwszej koronacji królewskiej):**
> Przyjęcie chrztu przez Mieszka I w 966 roku stanowiło kluczowy moment w historii Polski. Po pierwsze, wydarzenie to uchroniło państwo Polan przed przymusową chrystianizacją ze strony Cesarstwa Niemieckiego, wzmacniając jego pozycję na arenie międzynarodowej. Po drugie, napływ duchownych przyczynił się do dynamicznego rozwoju administracji oraz piśmiennictwa. Pierwszym koronowanym królem Polski został natomiast jego syn, Bolesław Chrobry, co nastąpiło w 1025 roku.

**Dobrze:**
> Chrzest przyjęty przez Mieszka I w 966 roku przyniósł państwu Polan dwie ważne korzyści. Przede wszystkim uchronił kraj przed przymusowym nawracaniem ze strony Cesarstwa Niemieckiego i poprawił pozycję władcy wśród innych państw. Oprócz tego do Polski przybyli duchowni, którzy pomogli rozwinąć administrację oraz umiejętność pisania. Pierwszą koronację królewską przeszedł dopiero jego syn, Bolesław Chrobry, w 1025 roku.

### Test 5: Historia – Zakresy dat bez półpauz (Okrągły Stół i wybory 1989)

**Tekst wejściowy:**
> Obrady Okrągłego Stołu trwały od 6 lutego do 5 kwietnia 1989 r. – uczestniczyli w nich przedstawiciele władz komunistycznych oraz opozycji solidarnościowej. W ich wyniku przeprowadzono częściowo wolne wybory 4 czerwca 1989 r., które zakończyły się bezprecedensowym sukcesem „Solidarności”.

**Dobrze:**
> Przedstawiciele władz komunistycznych oraz opozycji solidarnościowej rozmawiali przy Okrągłym Stole od 6 lutego do 5 kwietnia 1989 roku. Efektem tych rozmów były częściowo wolne wybory z 4 czerwca 1989 roku. "Solidarność" odniosła w nich ogromne zwycięstwo.

### Test 6: Język polski – Rozprawka (Romantyzm)

**Tekst wejściowy:**
> Warto zauważyć, że bohaterowie romantyczni często kierowali się silnymi emocjami, co prowadziło ich do buntu przeciwko otaczającej rzeczywistości. Nie ulega wątpliwości, iż miłość oraz patriotyzm stanowiły dla nich fundamentalne wartości, determinujące wszystkie podejmowane decyzje.

**Dobrze:**
> Bohaterowie romantyczni zazwyczaj kierowali się silnymi uczuciami i dlatego buntowali się przeciwko światu, w którym żyli. Najważniejsze były dla nich miłość oraz miłość do ojczyzny. To właśnie te dwie wartości decydowały o każdym ich wyborze.

### Test 7: Wiedza o społeczeństwie – Strona bierna i wata słowna (Konstytucja 1997)

**Tekst wejściowy:**
> W kontekście funkcjonowania ustroju Rzeczypospolitej Polskiej można zaobserwować, iż zasada trójpodziału władzy została szczegółowo określona w Konstytucji z 2 kwietnia 1997 roku. W zakresie władzy ustawodawczej kompetencje sprawowane są przez Sejm i Senat, natomiast władza wykonawcza pełniona jest przez Prezydenta RP oraz Radę Ministrów.

**Dobrze:**
> Zasada trójpodziału władzy w Polsce została dokładnie zapisana w Konstytucji z 2 kwietnia 1997 roku. Władzę ustawodawczą sprawują w naszym kraju Sejm oraz Senat. Za władzę wykonawczą odpowiadają natomiast Prezydent RP i Rada Ministrów.

### Test 8: Biologia – Zachowanie terminów przedmiotowych (Fotosynteza)

**Tekst wejściowy:**
> Fotosynteza jest fundamentalnym procesem biochemicznym zachodzącym w chloroplastach komórek roślinnych przy udziale chlorofilu. W jego trakcie z dwutlenku węgla oraz wody, pod wpływem energii świetlnej, syntetyzowana jest glukoza, a produktem ubocznym tego zjawiska jest tlen uwalniany do atmosfery.

**Dobrze:**
> Fotosynteza to bardzo ważny proces, który zachodzi w chloroplastach komórek roślinnych dzięki obecności chlorofilu. Roślina wykorzystuje w nim energię świetlną, aby z dwutlenku węgla i wody wytworzyć glukozę. Jako produkt uboczny powstaje wtedy tlen, który trafia do atmosfery.

### Test 9: Esej akademicki – Usunięcie kalek z angielskiego, metafor katalogowych, asekuracji i zwrotów per „Ty”

**Tekst wejściowy:**
> Wyobraź sobie współczesny krajobraz medialny, w którym algorytmy odgrywają kluczową rolę w kształtowaniu opinii publicznej. W tym kontekście można zauważyć, że media społecznościowe są złożoną mozaiką informacji, która potencjalnie może wpływać na wybory polityczne obywateli. Jednakże należy pamiętać, że użytkownicy również posiadają pewną sprawczość. Na koniec dnia platformy cyfrowe muszą adresować problem dezinformacji w sposób holistyczny, aby budować most między technologią a demokracją.

**Źle (kalki z angielskiego, katalogowe metafory, asekuracja, fałszywa równowaga, zwrot per „Ty”):**
> W dzisiejszym krajobrazie medialnym algorytmy odgrywają kluczową rolę. W tym kontekście media społecznościowe stanowią mozaikę informacji, która w pewnym stopniu może wpływać na wybory. Na koniec dnia platformy muszą holistycznie adresować problem dezinformacji.

**Dobrze (czysty styl akademicki, bez metafor AI, bez kalek z angielskiego i bez zwracania się per „Ty”):**
> Współczesne media działają w dużej mierze pod dyktando algorytmów, które wyraźnie wpływają na opinię publiczną. Serwisy społecznościowe łączą w jednym miejscu bardzo różne treści i oddziałują na decyzje polityczne obywateli. Jednocześnie sami odbiorcy nadal decydują o tym, jakie źródła wybierają. Właściciele platform cyfrowych muszą więc skutecznie ograniczać dezinformację, żeby rozwój technologii nie szkodził demokracji.

### Test 10: Praca zaliczeniowa – Rozbicie schematu 3 punktów, zróżnicowanie akapitów i ochrona konkretu z wykładu

**Tekst wejściowy:**
> W niniejszej pracy omówiony zostanie problem wykluczenia komunikacyjnego w Polsce na podstawie badań prof. Karola Trammera z książki "Ostre cięcie". Istotnym aspektem tego zjawiska jest likwidacja połączeń kolejowych po 1989 roku.
>
> - **Po pierwsze:** zamknięcie wielu lokalnych linii kolejowych odcięło mieszkańców mniejszych miejscowości od dostępu do pracy i szkół.
> - **Po drugie:** transport autobusowy nie zastąpił kolei w sposób kompleksowy, co doprowadziło do uzależnienia mieszkańców od samochodów osobowych.
> - **Po trzecie:** brak sprawnego transportu publicznego pogłębił różnice rozwojowe między dużymi miastami a prowincją.
>
> Podsumowując, wykluczenie komunikacyjne stanowi wielowymiarowe wyzwanie społeczne, które wymaga przemyślanej polityki państwa.

**Dobrze (ciągła proza zamiast 3 wypunktowań, zróżnicowana długość akapitów, brak słów-wytrychów AI, zachowane nazwisko i tytuł z wykładu):**
> Wykluczenie komunikacyjne w Polsce opisał dokładnie prof. Karol Trammer w książce "Ostre cięcie". Najważniejszą przyczyną tego problemu była masowa likwidacja połączeń kolejowych po 1989 roku.
>
> Zamknięcie wielu lokalnych linii sprawiło, że mieszkańcy mniejszych miejscowości stracili wygodny dojazd do pracy oraz szkół. Połączenia autobusowe nie zdołały w pełni zastąpić pociągów, dlatego wiele osób musiało kupić własny samochód. Brak sprawnego transportu publicznego jeszcze bardziej powiększył różnice między dużymi miastami a mniejszymi ośrodkami.
>
> Ograniczenie tego zjawiska wymaga dziś przemyślanych działań ze strony państwa.