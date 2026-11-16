# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Wenn wir Verbrauchern mit offenen Forderungen, die eine Ratenvereinbarung benötigen, auf dem Affordability Screen erklären, warum wir ihr Einkommen abfragen, brechen weniger von ihnen die Ratenvereinbarung ab.
- **From M3, your primary success metric & guardrail metric:** Abbruchquote am Affordability Screen
- **From M4, the feature you scoped in your PRD this is what you're testing:** Erklärung der Einkommensabfrage auf dem Affordability Screen

Was: Ein kurzer, verständlicher Hinweistext direkt am Einkommensfeld, der erklärt, warum wir das Einkommen abfragen und wie die Angabe verwendet wird.

Für wen: Verbraucher mit offenen Forderungen, die eine Ratenvereinbarung benötigen (Pilot Deutschland).

Ziel: Weniger Abbrüche am Affordability Screen.

Erfolgsmaß: Abbruchquote am Affordability Screen [−Y Punkte].

Im Scope:

Hinweistext am Einkommensfeld (mobil und Desktop)
Tracking der Abbruchquote an diesem Screen

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Erklärung der Einkommensabfrage am Income Field des Affordability Screen (Hinweistext, mobil und Desktop).

Getestet wird: Ob diese Erklärung die Abbruchquote am Affordability Screen senkt.

Vergleich: Version mit Erklärung gegen Version ohne.
- **Persona pull your M2 persona:** Persona: Mara

Role: Verbraucherin mit einer oder zwei offenen Forderungen, die eine Ratenvereinbarung benötigt und dem Inkassounternehmen nicht zutraut, sie neutral zu beraten.

Goal: Eine Ratenvereinbarung abschließen, die sie sich leisten und einhalten kann, ohne anzurufen.

Friction: Am Affordability Screen soll sie ihr Einkommen angeben, ohne zu wissen, warum es abgefragt wird. Sie bricht ab, um Antworten woanders zu suchen, oder legt sich auf einen geschätzten Betrag fest.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** Expected outcome:

Mit der Erklärung zur Einkommensabfrage brechen weniger Verbraucher am Affordability Screen ab.

Messgröße: Abbruchquote am Affordability Screen [−Y Punkte] gegenüber der Version ohne Erklärung.

Guardrail: Keine Zunahme der Agent-Eskalationen.

Y ist offen: Nimm die heutige Abbruchquote als Baseline, oder schreibe “Baseline wird in den ersten vier Wochen gemessen”.
- **Primary success metric the one number that defines success, from M3:** Abbruchquote am Affordability Screen
- **Baseline rate today's rate of your primary metric, from your M3 data:** 20%
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Guardrail metric: Agent-Eskalationsquote
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** 2%
- **Sample size per arm use the calculator in the builder, baseline + MDE:** Sample size per arm: ca. 6.040 Nutzer
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** Kontrolle: Affordability Screen ohne Erklärung (6.040 Nutzer)
Variante: mit Erklärung zur Einkommensabfrage (6.040 Nutzer)

Zufällige Zuweisung pro Nutzer, nicht pro Session, damit niemand beide Versionen sieht.

Test duration:

Dauer = 12.100 Nutzer ÷ wöchentliche Nutzer am Affordability Screen
- **Significance threshold p < 0.05 is standard, explain any deviation:** α = 0,05

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** Der Affordability Screen ohne Erklärung. Der Verbraucher soll sein Einkommen angeben, ohne zu erfahren, warum es abgefragt wird.
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** Der Affordability Screen mit Erklärung zur Einkommensabfrage. Alles andere bleibt identisch zu Control (A).
- **Isolation check, what has NOT changed? list everything identical between arms (app version, eligibility rules, notifications, onboarding). If something changed inadvertently, your test is compromised.:** Isolation check: identisch in beiden Varianten

Einzige Änderung: der Hinweistext am Income Field. Alles andere bleibt gleich.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that an explanation of why income is requested at the Income Field of the Affordability Screen for Mara and consumers like her with open claims who need an instalment agreement will result in fewer consumers abandoning the Affordability Screen, as measured by a 2-percentage-point reduction (20 % → 18 %) in the abandonment rate at the Affordability Screen within [X Wochen, abhängig vom Wochenvolumen; ca. 12.100 Nutzer nötig]. We will protect the agent escalation rate (no increase beyond [+Z points]) throughout the test.
- **Your shipping criteria (filled in):** We will SHIP if the abandonment rate at the Affordability Screen improves by ≥ 2 percentage points (20 % → 18 %) at α = 0.05 (95 % significance) and the agent escalation rate does not reach [baseline + Z points] after 2 weeks.

We will ITERATE if direction is positive but lift is below the MDE.

We will KILL if the primary metric shows no improvement or moves negatively.

The read date is fixed at the end of 2 weeks, no results reviewed before this date.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** Hardest parameter: the MDE (2 percentage points).

Why it was hardest:

It isn’t a measurement, it’s a judgement call. It has to balance what is commercially worth shipping against what the traffic can actually detect.
It drives everything else: sample size (about 12,100 users), duration, and whether the test is feasible at all.
The 20 % baseline and the 2-point MDE are assumptions, not data. A different baseline would change the required sample size.
