# Jak dodać plik SKILL.md do Google Gemini: przewodnik wieloplatformowy

Skill (po polsku **umiejętność**) to folder z plikiem `SKILL.md`. Plik zawiera instrukcje dla Gemini oraz opis tego, do czego umiejętność służy. Ten przewodnik pokazuje, jak ją dodać na każdej platformie:

- [Przeglądarka (Windows, macOS, Linux)](#przeglądarka-geminigooglecom)
- [Aplikacja Gemini na Maca](#aplikacja-gemini-na-maca)
- [Android](#android)
- [iPhone i iPad](#iphone-i-ipad)
- [Gemini CLI (terminal)](#gemini-cli-terminal)

## Spis treści

1. [Szybki wybór platformy](#1-szybki-wybór-platformy)
2. [Wymagania wspólne](#2-wymagania-wspólne)
3. [Przygotowanie folderu ze skillem](#3-przygotowanie-folderu-ze-skillem)
4. [Instrukcje dla platform](#4-instrukcje-dla-platform)
5. [Polecany przepływ: komputer → telefon](#5-polecany-przepływ-komputer--telefon)
6. [Rozwiązywanie problemów](#6-rozwiązywanie-problemów)
7. [Źródła](#7-źródła)

---

## 1. Szybki wybór platformy

| Chcę… | Przeglądarka | Aplikacja na Maca | Android | iPhone / iPad |
|---|:---:|:---:|:---:|:---:|
| **Wgrać** `SKILL.md`, folder lub `.zip` | tak | tak (nagranie) | **nie** | **nie** |
| Utworzyć ręcznie (wpisać instrukcje) | tak | tak (nagranie) | tak | tak |
| Utworzyć z pomocą Gemini na czacie | tak | tak | tak | tak |
| Utworzyć z szablonu (*Rekomendowane*) | tak | tak | tak | tak |
| Edytować opis i instrukcje | tak | tak | tak | tak |
| Edytować w rozmowie (*Edytuj za pomocą Gemini*) | tak | tak | tak | tak |
| Zastąpić umiejętność plikiem | tak | nie sprawdzono | nie | nie* |
| Dodawać, zastępować, usuwać pliki w skillu | tak | nie sprawdzono | nie | nie |
| Włączać i wyłączać | tak | tak | tak | tak |
| Pobrać jako `.zip` | tak | tak | tak | tak |
| Usunąć | tak | tak | tak | tak |
| Udostępnić innym | tak | nie sprawdzono | nie | nie |

Zakres kolumn:
- **Przeglądarka, Android, iPhone/iPad:** na podstawie oficjalnej pomocy Google.
- **Aplikacja na Maca:** wgrywanie i tworzenie ręczne widziałem na nagraniu ekranu. Pozostałe wiersze pomoc Google przypisuje przeglądarce, a dla aplikacji na Maca nic nie mówi, dlatego mają „nie sprawdzono” albo „tak” tam, gdzie pomoc ogólnie opisuje funkcję dla całego Gemini.
- *\* Pomoc Google dla iPhone'a opisuje opcję *Zastąp umiejętność*, a w tym samym artykule podaje, że przesyłanie plików w aplikacji mobilnej nie jest dostępne, więc działanie tej opcji jest niepewne.*

**Jeśli masz gotowy `SKILL.md`:** wgraj go w przeglądarce lub aplikacji na Maca. Na telefonie użyj obejścia z sekcji [Android](#android) lub [iPhone i iPad](#iphone-i-ipad).

## 2. Wymagania wspólne

- ukończone 18 lat,
- zalogowanie w aplikacji Gemini lub na gemini.google.com,
- włączona opcja **Zachowuj aktywność**. Przy wyłączonej umiejętności działają, ale bez dostępu do połączonych aplikacji, np. Kalendarza Google i Dysku Google,
- subskrypcja Google AI nie jest wymagana,
- według pomocy Google na iPhonie konta służbowe i szkolne nie są na razie obsługiwane.

### Słowniczek interfejsu

| English (nagranie) | Polski interfejs |
|---|---|
| Skills | Umiejętności |
| Customize | Dostosuj |
| More | Więcej |
| Create → Upload skill | Utwórz → Prześlij |
| Create manually | Utwórz ręcznie |
| Recommended | Rekomendowane |

## 3. Przygotowanie folderu ze skillem

Struktura:

```text
moj-skill/
├── SKILL.md        # wymagany
└── (opcjonalnie pliki pomocnicze: .md, .pdf, .csv, .py ...)
```

Minimalny `SKILL.md`:

```markdown
---
name: moj-skill
description: Krótko opisz, do czego służy umiejętność i kiedy Gemini ma jej użyć.
---

# Instrukcje

Tutaj napisz, jak Gemini ma wykonywać zadanie: kroki, styl odpowiedzi, ograniczenia.
```

Wymagania dla przesyłanych plików:

- w **katalogu głównym** folderu (lub archiwum `.zip`) musi być `SKILL.md`,
- nazwa w `SKILL.md` małymi literami, słowa oddzielone łącznikami (**kebab-case**), np. `moj-nauczyciel-niemieckiego`,
- łączny rozmiar do 100 MB,
- obsługiwane typy: dokumenty (.docx, .pdf, .md, .txt), arkusze (.csv, .xlsx), prezentacje (.pptx), obrazy (.jpg, .png, .webp), kod (.py, .js, .sh), konfiguracje (.json, .yaml, .xml),
- nieobsługiwane: stare formaty Office (.doc, .xls, .ppt), audio, wideo, archiwa w środku folderu oraz m.in. .ts, .tsx, .jsx, .php, .sql,
- przed wgraniem usuń pliki ukryte i binarne (`.DS_Store`, `.pyc`), bo powodują błąd,
- skrypty nie mogą wykonywać działań w sieci ani wysyłać żądań do zewnętrznych stron.

`description` jest tym, po czym Gemini rozpoznaje, kiedy umiejętność się przydaje. Wpisz w nim konkretne zadania i słowa, których będziesz używać w promptach.

---

## 4. Instrukcje dla platform

### Przeglądarka (gemini.google.com)

Działa na Windowsie, macOS i Linuxie. To pełny zestaw funkcji.

1. Otwórz [gemini.google.com](https://gemini.google.com) i zaloguj się.
2. W lewym panelu kliknij **Więcej** (*More*), a potem **Dostosuj** (*Customize*). Opcja „Dostosuj” może być schowana pod „Więcej”.
3. U góry wybierz zakładkę **Umiejętności** (*Skills*).
4. Kliknij **Utwórz** w prawym górnym rogu.
5. Wybierz **Prześlij**.
6. Wskaż plik `SKILL.md`, folder albo archiwum `.zip` (z `SKILL.md` w katalogu głównym) i kliknij **Otwórz**.
7. Opcjonalnie dodaj pliki referencyjne. Przy przesyłaniu całego folderu pojedyncze dodawanie plików jest pomijane.
8. Kliknij **Prześlij**, sprawdź umiejętność i kliknij **Utwórz**.
9. Umiejętność pojawi się na stronie Umiejętności.

Zamiast kroku 5 możesz wybrać **Utwórz ręcznie** (wpisujesz nazwę, opis i instrukcje) albo **Dodaj lub utwórz → Utwórz z Gemini**, żeby zbudować umiejętność w rozmowie.

Tylko w przeglądarce są dostępne: udostępnianie umiejętności (**Więcej → Udostępnij umiejętność**, role *Przeglądający* i *Edytujący*), zastępowanie umiejętności plikiem i zarządzanie plikami referencyjnymi.

### Aplikacja Gemini na Maca

Ta sekcja opiera się na nagraniu ekranu. Układ jest taki sam jak w przeglądarce, ale na nagraniu interfejs był po angielsku.

1. Otwórz aplikację Gemini.
2. W lewym panelu kliknij **More**, a z małego menu wybierz **Customize**.
3. U góry wybierz zakładkę **Skills**. Zobaczysz listy *Installed* i *Recommended*.
4. Kliknij **Create** w prawym górnym rogu. Są dwie opcje:
   - **Create manually** (*Write instructions*): wpisujesz instrukcje w aplikacji,
   - **Upload skill** (*From files or folder*): wgrywasz gotowy plik lub folder.
5. W oknie **Upload skill** przeciągnij folder do ramki albo wybierz **images**, **files** lub **folder**. Okno przypomina wymagania: nazwa w kebab-case i `SKILL.md` w głównym folderze.
6. Dokończ jak w przeglądarce (kroki 7–9 powyżej).

Nagranie kończy się na oknie przesyłania, więc kroki po wgraniu pochodzą z pomocy Google. W oknie jest też ostrzeżenie: wgrywaj pliki tylko z zaufanych źródeł.

### Android

W aplikacji mobilnej **nie można wgrać** `SKILL.md`, folderu ani `.zip`. Poniżej obejścia.

**Wejście na stronę Umiejętności:**

1. Otwórz aplikację Gemini.
2. U góry stuknij **Menu**, a potem **Dostosuj**. Jeśli nie widzisz „Dostosuj”, najpierw stuknij **Więcej**.
3. U góry wybierz **Umiejętności**.

**Sposób A: Utwórz ręcznie i wklej treść SKILL.md** (najbliższy odpowiednik wgrania pliku)

1. Stuknij **Dodaj lub utwórz**, a potem **Utwórz ręcznie**.
2. Wpisz **nazwę** (małe litery, łączniki) i **opis**, skopiowane z frontmatter pliku `SKILL.md`.
3. W polu **Instrukcje** wklej treść `SKILL.md` bez frontmatter, czyli to, co jest pod drugą linią `---`.
4. Opcjonalnie stuknij **Dodaj** i wybierz źródło plików: **obrazy** lub **pliki** z urządzenia, **Dysk Google**, **Zdjęcia Google** albo **Notatniki**. Potem stuknij **Prześlij**.
5. Stuknij **Utwórz** u góry ekranu.

**Sposób B: Poproś Gemini na czacie**

1. Stuknij **Dodaj lub utwórz**, potem **Utwórz z Gemini**.
2. Albo napisz w czacie: `Utwórz umiejętność na podstawie tych instrukcji:` i wklej treść `SKILL.md`, a potem stuknij **Prześlij**.
3. Zmiany opisujesz dalej na czacie.

**Sposób C: Dodaj skill na komputerze** i sprawdź listę w telefonie (patrz [sekcja 5](#5-polecany-przepływ-komputer--telefon)).

**Zarządzanie istniejącą umiejętnością:** otwórz ją i zmień opis lub instrukcje (**Zapisz**), albo stuknij **Więcej** i wybierz **Edytuj za pomocą Gemini**, **Dezaktywuj** / **Aktywuj**, **Pobierz** (plik `.zip`) lub **Usuń** (nie da się cofnąć).

### iPhone i iPad

Kroki są takie same jak na Androidzie: **Menu → Dostosuj → Umiejętności** (w razie potrzeby najpierw **Więcej**), a potem **Dodaj lub utwórz → Utwórz ręcznie** albo **Utwórz z Gemini**. Wgrywanie `SKILL.md`, folderu i `.zip` jest niedostępne.

Różnice względem Androida:

- konta służbowe i szkolne nie są na razie obsługiwane,
- opcja **Więcej → Zastąp umiejętność** jest opisana w pomocy, ale to samo źródło mówi, że przesyłanie plików w aplikacji mobilnej nie jest dostępne, więc nie liczyłbym na jej działanie,
- dodawanie, zastępowanie i usuwanie plików w istniejącej umiejętności wymaga przeglądarki,
- w czacie wpisz `/` (lub `@`, jeśli masz zaktualizowany skrót) i wybierz umiejętność.

### Gemini CLI (terminal)

To osobne narzędzie dla programistów. Umiejętność jest tu folderem na dysku, a nie wpisem na koncie.

> Według [dokumentacji](https://geminicli.com/docs/cli/skills/) Gemini CLI został 18 czerwca 2026 zastąpiony przez Antigravity CLI. Jeśli używasz nowszego narzędzia, sprawdź, czy poniższe ścieżki i komendy nadal działają.

| Zasięg | Ścieżka |
|---|---|
| Użytkownik (wszystkie projekty) | `~/.gemini/skills/<nazwa>/SKILL.md` (alias: `~/.agents/skills/`) |
| Workspace (jeden projekt) | `.gemini/skills/<nazwa>/SKILL.md` (alias: `.agents/skills/`) |

```bash
mkdir -p ~/.gemini/skills/moj-skill
# umieść w folderze SKILL.md z polami name i description
gemini
```

W sesji:

```text
/skills reload
/skills list
```

Przy pierwszym dopasowaniu Gemini CLI prosi o zgodę na aktywację. Instalacja z Gita: `gemini skills install <adres-repo> --scope workspace`. Usuwanie: `gemini skills uninstall <nazwa>`.

---

## 5. Polecany przepływ: komputer → telefon

1. Napisz `SKILL.md` na komputerze i przygotuj folder (sekcja 3).
2. Wgraj go w przeglądarce lub aplikacji na Maca (pełna kontrola nad plikami).
3. Na telefonie otwórz **Menu → Dostosuj → Umiejętności** i sprawdź, czy skill jest na liście. Pomoc Google wymienia umiejętności jako funkcję dostępną też w aplikacji mobilnej, ale nie znalazłem zapisu, że lista synchronizuje się natychmiast.
4. Jeśli skilla nie widać, utwórz go na telefonie ręcznie (Sposób A).
5. Drobne poprawki rób na telefonie przez **Edytuj za pomocą Gemini**. Zmiany plików referencyjnych rób w przeglądarce.

## 6. Rozwiązywanie problemów

| Objaw | Co sprawdzić |
|---|---|
| Błąd przy wgrywaniu | kebab-case w `name`, `SKILL.md` w katalogu głównym, rozmiar do 100 MB, ukryte pliki (`.DS_Store`), typy plików |
| Brak opcji „Prześlij” | jesteś w aplikacji mobilnej. Użyj przeglądarki lub Maca |
| Brak opcji „Dostosuj” | najpierw stuknij lub kliknij **Więcej** |
| Skill się nie uruchamia | czy jest **aktywny** (Więcej → Aktywuj), czy `description` pasuje do prośby, czy wywołujesz go przez `/` w czacie |
| Brak dostępu do Kalendarza lub Dysku | włącz **Zachowuj aktywność** |
| Aktualizacja plików w skillu | trzeba przesłać całą umiejętność ponownie razem z plikami referencyjnymi (w przeglądarce) |
| W CLI skill niewidoczny | `/skills reload`, poprawny YAML we frontmatter, ścieżka `skills/<nazwa>/SKILL.md` |

## 7. Źródła

- Nagranie ekranu z aplikacji Gemini na macOS: Skills → Create → Upload skill
- [Tworzenie i zarządzanie umiejętnościami w Gemini — pomoc Google (Android)](https://support.google.com/gemini/answer/17094296?hl=pl&co=GENIE.Platform%3DAndroid)
- [Tworzenie i zarządzanie umiejętnościami w Gemini — pomoc Google (iPhone i iPad)](https://support.google.com/gemini/answer/17094296?hl=pl&co=GENIE.Platform%3DiOS)
- [Agent Skills — dokumentacja Gemini CLI](https://geminicli.com/docs/cli/skills/)
