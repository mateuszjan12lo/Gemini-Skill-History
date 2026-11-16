# Jak dodać plik SKILL.md do Gemini

Przewodnik krok po kroku, jak dodać własną umiejętność (plik `SKILL.md`) do Gemini na komputerze, w telefonie i w terminalu. Pokazuje, co działa na której platformie, jak obejść brak wgrywania plików w aplikacji mobilnej i jak sprawdzić, czy umiejętność działa.

## Jak dodać umiejętność do Gemini (komputer)

Wgrywanie plików działa w przeglądarce i w aplikacji Gemini na Maca.

1. Wejdź na [gemini.google.com](https://gemini.google.com) i zaloguj się na konto Google. Na Macu możesz otworzyć aplikację Gemini.
2. W menu po lewej stronie kliknij **Więcej**.
3. Wybierz **Dostosuj**.
4. Na górze strony wybierz zakładkę **Umiejętności**.
5. Kliknij **Utwórz**.
6. Wybierz opcję **Prześlij**.
7. Wskaż plik `SKILL.md`, cały folder albo archiwum `.zip` (z `SKILL.md` w katalogu głównym).
8. Kliknij **Otwórz**, potem **Prześlij**, sprawdź umiejętność i kliknij **Utwórz**, aby ją zapisać.

Nazwy opcji w Gemini mogą się zmieniać. Jeśli któregoś kroku nie widzisz, poszukaj podobnej opcji w sekcji **Umiejętności**. W wersji angielskiej ścieżka to **More → Customize → Skills → Create → Upload skill**.

## Jak dodać umiejętność do Gemini (telefon)

W aplikacji mobilnej na Androidzie i iPhonie **nie da się wgrać** pliku `SKILL.md`, folderu ani `.zip`. Użyj jednego z obejść.

**Obejście A: utwórz ręcznie i wklej treść pliku**

1. Otwórz aplikację Gemini i stuknij **Menu**, a potem **Dostosuj**. Jeśli nie widzisz „Dostosuj”, najpierw stuknij **Więcej**.
2. Wybierz zakładkę **Umiejętności**.
3. Stuknij **Dodaj lub utwórz**, a potem **Utwórz ręcznie**.
4. W polach **nazwa** i **opis** wpisz to, co jest w nagłówku `SKILL.md` (między liniami `---`).
5. W polu **Instrukcje** wklej resztę pliku, czyli wszystko pod drugą linią `---`.
6. Stuknij **Utwórz** u góry ekranu.

**Obejście B: poproś Gemini na czacie**

Napisz w czacie `Utwórz umiejętność na podstawie tych instrukcji:`, wklej treść `SKILL.md` i wyślij. Umiejętność pojawi się na stronie Umiejętności.

**Obejście C: dodaj na komputerze**

Wgraj plik według instrukcji wyżej, a potem sprawdź w telefonie w **Menu → Dostosuj → Umiejętności**. Nie znalazłem zapisu, że lista synchronizuje się natychmiast, więc w razie braku użyj obejścia A.

## Jak dodać umiejętność w Gemini CLI

To osobne narzędzie dla programistów. Umiejętność jest folderem na dysku.

1. Utwórz folder: `mkdir -p ~/.gemini/skills/moj-skill` (dla jednego projektu: `.gemini/skills/moj-skill`).
2. Umieść w nim plik `SKILL.md`.
3. Uruchom `gemini` i wpisz `/skills reload`, a potem `/skills list`.
4. Zadaj pytanie pasujące do opisu. Gemini poprosi o zgodę na aktywację umiejętności.

Według [dokumentacji](https://geminicli.com/docs/cli/skills/) Gemini CLI został 18 czerwca 2026 zastąpiony przez Antigravity CLI. Jeśli używasz nowszego narzędzia, sprawdź, czy ścieżki i komendy nadal działają.

## Jak przygotować SKILL.md

Struktura folderu:

```text
moj-skill/
├── SKILL.md
└── (opcjonalnie pliki pomocnicze: .md, .pdf, .csv, .py)
```

Minimalny plik:

```markdown
---
name: moj-skill
description: Krótko opisz, do czego służy umiejętność i kiedy Gemini ma jej użyć.
---

# Instrukcje

Napisz, jak Gemini ma wykonywać zadanie: kroki, styl odpowiedzi, ograniczenia.
```

Opis (`description`) decyduje, kiedy Gemini sięga po umiejętność. Wpisz w nim konkretne zadania i słowa, których użyjesz w prośbach.

## Jak używać

1. Rozpocznij nowy czat w Gemini.
2. Wpisz `/` (lub `@`, jeśli masz zaktualizowany skrót) i wybierz umiejętność z podpowiedzi.
3. Napisz, co chcesz zrobić. Gemini używa też automatycznie włączonych umiejętności, gdy zadanie pasuje do ich opisu.

## Co działa na której platformie

| Działanie | Przeglądarka | Mac | Android | iPhone / iPad |
|---|:---:|:---:|:---:|:---:|
| Wgranie `SKILL.md`, folderu lub `.zip` | tak | tak | nie | nie |
| Utwórz ręcznie | tak | tak | tak | tak |
| Utwórz z Gemini na czacie | tak | tak | tak | tak |
| Edycja opisu i instrukcji | tak | tak | tak | tak |
| Edytuj za pomocą Gemini | tak | tak | tak | tak |
| Włączanie, wyłączanie, pobieranie, usuwanie | tak | tak | tak | tak |
| Zastąpienie umiejętności plikiem | tak | ? | nie | nie |
| Dodawanie i usuwanie plików w umiejętności | tak | ? | nie | nie |
| Udostępnianie innym | tak | ? | nie | nie |

Znak `?` oznacza, że nie sprawdzałem tego. Kolumna Mac opiera się na nagraniu ekranu (wgrywanie i tworzenie ręczne) oraz na tym, że pomoc Google wymienia aplikację na Maca wśród platform z umiejętnościami. Pozostałe kolumny pochodzą z oficjalnej pomocy Google.

## Ważne

- Plik musi nazywać się dokładnie `SKILL.md` (wielkie litery, rozszerzenie `.md`) i leżeć w katalogu głównym folderu lub archiwum.
- Nazwa w `SKILL.md` musi być zapisana małymi literami, a słowa oddzielone łącznikami (kebab-case), np. `moj-nauczyciel-niemieckiego`.
- Do Gemini wgrywasz `SKILL.md`, a nie `README.md`. Zasady działania umiejętności muszą być w `SKILL.md`.
- Limit: 100 MB łącznie. Obsługiwane typy: .docx, .pdf, .md, .txt, .csv, .xlsx, .pptx, .jpg, .png, .webp, .py, .js, .sh, .json, .yaml, .xml. Nieobsługiwane: .doc, .xls, .ppt, audio, wideo, archiwa w środku folderu oraz m.in. .ts, .tsx, .jsx, .php, .sql.
- Przed wgraniem usuń pliki ukryte i binarne (`.DS_Store`, `.pyc`), bo powodują błąd.
- Skrypty nie mogą wykonywać działań w sieci ani wysyłać żądań do zewnętrznych stron.
- Żeby zaktualizować pliki w umiejętności, prześlij ją w przeglądarce jeszcze raz razem z plikami referencyjnymi.
- Wymagania konta: ukończone 18 lat i włączona opcja **Zachowuj aktywność**. Przy wyłączonej umiejętności działają, ale bez dostępu do Kalendarza i Dysku Google. Na iPhonie konta służbowe i szkolne nie są na razie obsługiwane.
- Wgrywaj pliki tylko z zaufanych źródeł.
- Jeśli umiejętność nie pojawia się po wpisaniu `/` lub `@`, sprawdź, czy została zapisana, czy jest **aktywna** (**Więcej → Aktywuj**) i czy używasz tego samego konta Google.

## Źródła

- Nagranie ekranu z aplikacji Gemini na macOS: Skills → Create → Upload skill
- [Pomoc Google: umiejętności na Androidzie](https://support.google.com/gemini/answer/17094296?hl=pl&co=GENIE.Platform%3DAndroid)
- [Pomoc Google: umiejętności na iPhonie i iPadzie](https://support.google.com/gemini/answer/17094296?hl=pl&co=GENIE.Platform%3DiOS)
- [Agent Skills w dokumentacji Gemini CLI](https://geminicli.com/docs/cli/skills/)
