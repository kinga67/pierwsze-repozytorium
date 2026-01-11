# Fundamenty: Tydzień 1-2

*GitHub GUI, Issues, Projects, Pull Requests*

---

## Wprowadzenie

Ten dokument zawiera szczegółowe informacje i praktyczne zadania dla pierwszych dwóch tygodni wdrożenia. Wszystkie operacje wykonywane są wyłącznie przez interfejs graficzny GitHub (GUI) - **nie używamy konsoli ani Git CLI**.

**Czas trwania:** 2 tygodnie  
**Poziom:** Podstawowy  
**Narzędzie:** GitHub.com (przeglądarka)

---

## Tydzień 1: Git i GitHub przez GUI

### 1.1. Wprowadzenie do kontroli wersji

#### Informacje

**Kontrola wersji** to system śledzenia zmian w plikach. W projektach IT pozwala na:
- Przechowywanie historii zmian
- Współpracę wielu osób nad tym samym kodem
- Cofanie błędnych zmian
- Tworzenie równoległych wersji (branchy)

**GitHub** to platforma hostująca repozytoria Git z dodatkowymi funkcjami:
- Issues (zadania, błędy)
- Projects (tablice Kanban)
- Pull Requests (prośby o połączenie zmian)
- Code Review (przegląd kodu)

#### Kluczowe pojęcia

* **Repozytorium (repo)** - folder projektu na GitHubie zawierający wszystkie pliki i historię zmian
* **Commit** - zapisana zmiana w repozytorium (jak "zapis" w historii)
* **Branch** - równoległa wersja kodu (np. "main" - główna, "feature/login" - nowa funkcja)
* **Merge** - połączenie zmian z jednego brancha do drugiego **[ZAAWANSOWANE]**
* **Pull Request (PR)** - prośba o połączenie zmian z jednego brancha do drugiego

---

### 1.2. Zakładanie i konfiguracja repozytorium

#### Informacje

Repozytorium na GitHubie może być:
- **Publiczne** - widoczne dla wszystkich
- **Prywatne** - widoczne tylko dla wybranych osób

Każde repozytorium ma:
- **README.md** - główny plik dokumentacji (wyświetla się na stronie głównej repo)
- **Settings** - ustawienia (dostęp, integracje, szablony)
- **Insights** - statystyki i metryki

