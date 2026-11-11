# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** Mara hat zwei offene Forderungen, arbeitet im Schichtdienst und nutzt das Portal in der Pause auf dem Handy.

Ziel: Sie will ihre Forderungen so begleichen, dass sie es sich leisten und einhalten kann, ohne anzurufen.
Problem: Beim Einkommensschritt weiß sie nicht, warum gefragt wird und was eine verpasste Zahlung bedeutet. Sie bricht ab oder rät einen Plan, den sie nicht halten kann.

Warum sie: Wer mehrere Forderungen hat, schließt nur zu 28–38 % ab (bei einer Forderung: 52 %).
- **Primary success metric (M3), your leading indicator:** Primäre Erfolgskennzahl: Anteil der Personen, die nach den Finanzfragen zum nächsten Schritt (Dokumente) weitergehen.

Heute: 80,7 % (5.943 von 7.364).
Ziel (Vorschlag): mindestens 83,7 % (+3 Punkte).
Warum diese: Sie misst genau die Stelle, an der Mara abbricht, und zeigt schon nach etwa 3 Wochen eine Veränderung.
- **Moment of misery (M2), the specific friction blocking the goal:** Moment of Misery: Mara öffnet das Portal in der Pause auf dem Handy, wird nach ihrem Einkommen gefragt und weiß nicht, ob “diesen Monat” oder “ein normaler Monat” gemeint ist. Sie schließt die Seite und will “später wiederkommen” (N-01).

Warum es blockiert: Ohne Erklärung weiß sie nicht, wofür die Angabe genutzt wird und was passiert, wenn sie sich irrt (N-06: “What if they use it against me?”).
Zahl dazu: 19,3 % verlassen das Portal bei den Finanzfragen (1.421 von 7.364).
- **Guardrail metric (M3), what must not drop or break:** Guardrail-Kennzahl: Quote gehaltener Pläne, also Vereinbarungen ohne verpasste Zahlung innerhalb von 60 Tagen.

Heute: 81,0 % (3.115 von 3.846).
Untergrenze (Vorschlag): 78 %.
Warum: In Monat 4 stiegen die Abschlüsse, aber mehr Pläne brachen ab (von etwa 84 % auf 81,6 % und dann 81,0 %). Mehr Abschlüsse zählen nur, wenn die Pläne halten.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** 1. B2: explainer for the income question.

Value 4, effort 1: it needs no new logic, only text.
Why it matters: it hits the exact point where people leave (N-01, N-06, T-206).
How you’d know: it is measured by the primary metric (80.7% today) and falls to the “why income” contacts.

2. B5: working mobile upload.

Value 4, effort 2: it is a technical fix for a known bug (T-201).
Why it matters: it removes the largest documented cause of the 22.1% loss at the document step.
Caveat: “skip the document under a set amount” needs a risk and compliance decision. Fix the upload first.

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** have not done it
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** no
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** no

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** B2, Erklärung zur Einkommensfrage: Value 5, Aufwand 1. Sie trifft genau die Stelle, an der Mara abbricht (19,3 %), und braucht nur Text.
B5, Foto-Upload am Handy: Value 3, Aufwand 2. Sie behebt 853 fehlgeschlagene Uploads (T-201). Der Fehler liegt aber im Schritt nach der Primärkennzahl, deshalb steht B5 jetzt bei “Fill-In”. In meiner ersten Bewertung hatte B5 Value 4 und zählte als Quick Win.
- **What I cut, and the “no” I’m protecting the scope from:** Cut for now

B1, one plan for several claims: a major project, so it doesn’t fit 8 weeks. It is the next step after the pilot.
B3, affordability check: a major project too. It could also add questions that lower the primary metric.
B4, agent handoff summary: it helps Daniel, not Mara, and doesn’t move the primary metric.
B6, pay-day payment date: the link to broken plans is only plausible.

The “no” I’m protecting the scope from

B7, shortest plan first: it is cheap and promises more recovery, which makes it tempting. But it repeats the Month 4 change, after which broken plans rose from 15.6% to 18.4%. It would put the guardrail (plan-kept 81.0%, floor 78%) at risk.
B8, chat on every page: chat users miss more payments (21.6% vs 18.3%), and the chat doesn’t show the consequences (T-208). It would spread the problem instead of fixing it.
- **Prototype/roadmap screenshot link (paste into your deliverables):** bu_collection_roadmap.html
