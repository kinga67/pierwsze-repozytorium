## Jira – Backlog management, backlog refinement, priorytetyzacja

* **Backlog management**: tworzenie i utrzymywanie listy wszystkich zadań w projekcie. Podział na epiki, story, taski. Priorytety według wartości biznesowej i ryzyka.
* **Backlog refinement**: regularne spotkania PM z zespołem w celu doprecyzowania zadań, dodania estymat, rozbicia dużych tasków na mniejsze.
* **Priorytetyzacja**: ustawianie kolejności realizacji tasków, zgodnie z wartością dla klienta i ograniczeniami budżetowymi.

---

## Jira – Roadmap, versions, releases, milestones

* **Roadmap**: wizualizacja planowanych epików i ich terminów w czasie.
* **Versions / Releases**: tworzenie wersji projektu w Jira, przypisanie zadań do release’ów.
* **Milestones**: punkty kontrolne projektu, przypisanie epików lub story do milestone, monitoring ukończenia.

---

## Jira – Workflow design, statusy, przejścia statusów

* **Workflow design**: definiowanie statusów zadań (Backlog, Selected, In Progress, Code Review, Testing, Done).
* **Statusy**: zdefiniowane etapy tasków w Jira.
* **Przejścia statusów**: automatyczne lub manualne zmiany statusów w oparciu o akcje deweloperów, np. po zamknięciu review status przechodzi do Testing.

---

## Jira – Dependency management, acceptance criteria, definition of done

* **Dependency management**: określanie zależności między taskami lub epikami, aby unikać blokad.
* **Acceptance criteria**: szczegółowe wymagania, które muszą być spełnione, aby zadanie uznać za zakończone.
* **Definition of Done (DoD)**: standardy, które muszą być spełnione przy zamknięciu taska – kod, testy, review, QA.

---

## Jira – Tempo – konfiguracja budżetu projektu, budget hours

* Ustawienie całkowitego budżetu godzinowego projektu w Tempo.
* Przypisanie budżetu do epików lub milestone.
* Definiowanie alertów przy zbliżaniu się do limitu godzin.

---

## Jira – Tempo – raporty czasu: time spent, planned vs actual

* **Time Spent**: czas faktycznie zalogowany przez deweloperów.
* **Planned vs Actual**: porównanie szacowanego czasu tasków z rzeczywistym czasem logowania.
* Analiza odchyleń do kontroli przepalenia budżetu.

---

## Jira – Tempo – kontrola budżetu, forecast

* Monitorowanie wykorzystania godzin budżetowych względem postępu.
* Prognozowanie czy projekt zakończy się w ramach przydzielonego budżetu.
* Generowanie alertów dla PM przy przekroczeniu 80–90% budżetu.

---

## Estymacja – T-shirt estimation XS, S, M, L, XL

* Szybka metoda planowania dla PM i zespołu.
* Skala: XS=2h, S=4h, M=8h, L=16h, XL=24h.
* Duże taski (>24h) dzielone na mniejsze podtaski.

---

## Estymacja – estymacja godzinowa tasków

* Każdy task posiada **Original Estimate** (plan) w godzinach.
* Wlicza czas developmentu, code review, testów oraz bufor.
* Pozwala PM kontrolować przepalenie i planować sprinty.

---

## Estymacja – struktura estymacji

* **Development** – czas pracy dewelopera nad zadaniem.
* **Review** – czas potrzebny na code review.
* **Testing** – czas QA i testów automatycznych/manualnych.
* **Buffer** – dodatkowy czas na nieprzewidziane trudności.

---

## Estymacja – estymacja feature i agregacja tasków

* Feature rozbijane na taski i subtaski.
* Sumowanie wszystkich godzin tasków daje całkowity czas feature.
* PM dodaje procentowy bufor ryzyka (10–20%) do planowanej estymacji.

---

## Estymacja – capacity planning zespołu

* Obliczanie dostępnej liczby godzin w sprintach:

  ```
  Capacity = liczba dev × dni sprintu × godziny/dzień – meetings, review
  ```
* Pozwala dobrać ilość tasków do realnej wydajności zespołu.

---

## Estymacja – velocity zespołu

* Średnia liczba godzin faktycznie zrealizowanych w poprzednich sprintach.
* Używana do planowania kolejnych sprintów (max 90% velocity dla bezpieczeństwa).

---

## Sprinty – sprint planning

* Wybór tasków do sprintu zgodnie z capacity.
* Upewnienie się, że wszystkie taski mają estymaty, acceptance criteria i DoD.

---

## Sprinty – zarządzanie sprintem

* Codzienny monitoring statusów tasków.
* Usuwanie blokad i wspieranie deweloperów w progressie.
* Logowanie czasu przez zespół w Tempo.

---

## Sprinty – sprint review

* Spotkanie podsumowujące ukończone taski i postęp sprintu.
* Analiza wykresu burndown i odchyleń od planu.

---

## Sprinty – sprint retrospective

* Omówienie problemów sprintu, co zadziałało dobrze, co poprawić.
* Wprowadzenie usprawnień w workflow i estymacjach.

---

## Dashboard – konfiguracja w Jira

* Tworzenie dashboardu dla PM z widgetami:

  * Sprint burndown
  * Sprint velocity
  * Cumulative flow diagram
  * Issue statistics

---

## Dashboard – sprint burndown

* Wykres pokazujący pozostałą pracę vs idealną linię spadku w czasie sprintu.
* Wskazuje opóźnienia lub scope creep.

---

## Dashboard – sprint velocity

* Monitorowanie faktycznej liczby godzin zrealizowanych w sprintach.
* Porównanie planowanego vs faktycznego czasu, analiza odchyleń.

---

## Dashboard – cumulative flow diagram

* Wizualizacja przepływu tasków przez statusy.
* Pozwala wykryć wąskie gardła w procesie developmentu.

---

## Dashboard – issue statistics

* Liczba tasków w każdym statusie.
* Liczba opóźnionych tasków.
* Liczba blokad w backlogu lub sprintach.

