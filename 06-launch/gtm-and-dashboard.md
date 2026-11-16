# GTM Strategy & Success Dashboard (Module 6)

## Get your prior work ready
- **The feature you're launching from your M4 PRD, one feature, not a list:** Feature: Explanation of why income is requested, shown at the Income Field of the Affordability Screen.
- **What your M5 experiment will test your hypothesis, primary metric and ship / iterate rule, the evidence the launch rests on:** Experiment (M5, kurz):

Hypothese: Erklären wir am Income Field des Affordability Screen, warum das Einkommen abgefragt wird, brechen weniger Verbraucher mit Ratenbedarf dort ab.

Primärmetrik: Abbruchquote am Affordability Screen, 20 % → 18 % (MDE 2 Punkte), α = 0,05, ca. 6.050 Nutzer pro Variante.

Guardrail: Agent-Eskalationsquote darf [Baseline + Z] nicht erreichen.

Regel (Read Date nach 2 Wochen):

Ship: ≥ 2 Punkte Verbesserung bei α = 0,05, Guardrail hält
Iterate: positiv, aber unter 2 Punkten
Kill: keine Verbesserung oder Verschlechterung

Evidenz: Problem Hook und Moment of Misery (M1/M2). Die 20 % sind eine Annahme, ein Interviewzitat oder Funnel-Daten fehlen noch.
- **Your persona pull your M2 persona, this anchors your audience:** Persona (M2): Mara

Rolle: Verbraucherin mit einer oder zwei offenen Forderungen, die eine Ratenvereinbarung benötigt und dem Inkassounternehmen nicht zutraut, sie neutral zu beraten.

Ziel: Eine Ratenvereinbarung abschließen, die sie sich leisten und einhalten kann, ohne anzurufen.

Friction: Am Affordability Screen soll sie ihr Einkommen angeben, ohne zu wissen, warum es abgefragt wird. Sie bricht ab, um Antworten woanders zu suchen, oder legt sich auf einen geschätzten Betrag fest.

Audience im Test: Mara steht stellvertretend für Verbraucher mit offenen Forderungen, die eine Ratenvereinbarung benötigen (Pilot Deutschland).

## Set your goal, then your audience
- **Primary GTM goal awareness · engagement · conversion, pick one:** Primary GTM goal: Conversion

Mehr Verbraucher, die den Affordability Screen abschließen und einen Ratenplan erreichen.
- **Why this goal? what makes this the right goal for this feature right now:** Warum Conversion:

Das Feature wirkt an einem Schritt im Funnel. Die Erklärung am Income Field soll Nutzer durch den Affordability Screen bringen, nicht mehr Nutzer ins Portal holen (Awareness) oder länger dort halten (Engagement).
Die Primärmetrik ist eine Conversion-Metrik. Die Abbruchquote ist das Gegenstück zur Abschlussquote an diesem Schritt.
Der Business-Case hängt am Abschluss. Laut Problem Hook geht Geld verloren, wenn Verbraucher abbrechen oder Pläne abschließen, die sie nicht halten. Reichweite und Interaktion lösen das nicht.
Die Funnel-Daten stützen es. Es gibt bereits 8.360 Nutzer pro Monat im Journey. Das Problem ist nicht, sie zu erreichen, sondern sie zum Abschluss zu bringen.
- **Target audience the specific segment your goal implies, be precise:** arget audience (präzise):

Verbraucher in Deutschland (Pilot) mit mindestens einer offenen Forderung, die im Portal einen Ratenplan-Journey starten und den Affordability Screen erreichen.

Ein- und Ausschluss:

Eingeschlossen: Einzel- und Mehrfachforderungen, mobil und Desktop
Ausgeschlossen: Verbraucher, die den Screen nie erreichen, andere Märkte, Fälle, die direkt beim Agenten starten

Größe aus deiner Datei:

Obergrenze 8.360 Nutzer pro Monat im Ratenplan-Journey
davon 2.968 mit zwei oder mehr Forderungen und 6.563 mobil

## Size your launch
- **Launch tier S (minimal) · M (targeted) · L (multi-channel) · XL (full GTM):** _(not filled in)_
- **Justification reach + revenue impact + what silence would risk:** _(not filled in)_
- **Is this a launch or a release? does it need go-to-market, or can it just ship?:** _(not filled in)_

## Choose your top three channels and plan assets
- **Channel 1 owned / earned / paid, and why it reaches your audience:** Im Portal selbst (Hinweistext am Income Field)
- **Channel 2 owned / earned / paid, and why:** E-Mail oder SMS an Abbrecher.
- **Channel 3 owned / earned / paid, and why:** Briefing der Agenten
- **Enablement & assets what Sales / CS / Support need, plus the assets to build (one-pager, demo, etc.):** Enablement & Assets (Zusammenfassung)

