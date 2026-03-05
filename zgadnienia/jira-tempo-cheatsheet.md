## Szablon projektu w Jira dla software house (model **Fixed Price + Sprinty**)

### Struktura projektu

```
Project

Version (Release)
    Milestone 1
    Milestone 2
    Milestone 3

Epics
    Backend
    Frontend
    Infrastructure
    QA

Sprinty
    Sprint 1
    Sprint 2
    Sprint 3
```

### Powiązanie fixed price z zakresem

```
Contract

Budget hours: 1200h
Budget money: 120 000 PLN

Milestone 1
    Budget: 300h

Milestone 2
    Budget: 400h

Milestone 3
    Budget: 500h
```

Sprint działa jako **narzędzie delivery**, nie rozliczenie finansowe.

---

### Struktura backlogu

```
Epic: Authentication

Story: Login API
    Task: Endpoint login
    Task: JWT generation
    Task: Error handling

Story: Password reset
    Task: Email flow
    Task: Token verification
```

---

### Sprint template

Sprint długość:

```
2 tygodnie
```

Sprint capacity:

```
Team size: 5 dev
8h/day
10 days

Capacity = 5 × 8 × 10 = 400h
```

Realna capacity:

```
400h
– meetings
– code review
– support

Real capacity ≈ 320h
```

---

### Sprint planning

Do sprintu trafia tylko:

```
Task z estimate
Task z opisem
Task z acceptance criteria
```

---

### Definition of Done

```
Code
Tests
Code review
Deploy na staging
QA verified
```

---

# Model estymacji godzin dla zespołu dev

Model oparty o **3 poziomy estymacji**.

---

## 1. T-shirt estimation (szybkie planowanie)

```
XS = 2h
S  = 4h
M  = 8h
L  = 16h
XL = 24h
```

Nie wolno tworzyć tasków > 24h.

---

## 2. Estymacja developerska

Każdy task ma:

```
Dev time
Review
Testing
Buffer
```

Przykład:

```
Feature: Payment webhook

Development: 6h
Code review: 1h
Testing: 2h
Buffer: 1h

Total: 10h
```

---

## 3. Estymacja projektowa (PM)

PM dodaje **risk buffer**.

```
Team estimate: 100h

+ 20% risk

Project estimate: 120h
```

---

## Wzór estymacji feature

```
Feature: User profile

Backend
    endpoint profile 6h
    validation 4h

Frontend
    UI 8h
    API integration 4h

Testing
    QA 6h

Total
    28h

PM buffer
    35h
```

---

## Velocity zespołu

Po 3 sprintach liczona jest średnia.

```
Sprint 1 = 300h
Sprint 2 = 280h
Sprint 3 = 310h

Velocity = 296h
```

Sprint planning:

```
Max load ≈ 90% velocity
```

---

# Dashboard PM w Jira + Tempo Timesheets

Dashboard składa się z 5 bloków.

---

## 1. Budget burn

Źródło: Tempo

```
Budget hours
Spent hours
Remaining
```

Przykład:

```
Budget: 1200h
Spent: 460h
Remaining: 740h
```

---

## 2. Burn rate

```
Burn rate = spent / planned progress
```

Przykład:

```
Progress: 30%
Budget used: 50%
```

Wniosek:

```
przepalenie
```

---

## 3. Sprint health

Widgety:

```
Sprint burndown
Sprint velocity
Open tasks
Blocked tasks
```

---

## 4. Delivery progress

```
Epics progress
Stories done / total
Milestone completion
```

Przykład:

```
Milestone 1
70% done
```

---

## 5. Risk panel

Filtry:

```
Tasks > 16h
Tasks overdue
Tasks blocked
Tasks without estimate
```

---

# Minimalny zestaw raportów PM

Raport tygodniowy:

```
Scope
Progress
Budget
Risks
Next sprint
```

---

# Najważniejsze zasady fixed-price

1. Scope kontrolowany przez **epiki**
2. Każdy task ma **estimate**
3. Czas logowany codziennie w **Tempo**
4. Sprint capacity ≤ 90% velocity
5. Milestone ma **budżet godzin**

---

# Przykładowa struktura realnego projektu

```
Project

Release 1.0

Milestone 1 – Authentication
    Epic Auth
        Login API
        Registration
        Password reset

Milestone 2 – Payments
    Epic Payments
        Stripe integration
        Subscription logic
        Webhooks

Milestone 3 – Admin
    Epic Admin
        User list
        Roles
        Billing panel
```

---

Rozwinięcie, które znacząco zwiększa kontrolę projektu:

* **system wykrywania przepalenia budżetu przed sprintem**
* **matematyczny model estymacji dla software house (bardzo używany w dużych firmach)**
* **model wyceny fixed price żeby nie tracić marży**.
