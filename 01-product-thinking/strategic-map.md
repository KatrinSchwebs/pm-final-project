# Strategic Discovery Map (Module 1)

## Responses
- **Write one feature from the map that, if an engineer asked “why is this a priority for our 12-week roadmap?”, you honestly could not give a strategic answer for.:** Strategische Begründung: Dispute-Status-Tracking

Ich habe das Feature vorher zu eng gesehen. Der stärkste Grund liegt in den Mehrfachforderungen, die der Pilot ausdrücklich abdeckt.

1. Ein offener Dispute blockiert den Ratenplan
Mara hat zwei offene Forderungen. Wenn sie eine davon bestreitet, hängt die Ratenplan-Journey vom Status dieses Disputes ab. Kann sie ihn nicht sehen, weiß sie nicht, ob die bestrittene Forderung in den Plan gehört, ob sie während der Prüfung weiter gemahnt wird und ob ein Plan ihre Position verschlechtert. Das ist genau die Unsicherheit (“Kann die Annahme eines Angebots alles schlimmer machen?”), die laut Briefing zum Anruf führt. Der Dispute-Status ist also eine Voraussetzung dafür, dass der Ratenplan im Mehrfachforderungsfall funktioniert, und kein Nebenpfad.

2. Es schützt die North-Star-Metrik
Die SSR zählt nur Fälle ohne eingehenden Kontakt 30 Tage vor und nach der Lösung. “Wo steht mein Widerspruch?” ist ein typischer vermeidbarer Anruf. Jeder davon macht einen Fall für die SSR unzählbar, obwohl er sonst sauber gelaufen wäre. Das Feature wirkt damit weniger auf die Zahl selbst als auf ihre Qualität: Es verhindert, dass die SSR nur durch Fälle steigt, die den schwierigen Disputes ausweichen.

3. Fairness und Reputation beim Client
Der Leitplanken-Punkt zur Fairness verlangt, dass Verbraucher nicht im Dunkeln gelassen werden. Ein Widerspruch ohne sichtbare Antwort wirkt wie Ignorieren, und das trifft die Reputation des Clients, in dessen Namen wir inkassieren. Transparentes Reporting an Clients wird ebenfalls einfacher, wenn der Status strukturiert vorliegt und nicht nur in Agentennotizen.

4. Entlastung für Daniel
Daniel will Kommunikationshistorie und eine klare Zusammenfassung. Ein strukturierter Dispute-Status liefert beides und beseitigt die Rückfragen, ob schon ein Widerspruch läuft.

Minimaler Umfang für 12 Wochen

Vier Statusstufen: eingegangen, in Prüfung, entschieden, Folgeschritt.
Status wird aus dem bestehenden Case-Management gelesen, keine Neuentwicklung des Backends.
Benachrichtigung über die vorhandenen digitalen Kanäle.
Im Ratenplan: bestrittene Forderung klar kennzeichnen und separat behandeln.
Nicht gebaut: Live-Chat zum Dispute, Dokumentennachforderung im Portal, Statusdetails pro Prüfschritt des Clients.

Woran wir den Erfolg messen

Anteil der Kontakte mit Grund “Dispute-Status” (Baseline vor Pilotstart erheben).
Abbruchrate der Ratenplan-Journey bei Mehrfachforderungen mit offenem Dispute.
SSR, getrennt nach Fällen mit und ohne Dispute.

Stopp-Kriterium: Steigen die Kontakte zum Dispute-Status trotz Tracking oder zeigt das Backend den Status häufig falsch an, pausieren wir die Anzeige und gehen zurück zur reinen Bestätigung.

Was stimmen muss, damit das trägt
Diese Begründung gilt nur, wenn das Case-Management den Dispute-Status zuverlässig und aktuell liefert. Das habe ich nicht geprüft. Ich würde es in Woche 1 klären, bevor wir das Feature zusagen. Außerdem fehlen mir Zahlen, wie häufig Disputes im Pilotsegment überhaupt vorkommen. Ist der Anteil klein, bleibt die Priorität bei der Ratenplan-Erklärung.
- **Write one feature that looks “correct” for the app but has zero strategic weight, you have no idea if it helps the company make money or whether a single user actually asked for it.:** Feature: Visual case timeline (Understand branch)

What it would be: A scrollable timeline in the portal that shows every event in a case in order: claim received, letter sent, reminder opened, partial payment, dispute filed. Each event gets an icon, a date and a short label.

Why it looks correct: It fits the “understand my case” journey. It is easy to demo and gives the portal a polished feel. Any reviewer would say “yes, consumers should see their history.” It also sounds like it supports the north star, because a consumer who understands their case should not need to call.

What I can’t answer:

Did anyone ask for it? Nothing in the brief says so. Mara’s open questions are whether a plan would be affordable, why we ask about her income, what happens if she misses a payment, and whether both claims can be handled together. None of those is “show me my history.” I’d be guessing that a timeline answers her real question.
Does it make money? I can’t connect it to recovery rate, plan completion or cost per case. A consumer can read a perfect timeline and still not pay or still call.
Does it reduce agent work? Daniel wants a summary of what the consumer entered and why a case was escalated. A consumer-facing timeline doesn’t give him that.
Is it affordable to build? A reliable timeline needs clean event data from letters, digital reminders, payments and the case-management backend. Where that data is incomplete, the timeline will be wrong, and a wrong history creates more calls and distrust.

Honest verdict: It earns its place on a mindmap because it feels complete, but it has no strategic weight. If an engineer asked why it’s in the 12-week roadmap, my only answer would be “a case view should have one,” and that is a reason of form, not of value.

What would give it weight: Contact-reason data showing that a large share of calls ask “what has happened on my case?”, or a client requirement for transparent history. Without that, I’d replace it with a plain “what you owe and what happens next” summary, which answers Mara’s actual questions at a fraction of the cost.
- **Compare V3 to your Step 1 baseline. What changed, and is the output objectively better, did the AI get smarter, or did your added PM knowledge (JTBD, effort/impact, retention) force it to be useful?:** it changed but that much better. Time to short to properly iterate
- **Key takeaway: how does this prove the PM’s role is to think while the AI’s role is to execute?:** yes it does but you still have to think