Portal: rechtlich geprüfter Hinweistext (DE, mobil und Desktop), Design-Spec und Tracking-Plan für beide Varianten.
E-Mail/SMS an Abbrecher: Nachrichtentext mit Link zurück in den Journey und Versandregeln inklusive Datenschutz. Start erst nach dem Read Date.
Agenten: Einseitiger Leitfaden mit Standardantwort auf “Warum fragen Sie nach meinem Einkommen?”.
Intern: One-Pager für Product, Operations, UX, QA und Development sowie Release-Freeze für den Screen während des Tests.

## Make it executable
- **Ownership named owner per key activity, individual, not department:** Aktivität	Owner
Gesamtverantwortung Experiment, Ship/Iterate/Kill-Entscheidung	Du (Product)
Hinweistext schreiben	[Name], UX Writing oder Content
Rechtliche und Compliance-Prüfung des Textes	[Name], Legal/Compliance
Design-Spec und Umsetzung im Portal	[Name], UX und [Name], Development
Tracking und Auswertung (Abbruchquote, Guardrail)	[Name], Data/Analytics
QA und Variantenzuweisung (50/50)	[Name], QA
Release-Freeze und Isolation	[Name], Development Lead
Agenten-Leitfaden und Briefing	[Name], Operations
E-Mail/SMS an Abbrecher (nach Read Date)	[Name], Marketing/CRM
Intern-One-Pager an Stakeholder	Du (Product)
- **Budget & resource gaps what costs extra, and any asset you can't currently build:** sms can cost extra
- **Timeline Phase 1 beta → Phase 2 launch moment → Phase 3 post-launch:** imeline (relative Wochen, ich kenne euer Startdatum nicht)

Phase 1: Beta (Experiment)

Woche 0: Text, Legal-Freigabe, Tracking und Release-Freeze stehen. Baseline bestätigt.
Woche 1-2: A/B-Test läuft (50/50), keine Zwischenauswertung.
Ende Woche 2: Read Date, Entscheidung Ship / Iterate / Kill.
Hinweis: Bei ca. 1.930 Nutzern pro Woche brauchst du für 12.100 Nutzer rund 6 bis 7 Wochen. Bei 2 Wochen gilt der größere MDE (ca. 4 Punkte).

Phase 2: Launch Moment (nur bei Ship)

Woche 3: Erklärung für 100 % der Nutzer im Portal ausgerollt.
Woche 3: Agenten-Leitfaden und Briefing live.
Woche 3-4: E-Mail/SMS an Abbrecher startet, Intern-One-Pager an Stakeholder.

Phase 3: Post-Launch

Woche 4-8: Abbruchquote und Eskalationsquote wöchentlich beobachten.
Woche 8: Plan-Kept-Rate lesen (erste Pläne sind dann fällig) und prüfen, ob der Effekt hält.
Danach: Nächster Test, etwa Selbsteingabe des Betrags oder Erklärung zu verpassten Raten.

## Define how you'll know it worked
- **Success metrics 2 to 3 metrics that match your GTM goal:** Success Metrics (passend zum Ziel Conversion)

Abschlussquote am Affordability Screen (Primär): Anteil der Nutzer, die den Screen abschließen. Gegenstück zur Abbruchquote, Ziel 80 % → 82 % (MDE 2 Punkte, Annahme).
Plan-Kept-Rate (Qualität): Anteil der Pläne, bei denen alle Raten im definierten Zeitraum (z. B. 90 Tage) gezahlt werden. Sie verhindert, dass Conversion nur Pläne zählt, die später scheitern.
Agent-Eskalationsquote (Guardrail): Darf nicht steigen. Sonst sinkt der Abbruch nur, weil schwierige Fälle beim Agenten landen.
- **Bad signal to watch for e.g. high reach, zero signups = message-market mismatch:** Bad Signal: Mehr Abschlüsse am Affordability Screen, aber die Plan-Kept-Rate fällt oder die Eskalationen steigen.

Bedeutung: Die Erklärung bringt Nutzer durch den Screen, aber zu Plänen, die sie nicht halten können, oder zu Fällen, die später beim Agenten landen. Die Conversion ist nur scheinbar, wie beim SSR-Problem aus deinem Hook.

Weitere Warnzeichen:

Abbruchquote unverändert trotz Erklärung: Der Grund für den Abbruch war nicht fehlende Erklärung (Nachrichten-Markt-Mismatch).
Abbruch sinkt nur auf Mobil oder nur auf Desktop: Layout-Problem statt Textproblem.

Reaktion: Bei fallender Plan-Kept-Rate oder steigenden Eskalationen gilt der Test nicht als bestanden, auch wenn die Abbruchquote sinkt.
- **Most likely post-launch decision double-down · iterate · pivot · deprioritize, and what would trigger it:** _(not filled in)_