📚 **Dokumentacja GitHub:** [Tworzenie nowego repozytorium](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

#### Zadania

**Zadanie 1.1: Utworzenie repozytorium testowego**

1. Zaloguj się na GitHub.com
2. Kliknij przycisk **"+"** w prawym górnym rogu → **"New repository"**
3. Wypełnij formularz:
   - **Repository name:** `moje-pierwsze-repo` (lub inna nazwa)
   - **Description:** "Repozytorium testowe do nauki GitHub"
   - **Visibility:** Wybierz **Private** (prywatne)
   - **Initialize this repository with:**
     - ✅ Zaznacz **"Add a README file"**
     - ✅ Zaznacz **"Add .gitignore"** → wybierz template (np. "Node")
4. Kliknij **"Create repository"**

**Zadanie 1.2: Przegląd interfejsu repozytorium**

1. Po utworzeniu repo, zapoznaj się z elementami interfejsu:
   - **Code** - pliki i foldery projektu
   - **Issues** - zadania i błędy
   - **Pull requests** - prośby o połączenie zmian
   - **Actions** - automatyzacja (CI/CD)
   - **Projects** - tablice Kanban
   - **Wiki** - dokumentacja wiki
   - **Settings** - ustawienia

2. Przejdź do zakładki **Code** i sprawdź:
   - Jak wygląda plik README.md
   - Jak wygląda plik .gitignore
   - Przycisk **"Add file"** (dodawanie plików)

**Zadanie 1.3: Edycja pliku przez GUI**

1. W zakładce **Code**, kliknij na plik **README.md**
2. Kliknij ikonę ołówka (✏️) **"Edit this file"** w prawym górnym rogu
3. Dodaj tekst:
   ```markdown
   # Moje pierwsze repozytorium
   
   To jest repozytorium testowe do nauki GitHub.
   
   ## Funkcje
   - Nauka Git i GitHub
   - Praca z Issues
   - Zarządzanie projektami
   ```
4. Przewiń w dół i wypełnij formularz **"Commit changes"**:
   - **Commit message:** "Dodano opis do README"
   - **Description (opcjonalne):** "Pierwsza edycja pliku przez GUI"
5. Wybierz opcję **"Commit directly to the main branch"**
6. Kliknij **"Commit changes"**

📚 **Dokumentacja GitHub:** [Edycja plików w repozytorium](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files)

**Zadanie 1.4: Tworzenie nowego pliku**

1. W zakładce **Code**, kliknij przycisk **"Add file"** → **"Create new file"**
2. W polu nazwy pliku wpisz: `informacje.md`
3. W edytorze dodaj treść:
   ```markdown
   # Informacje o projekcie
   
   Data utworzenia: [wpisz dzisiejszą datę]
   
   ## Cel projektu
   Nauka pracy z GitHub przez interfejs graficzny.
   ```
4. Przewiń w dół i wypełnij **"Commit changes"**:
   - **Commit message:** "Dodano plik informacje.md"
5. Kliknij **"Commit new file"**

📚 **Dokumentacja GitHub:** [Tworzenie nowych plików](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-or-editing-files#creating-new-files)

**Zadanie 1.5: Przegląd historii zmian**

1. W zakładce **Code**, kliknij na liczbę commitów (np. "2 commits") obok nazwy brancha
2. Zobaczysz listę wszystkich commitów z:
   - Autorem
   - Datą i godziną
   - Komentarzem commit message
3. Kliknij na dowolny commit, aby zobaczyć szczegóły zmian (diff)

📚 **Dokumentacja GitHub:** [Przeglądanie historii commitów](https://docs.github.com/en/repositories/working-with-files/using-files/viewing-a-file#viewing-commit-history)

---

### 1.3. Markdown jako standard dokumentacji

#### Informacje

**Markdown** to język formatowania tekstu używany powszechnie w dokumentacji IT. Pliki Markdown mają rozszerzenie `.md`.

📚 **Dokumentacja GitHub:** [Podstawowe formatowanie i składnia zapisu](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

#### Podstawowa składnia Markdown

```markdown
# Nagłówek 1
## Nagłówek 2
### Nagłówek 3

**pogrubienie** lub __pogrubienie__
*kursywa* lub _kursywa_

- Lista punktowana
- Kolejny punkt

1. Lista numerowana
2. Kolejny punkt

[Link](https://github.com)

`kod inline`

```kod w bloku```

> Cytat

| Tabela | Kolumna 2 |
|--------|-----------|
| Wiersz 1 | Dane |
```

#### Zadania

**Zadanie 1.6: Utworzenie dokumentacji w Markdown**

1. Utwórz nowy plik `dokumentacja.md` (Add file → Create new file)
2. Dodaj strukturę dokumentacji:
   ```markdown
   # Dokumentacja projektu
   
   ## Wprowadzenie
   Krótki opis projektu.
   
   ## Instalacja
   Instrukcje instalacji.
   
   ## Użycie
   Jak korzystać z projektu.
   
   ## Kontakt
   Informacje kontaktowe.
   ```
3. Commit: "Dodano dokumentację w Markdown"

**Zadanie 1.7: Formatowanie tekstu**

1. Edytuj plik `README.md`
2. Dodaj sekcję z różnymi formatowaniami:
   ```markdown
   ## Formatowanie
   
   To jest **pogrubiony tekst**.
   To jest *tekst kursywą*.
   
   Lista zakupów:
   - Mleko
   - Chleb
   - Jajka
   
   Link do [GitHub](https://github.com).
   ```
3. Commit: "Dodano przykłady formatowania Markdown"

---

### 1.4. Przegląd projektów open-source

#### Informacje

Projekty open-source na GitHubie to doskonałe źródło nauki:
- Jak organizować repozytoria
- Jak pisać dokumentację
- Jak zarządzać Issues i Pull Requests
- Jakie standardy stosować

#### Zadania

**Zadanie 1.8: Analiza projektu open-source**

1. Przejdź do repozytorium: `https://github.com/microsoft/vscode` (lub innego popularnego projektu)
2. Przeanalizuj strukturę:
   - Jak wygląda README.md?
   - Jakie pliki są w głównym katalogu?
   - Jak zorganizowane są foldery?
3. Sprawdź zakładkę **Issues**:
   - Jak wyglądają otwarte Issues?
   - Jakie etykiety są używane?
   - Jak wygląda szablon Issue?
4. Sprawdź zakładkę **Pull requests**:
   - Jak wygląda otwarty PR?
   - Jakie informacje zawiera?
5. Sprawdź zakładkę **Projects**:
   - Czy projekt używa tablicy Kanban?
   - Jak zorganizowane są kolumny?

**Zadanie 1.9: Notatki z analizy**

1. W swoim repozytorium utwórz plik `analiza-projektow.md`
2. Zapisz obserwacje:
   ```markdown
   # Analiza projektów open-source
   
   ## Projekt: [nazwa]
   
   ### Struktura
   - [co zauważyłeś]
   
   ### Issues
   - [jakie etykiety, jak wyglądają]
   
   ### Pull Requests
   - [jakie informacje zawierają]
   ```
3. Commit: "Dodano analizę projektów open-source"

---

## Tydzień 2: Issues, Projects i współpraca

### 2.1. Zarządzanie zadaniami przez GitHub Issues

#### Informacje

**GitHub Issues** to system zarządzania zadaniami, błędami i prośbami o funkcje. Każde Issue to:
- Zadanie do wykonania
- Zgłoszony błąd
- Prośba o nową funkcję
- Pytanie lub dyskusja

Issue może mieć:
- **Tytuł** - krótki opis
- **Opis** - szczegóły zadania
- **Etykiety (Labels)** - kategoryzacja
- **Przypisanie (Assignees)** - osoba odpowiedzialna
- **Milestone** - kamień milowy/wersja
- **Projekty** - powiązanie z tablicą Kanban

📚 **Dokumentacja GitHub:** 
- [Tworzenie Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue)
- [Zarządzanie etykietami](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels)

#### Zadania

**Zadanie 2.1: Utworzenie pierwszego Issue**

1. W swoim repozytorium przejdź do zakładki **Issues**
2. Kliknij **"New issue"**
3. Wypełnij formularz:
   - **Title:** "Dodać sekcję 'O projekcie' do README"
   - **Comment:**
     ```markdown
     ## Opis
     Należy dodać sekcję opisującą cel projektu w pliku README.md.
     
     ## Zadanie
     - [ ] Dodać nagłówek "O projekcie"
     - [ ] Napisać 2-3 zdania o celu projektu
     - [ ] Zaktualizować README.md
     
     ## Kryteria akceptacji
     - README zawiera sekcję "O projekcie"
     - Sekcja zawiera opis celu projektu
     ```
4. Kliknij **"Submit new issue"**

**Zadanie 2.2: Zarządzanie etykietami (Labels)**

1. W zakładce **Issues**, kliknij **"Labels"** (lub przejdź do Settings → Labels)
2. Utwórz nowe etykiety:
   - **"enhancement"** - kolor zielony, opis: "Nowa funkcja lub ulepszenie"
   - **"bug"** - kolor czerwony, opis: "Coś nie działa"
   - **"documentation"** - kolor niebieski, opis: "Zmiany w dokumentacji"
   - **"task"** - kolor szary, opis: "Zadanie do wykonania"
3. Wróć do utworzonego Issue i dodaj etykietę **"documentation"**:
   - Kliknij na Issue
   - Po prawej stronie kliknij **"Labels"** → wybierz **"documentation"**

**Zadanie 2.3: Przypisanie i zamknięcie Issue**

1. W otwartym Issue, po prawej stronie:
   - Kliknij **"Assignees"** → wybierz siebie
   - Kliknij **"Labels"** → dodaj etykietę (jeśli jeszcze nie ma)
2. Wykonaj zadanie z Issue:
   - Edytuj README.md i dodaj sekcję "O projekcie"
   - Commit: "Dodano sekcję 'O projekcie' do README"
3. Zamknij Issue:
   - W komentarzu napisz: "Zadanie wykonane, sekcja dodana do README"
   - Kliknij **"Close issue"** (lub użyj słowa kluczowego: "Closes #1" w komentarzu commit)

**Zadanie 2.4: Utworzenie kilku Issues**

Utwórz 3-4 różne Issues:
1. **Bug:** "Błąd w formatowaniu tabeli w dokumentacji.md"
2. **Enhancement:** "Dodać sekcję 'Instalacja' do README"
3. **Task:** "Przejrzeć i zaktualizować wszystkie pliki Markdown"
4. **Documentation:** "Dodać przykłady użycia do dokumentacji"

Dla każdego:
- Dodaj odpowiednie etykiety
- Napisz szczegółowy opis
- Użyj checklisty w opisie (jeśli dotyczy)

---

### 2.2. Milestone'y i organizacja

#### Informacje

**Milestone** to kamień milowy - grupa Issues powiązanych z konkretnym celem lub wersją (np. "Wersja 1.0", "Sprint 1", "Fundamenty - Tydzień 1").

Milestone pomaga:
- Grupować powiązane zadania
- Śledzić postęp
- Planować release'y

📚 **Dokumentacja GitHub:** [O milestone'ach](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones)

#### Zadania

**Zadanie 2.5: Utworzenie Milestone**

1. W zakładce **Issues**, kliknij **"Milestones"** → **"New milestone"**
2. Wypełnij formularz:
   - **Title:** "Fundamenty - Tydzień 1"
   - **Description:** "Zadania z pierwszego tygodnia wdrożenia"
   - **Due date:** Ustaw datę końca tygodnia
3. Kliknij **"Create milestone"**
4. Wróć do Issues i przypisz 2-3 Issues do tego Milestone:
   - Otwórz Issue
   - Po prawej stronie kliknij **"Milestone"** → wybierz utworzony Milestone

**Zadanie 2.6: Przegląd postępu Milestone**

1. Przejdź do **Issues** → **Milestones**
2. Kliknij na utworzony Milestone
3. Zobaczysz:
   - Listę Issues przypisanych do Milestone
   - Pasek postępu (ile Issues zamkniętych)
   - Statystyki

---

### 2.3. GitHub Projects (Kanban, Timeline)

#### Informacje

**GitHub Projects** to tablice Kanban do wizualizacji i zarządzania pracą. Projekty mogą być:
- **Board (Kanban)** - kolumny z kartami (To Do, In Progress, Done)
- **Table** - widok tabelaryczny
- **Timeline** - widok czasowy (dla planowania)

Karty na tablicy mogą reprezentować:
- Issues
- Pull Requests
- Notatki (Notes)

📚 **Dokumentacja GitHub:** 
- [O Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)
- [Tworzenie projektu](https://docs.github.com/en/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project)

#### Zadania

**Zadanie 2.7: Utworzenie projektu Kanban**

1. W repozytorium kliknij zakładkę **Projects**
2. Kliknij **"New project"**
3. Wybierz **"Board"** (Kanban)
4. Wypełnij:
   - **Project name:** "Mój pierwszy projekt"
   - **Description:** "Tablice Kanban do zarządzania zadaniami"
5. Kliknij **"Create"**
6. Domyślnie utworzą się kolumny: **"Todo"**, **"In progress"**, **"Done"**

**Zadanie 2.8: Dodanie Issues do projektu**

1. W projekcie Kanban kliknij **"Add item"** (lub **"+"**)
2. Wybierz **"Issue"**
3. Wybierz jedno z utworzonych Issues
4. Powtórz dla 3-4 Issues
5. Zobaczysz karty Issues na tablicy

**Zadanie 2.9: Zarządzanie kartami na tablicy**

1. **Przenoszenie kart:**
   - Kliknij i przeciągnij kartę z kolumny "Todo" do "In progress"
   - To oznacza, że zadanie jest w trakcie realizacji

2. **Edycja karty:**
   - Kliknij na kartę
   - Możesz dodać notatki, zmienić przypisanie, dodać etykiety

3. **Dodanie notatki:**
   - Kliknij **"Add item"** → **"Draft issue"** (lub **"Note"**)
   - Napisz notatkę, np. "Pamiętać o aktualizacji dokumentacji"

4. **Zmiana statusu:**
   - Przenieś kartę do kolumny "Done", gdy zadanie jest ukończone

**Zadanie 2.10: Konfiguracja kolumn**

1. W projekcie kliknij **"..."** (trzy kropki) obok nazwy kolumny
2. Wybierz **"Edit column"**
3. Możesz:
   - Zmienić nazwę kolumny
   - Ustawić limit kart (np. max 3 karty w "In progress")
   - Dodać automatyzację (np. automatyczne przenoszenie do "Done", gdy Issue jest zamknięte)

4. Dodaj nową kolumnę:
   - Kliknij **"Add column"**
   - Nazwa: **"Review"** (do przeglądu)
   - Umieść między "In progress" a "Done"

---

### 2.4. Pull Requests i Code Review

#### Informacje

**Pull Request (PR)** to prośba o połączenie zmian z jednego brancha do drugiego. PR umożliwia:
- Przegląd zmian przed połączeniem
- Dyskusję nad kodem
- Testowanie zmian
- Współpracę nad kodem

Typowy workflow:
1. Utworzenie brancha z nową funkcją
2. Wprowadzenie zmian
3. Utworzenie PR
4. Code Review (przegląd kodu)
5. **[ZAAWANSOWANE]** Merge (połączenie zmian)

**Uwaga:** W tym kursie używamy tylko GUI, więc branchy tworzymy przez interfejs GitHub.

📚 **Dokumentacja GitHub:** 
- [O Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
- [Tworzenie Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- [Tworzenie i usuwanie branchy w repozytorium](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-the-default-branch-name-for-repositories-in-your-organization)

#### Zadania

**Zadanie 2.11: Utworzenie brancha przez GUI**

1. W zakładce **Code**, kliknij na nazwę brancha (domyślnie "main")
2. W polu wyszukiwania wpisz nową nazwę: `feature/dodaj-sekcje-kontakt`
3. Kliknij **"Create branch: feature/dodaj-sekcje-kontakt from 'main'"**
4. Zostaniesz przekierowany do nowego brancha

📚 **Dokumentacja GitHub:** [Tworzenie i usuwanie branchy w repozytorium](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-or-editing-files#creating-a-file-on-a-branch)

**Zadanie 2.12: Edycja pliku w nowym branchu**

1. W branchu `feature/dodaj-sekcje-kontakt` edytuj plik README.md
2. Dodaj sekcję:
   ```markdown
   ## Kontakt
   
   W razie pytań, proszę o kontakt przez Issues.
   ```
3. Commit: "Dodano sekcję Kontakt"

**Zadanie 2.13: Utworzenie Pull Request**

1. Po commit w nowym branchu, GitHub pokaże żółty baner z przyciskiem **"Compare & pull request"**
2. Kliknij **"Compare & pull request"** (lub przejdź do **Pull requests** → **New pull request**)
3. Wypełnij formularz:
   - **Title:** "Dodano sekcję Kontakt do README"
   - **Description:**
     ```markdown
     ## Zmiany
     Dodano sekcję "Kontakt" do pliku README.md.
     
     ## Powód
     Issue #X (dodaj numer swojego Issue)
     
     ## Sprawdzenie
     - [x] Plik został zaktualizowany
     - [x] Formatowanie Markdown jest poprawne
     ```
4. Po prawej stronie:
   - **Reviewers:** Możesz poprosić kogoś o przegląd (jeśli masz współpracowników)
   - **Assignees:** Przypisz siebie
   - **Labels:** Dodaj etykietę "documentation"
5. Kliknij **"Create pull request"**

📚 **Dokumentacja GitHub:** [Tworzenie Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)

**Zadanie 2.14: Przegląd Pull Request**

1. W zakładce **Pull requests** otwórz utworzony PR
2. Zobaczysz:
   - **Conversation** - dyskusja i komentarze
   - **Files changed** - lista zmienionych plików z diff (różnice)
3. W **Files changed**:
   - Zielone linie = dodane
   - Czerwone linie = usunięte
   - Możesz dodać komentarz do konkretnej linii (hover → ikona "+")

📚 **Dokumentacja GitHub:** [Przeglądanie zmian w Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)

**Zadanie 2.15: Merge Pull Request**

1. W otwartym PR, przewiń w dół
2. Kliknij **"Merge pull request"**
3. **[ZAAWANSOWANE]** Wybierz typ merge:
   - **Create a merge commit** - zachowuje historię brancha (podstawowa opcja)
   - **Squash and merge** - łączy wszystkie commity w jeden (zaawansowane)
   - **Rebase and merge** - liniowa historia (zaawansowane)
4. Dla nauki wybierz **"Create a merge commit"**
5. Kliknij **"Confirm merge"**
6. Po merge możesz usunąć branch (przycisk **"Delete branch"**)

📚 **Dokumentacja GitHub:** 
- [Scalanie Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request)
- **[ZAAWANSOWANE]** [O metodach scalania na GitHubie](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/about-merge-methods-on-github)
- **[ZAAWANSOWANE]** [Konfigurowanie scalania commitów dla pull requestów (squash)](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/configuring-commit-squashing-for-pull-requests)

**Zadanie 2.16: Code Review (symulacja)**

1. Utwórz kolejny branch: `feature/dodaj-licencje`
2. Dodaj plik `LICENSE.md` z prostą licencją:
   ```markdown
   # Licencja
   
   Ten projekt jest dostępny na licencji MIT.
   ```
3. Utwórz PR
4. W PR dodaj komentarz do siebie (symulacja review):
   - W **Files changed** kliknij na linię
   - Dodaj komentarz: "Czy możemy dodać więcej szczegółów o licencji?"
5. Odpowiedz na komentarz w **Conversation**
6. Zaktualizuj plik (edytuj w branchu, dodaj commit)
7. **[ZAAWANSOWANE]** Merge PR (możesz wypróbować różne metody merge)

📚 **Dokumentacja GitHub:** [Przeglądanie zmian w Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)

---

### 2.5. Szablony PR i Issues

#### Informacje

**Szablony** to gotowe formularze dla Issues i Pull Requests, które zapewniają:
- Spójność informacji
- Kompletność danych
- Łatwiejsze zarządzanie

Szablony przechowujemy w folderze `.github` w repozytorium:
- `.github/ISSUE_TEMPLATE/` - szablony Issues
- `.github/pull_request_template.md` - szablon PR

📚 **Dokumentacja GitHub:** 
- [Szablony Issues i Pull Requests](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates)
- [Tworzenie szablonu Issue](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-issue-templates-for-your-repository)
- [Tworzenie szablonu Pull Request](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository)

#### Zadania

**Zadanie 2.17: Utworzenie szablonu Issue**

1. W zakładce **Code** kliknij **"Add file"** → **"Create new file"**
2. Wpisz nazwę: `.github/ISSUE_TEMPLATE/bug_report.md`
   - GitHub automatycznie utworzy folder `.github/ISSUE_TEMPLATE/`
3. Dodaj treść szablonu:
   ```markdown
   ---
   name: Zgłoszenie błędu
   about: Zgłoś błąd, aby pomóc nam ulepszyć projekt
   title: '[BUG] '
   labels: bug
   assignees: ''
   ---
   
   ## Opis błędu
   Krótki i jasny opis błędu.
   
   ## Kroki do odtworzenia
   1. Przejdź do '...'
   2. Kliknij na '....'
   3. Przewiń w dół do '....'
   4. Zobacz błąd
   
   ## Oczekiwane zachowanie
   Opisz, co powinno się wydarzyć.
   
   ## Zrzuty ekranu
   Jeśli dotyczy, dodaj zrzuty ekranu.
   
   ## Środowisko
   - System operacyjny: [np. macOS, Windows]
   - Przeglądarka: [np. Chrome, Firefox]
   - Wersja: [np. 1.0.0]
   
   ## Dodatkowe informacje
   Inne informacje o problemie.
   ```
4. Commit: "Dodano szablon Issue dla zgłoszeń błędów"

**Zadanie 2.18: Utworzenie szablonu dla Feature Request**

1. Utwórz kolejny szablon: `.github/ISSUE_TEMPLATE/feature_request.md`
2. Treść:
   ```markdown
   ---
   name: Prośba o funkcję
   about: Zaproponuj pomysł na projekt
   title: '[FEATURE] '
   labels: enhancement
   assignees: ''
   ---
   
   ## Opis funkcji
   Jasny i zwięzły opis funkcji, którą chcesz zobaczyć.
   
   ## Problem, który rozwiązuje
   Jaki problem rozwiązuje ta funkcja?
   
   ## Proponowane rozwiązanie
   Jak powinna działać ta funkcja?
   
   ## Alternatywy
   Rozważane alternatywne rozwiązania.
   
   ## Dodatkowe informacje
   Inne informacje lub zrzuty ekranu.
   ```
3. Commit: "Dodano szablon Issue dla prośb o funkcje"

**Zadanie 2.19: Utworzenie szablonu Pull Request**

1. Utwórz plik: `.github/pull_request_template.md`
2. Treść:
   ```markdown
   ## Opis zmian
   Krótki opis zmian wprowadzonych w tym PR.
   
   ## Typ zmian
   - [ ] Bug fix
   - [ ] Nowa funkcja
   - [ ] Zmiana w dokumentacji
   - [ ] Refaktoryzacja
   - [ ] Inne (opisz)
   
   ## Powiązane Issues
   Zamyka #X (dodaj numer Issue)
   
   ## Sprawdzenie
   - [ ] Kod został przetestowany
   - [ ] Dokumentacja została zaktualizowana
   - [ ] Nie ma błędów w konsoli
   - [ ] Zmiany są zgodne z wytycznymi projektu
   
   ## Zrzuty ekranu
   Jeśli dotyczy, dodaj zrzuty ekranu.
   
   ## Dodatkowe informacje
   Inne informacje dla reviewerów.
   ```
3. Commit: "Dodano szablon Pull Request"

**Zadanie 2.20: Testowanie szablonów**

1. Przejdź do **Issues** → **New issue**
2. Zobaczysz opcje wyboru szablonu:
   - "Zgłoszenie błędu"
   - "Prośba o funkcję"
   - "Blank" (pusty)
3. Wybierz "Zgłoszenie błędu" i sprawdź, czy szablon się wczytał
4. Utwórz nowy PR i sprawdź, czy szablon PR się wczytał

---

## Podsumowanie Tygodnia 1-2

### Co powinieneś umieć:

✅ **Tydzień 1:**
- Utworzyć i skonfigurować repozytorium na GitHubie
- Edytować pliki przez GUI
- Tworzyć nowe pliki i foldery
- Rozumieć podstawy Markdown
- Przeglądać historię zmian
- Analizować projekty open-source

✅ **Tydzień 2:**
- Tworzyć i zarządzać Issues
- Używać etykiet, milestone'ów i przypisań
- Tworzyć i konfigurować projekty Kanban
- Tworzyć branchy przez GUI
- Tworzyć i merge'ować Pull Requests (podstawowe)
- **[ZAAWANSOWANE]** Rozumieć różne metody merge (squash, rebase)
- Tworzyć szablony dla Issues i PR

### Artefakty do utworzenia:

- [ ] Repozytorium testowe z dokumentacją
- [ ] Minimum 5 Issues z różnymi etykietami
- [ ] Milestone z przypisanymi Issues
- [ ] Projekt Kanban z kartami
- [ ] Minimum 2 Pull Requests (utworzone i zmerge'owane)
- [ ] Szablony Issue (bug, feature request)
- [ ] Szablon Pull Request

### Sprawdzenie wiedzy:

Odpowiedz na pytania:
1. Czym różni się Issue od Pull Request?
2. Do czego służy Milestone?
3. Jakie są korzyści z używania szablonów?
4. Co to jest Code Review?
5. Jak działa tablica Kanban w GitHub Projects?

---

## Przydatne linki

### Ogólne
- [GitHub Docs](https://docs.github.com) - pełna dokumentacja GitHub
- [GitHub Skills](https://skills.github.com) - interaktywne kursy GitHub
- [Markdown Guide](https://www.markdownguide.org) - przewodnik po składni Markdown
- [GitHub Guides](https://guides.github.com) - przewodniki GitHub

### Konkretne tematy
- [Tworzenie repozytorium](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)
- [Tworzenie Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue)
- [Zarządzanie etykietami](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels)
- [Tworzenie Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- [Scalanie Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request)
- [GitHub Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)

### [ZAAWANSOWANE] Metody scalania
- [O metodach scalania na GitHubie](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/about-merge-methods-on-github)
- [Konfigurowanie scalania commitów (squash)](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/configuring-commit-squashing-for-pull-requests)
- [Konfigurowanie rebase merge](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/configuring-commit-rebasing-for-pull-requests)

---

## Następne kroki

Po ukończeniu fundamentów przejdź do ścieżek specjalizacyjnych:
- **Project Manager:** Procesy IT i Agile
- **QA:** Podstawy testowania

---

*Dokument utworzony: [data]*  
*Wersja: 1.0*

