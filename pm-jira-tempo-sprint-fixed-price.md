**PM projektu w Jira z użyciem Tempo Timesheets**

---

## 1. Struktura projektu

Hierarchia pracy:

* **Epic** – duży obszar funkcjonalny lub etap projektu
* **Story / Task** – konkretna funkcjonalność lub zadanie
* **Sub-task** – małe elementy implementacyjne

Przykład:

```
EPIC: System płatności

Story: Integracja Stripe
Task: Endpoint tworzenia płatności
Task: Webhook potwierdzenia
Task: Testy integracyjne
```

Zasada:
Task maksymalnie **1–2 dni pracy**. Jeśli większy → podział.

---

## 2. Milestones

Milestone = punkt kontrolny projektu.

W Jira realizuje się to przez:

* **Version / Release**
* **Sprint**

Struktura:

```
Version 1.0
  Sprint 1
  Sprint 2
  Sprint 3
```

Każdy milestone powinien zawierać:

* datę release
* scope (epiki)
* budżet godzin

---

## 3. Planowanie czasu

Każdy task ma:

* **Original Estimate** – plan godzin
* **Remaining Estimate** – ile zostało
* **Time Spent** – realny czas z Tempo

Przykład:

```
Task: API endpoint
Original Estimate: 6h
Time Spent: 4h
Remaining: 2h
```

---

## 4. Logowanie czasu w Tempo

Każdy developer:

* loguje **czas codziennie**
* przypisuje do **taska**
* opisuje krótko wykonane działania

Przykład:

```
4h – implementacja endpointu
2h – testy integracyjne
1h – code review
```

---

## 5. Liczenie przepalenia budżetu

Podstawowe metryki:

### Plan

```
Total Planned Hours = suma Original Estimate
```

### Wykonanie

```
Total Spent Hours = suma Time Spent
```

### Burn Rate

```
Burn Rate = Spent / Planned
```

Interpretacja:

| Burn Rate | Znaczenie               |
| --------- | ----------------------- |
| 0.8       | projekt poniżej budżetu |
| 1.0       | zgodnie z planem        |
| 1.2+      | przekroczenie           |

---

## 6. Burn-down sprintu

Sprint:

```
Sprint Budget = suma godzin tasków
```

Każdego dnia:

```
Remaining Work = Remaining Estimate
```

Wykres burn-down powinien:

* spadać liniowo
* jeśli rośnie → scope creep

---

## 7. Kontrola budżetu projektu

W Tempo Planner:

```
Budget = 1000h
Spent = 420h
Remaining = 580h
```

Kontrola:

```
Project Progress = Completed Story Points / Total Story Points
```

Porównanie:

```
Progress 30%
Budget used 60%
```

oznacza poważne przepalenie.

---

## 8. Workflow taska

Minimalny workflow:

```
Backlog
↓
Selected for Sprint
↓
In Progress
↓
Code Review
↓
Testing
↓
Done
```

Zasady:

* tylko 1 status aktywny
* developer zmienia status sam
* brak pracy bez taska

---

## 9. Weekly PM review

Co tydzień:

1. sprawdzenie **burn rate**
2. analiza **przekroczonych tasków**
3. aktualizacja **remaining estimate**
4. zamknięcie ukończonych zadań

Raport:

```
Tasks Done
Tasks Delayed
Budget Used
Risk
```

---

## 10. Najczęstsze błędy

1. Taski po **20–40h**
2. Brak **original estimate**
3. Czas logowany raz w tygodniu
4. Scope bez epików
5. Milestone bez budżetu

---

## 11. Minimalny setup Jira dla projektu

Boards:

```
Development board
PM board
```

Epics:

```
Backend
Frontend
Infrastructure
QA
```

Raporty:

* Sprint report
* Burn-down
* Tempo budget report

---

## 12. Wzór struktury projektu

```
Project

Epic: Auth System
  Task: Login endpoint
  Task: JWT generation
  Task: Password reset

Epic: Payments
  Task: Stripe integration
  Task: Webhook handling

Epic: Admin panel
  Task: User list
  Task: Role management
```

---

Jeśli potrzebne:

* **szablon projektu Jira dla software house**
* **model estymacji godzin dla zespołu dev (bardzo praktyczny)**
* **dashboard PM do kontroli przepaleń**.
