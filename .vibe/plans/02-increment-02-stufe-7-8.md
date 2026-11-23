---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Written by `lernapps plan` and the hooks. Never change a key or a value by hand.
# Archetype, as in the app's first plan. Allowed values: explainer, interactive, quiz.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit.
phase: commit
# prePushFailures: failed pre-push runs of this increment, written by the hook.
prePushFailures: 0
# failedChecks: failed rules and runs, written by lernapps check and the hooks.
failedChecks: { checks-pass: 11, explainer-readable-without-js: 2 }
---

# Increment: increment-02-stufe-7-8

<!--
For you, the assistant. One increment of a published app: new competencies, chapters, pages, rounds, questions, or a
correction. The process is in AGENTS.md; this plan holds the method.
- `npx --no -- lernapps plan next` prints the task to do now, `plan done` ticks it and prints the next one.
- You write only below Goal, Key decisions, Notes, Answers, Content method and Retrospective, in the creator's
  language. Delete the comment of a section once the section is filled.
- The first version's decisions stand: archetype, content method, content guide. Never change an earlier plan.
- Work on the branch `increment/<NN>-<short name>`. Until Commit everything is local: push nothing.
-->

*Started 2026-11-22. Explore, Plan, Code, Commit.*

## Goal

Jugendliche der Klasse 7-8 können Relativsätze genauer bilden (ohne Relativpronomen, mit Kommas), Gegensätze und Absichten mit although, while, whereas und so that ausdrücken, mit if über Unwirkliches und Vergangenes und mit I wish über Wünsche sprechen, und wiedergeben, was jemand gesagt oder verlangt hat. Jede Seite hat ein Lesestück (Chat, Tagebuch, Blog, kurzer Artikel) als Kern.

## Key decisions

- Kapitel 2 „Relativsätze genauer“ (3 Seiten), Kapitel 3 „Was wäre, wenn …?“ (3 Seiten), Kapitel 4 „Weitersagen, was jemand sagt“ (3 Seiten); Kapitel 5 (9-10) kommt später (Auftrag der Orchestrator-Session in der Rolle der Ersteller:in).
- Das Muster der ersten Version bleibt: Satzstreifen-Wand, Verbindungskarten, Weiche, Poster-Tabellen, Szene mit Figuren; Sophie ist jetzt 13 bis 14 und bleibt in England; Form der Geschichte: Chats, Nachrichten, Tagebuch, kurze Artikel; ein Bild nur, wo es etwas zeigt (Konventionen 2 und 8).
- Jede Seite hat ein Lesestück von etwa 150 bis 300 Wörtern als Kern (Vorwissen-Frage, Text in Abschnitten mit Randglossar, Aufgaben in drei Stufen: Verstehen, Belegen mit Zeile, Meinung; zuletzt Schreib- oder Sprechauftrag); es zählt nicht zu den 350 Wörtern Erklärtext (Konventionen 8).
- Lesestücke sind eigene Texte (der Normalfall), nach Fakten, keine Sätze aus fremden Texten; erfundene Schule und Personen, keine echten Menschen (guess). Kein VOA-, Wikinews- oder African-Storybook-Text, weil jeder Text die Figuren und das Thema der Seite braucht (guess).
- Neue Karten: Kontaktkarte (Relativkarte darf fehlen), Klammer aus Kommas (nicht notwendiger Streifen), although/whereas/while/so that, Weichen für unwirklich jetzt und früher, Wunschkarte I wish, Sprechblase wird Streifen mit said that, Zeitstrahl rückt nach links (Konventionen 2, Issue 481).
- Wiederholungsseiten `das-brauchst-du` je Kapitel (kompakt, ohne Übung) für Bausteine anderer Explainer oder nicht praktizierte: simple-past (K3), past-perfect (K3 und K4), infinitivkonstruktionen und imperativ (K4) (guess: je Kapitel eine Sammel-Wiederholung).
- Inkrement nach dem Muster der ersten Version; keine Komponenten.

## Notes

- Strang `englisch/grammatik`, Karte `https://lernapps.net/apps/map/englisch.json` (am 2026-11-21 geöffnet), alle neun Bausteine Lücken (`practisedBy` leer), Band 7-8:
  - Kapitel 2 `relativsaetze-2` „Relativsätze genauer“: `contact-clauses` (Schritt 1, braucht relativsaetze): Ich kann Relativsätze ohne Relativpronomen bilden, wenn das Pronomen Objekt ist (the book I read). `relativsaetze-nicht-notwendig` (Schritt 1, braucht relativsaetze, öffnet 2): Ich kann nicht notwendige Relativsätze mit Kommas bilden und von notwendigen unterscheiden. `konjunktionen-although` (Schritt 1, braucht konjunktionen, öffnet 1): Ich kann Gegensätze und Absichten mit although, while, whereas und so that ausdrücken.
  - Kapitel 3 `was-waere-wenn` „Was wäre, wenn …?“: `if-satz-2` (Schritt 1, braucht if-satz-1 und simple-past, öffnet 2): Typ 2 (If I had more time, I would …). `if-satz-3` (Schritt 2, braucht if-satz-2 und past-perfect): Typ 3 (If you had asked me, I would have helped.). `i-wish` (Schritt 2, braucht if-satz-2): Ich kann mit „I wish …“ und „If only …“ Wünsche und Bedauern ausdrücken.
  - Kapitel 4 `weitersagen` „Weitersagen, was jemand sagt“: `reported-speech` (Schritt 1, braucht that-saetze und personalpronomen, öffnet 3): ohne Zeitverschiebung. `backshift` (Schritt 2, braucht reported-speech und past-perfect, öffnet 1): mit Zeitverschiebung. `indirekte-aufforderungen` (Schritt 2, braucht reported-speech, infinitivkonstruktionen und imperativ): She told me to wait.
- Didaktik je Baustein (Satzstreifen tragen weiter; jede Seite hat ein Lesestück als Kern):
  - contact-clauses: Die Relativkarte who/which/that darf fehlen, wenn sie Objekt ist (the book (that) I read, the girl (who) I met); Kinder sehen am Streifen, ob das Pronomen Subjekt (darf nicht fehlen) oder Objekt (darf fehlen) ist. Lesestück: Chat von Sophie und Amir über Bücher, Filme und Leute. Irrtum: Relativkarte weglassen, wenn sie Subjekt ist („the girl lives here“).
  - relativsaetze-nicht-notwendig: Nicht notwendige Streifen stehen in Klammern aus Kommas und lassen sich herausnehmen; notwendige nicht. Lesestück: Tagebucheintrag (Sophie über ihre Lehrerin, ihre Gastfamilie). Irrtum: Kommas fehlen oder that in nicht notwendigen Streifen.
  - konjunktionen-although: although, while, whereas (Gegensatz) und so that (Absicht) als neue Verbindungskarten. Lesestück: kurzer Zeitungsartikel der Schulzeitung. Irrtum: although mit but im selben Satz, so that mit so; Gegensatz mit because.
  - if-satz-2: Weiche „unwirklich jetzt“: if + simple past, would + Verb; Zeitstrahl rückt nach links. Lesestück: Chat „Was würdest du tun, wenn …“. Irrtum: would im if-Streifen, simple present statt past, if I was/were.
  - if-satz-3: Weiche „unwirklich früher“: if + past perfect, would have + 3. Form. Lesestück: Geschichtenauszug oder Blog über eine verpasste Chance (Bus verpasst). Irrtum: would im if-Streifen, simple past statt past perfect.
  - i-wish: I wish/If only + simple past (jetzt), + past perfect (früher), + would (Ärger über andere). Lesestück: Blog-Eintrag. Irrtum: I wish + present oder will.
  - reported-speech: Aus einer Sprechblase wird ein Streifen mit said that; Pronomen wechseln (I → she), Orts- und Zeitwörter (here → there); ohne Zeitverschiebung, wenn das Sagen noch gilt oder says. Lesestück: Chat mit Nachrichten und Bericht. Irrtum: Pronomen bleibt, Anführungszeichen.
  - backshift: Das Sagen ist vorbei → Zeitstrahl rückt einen Schritt nach links (am/is → was, will → would, present perfect → past perfect). Lesestück: Interview in der Schulzeitung und Bericht. Irrtum: Zeit nicht verschoben, tomorrow nicht geändert.
  - indirekte-aufforderungen: told/asked + Person + (not) to + Verb. Lesestück: Dialog oder Chat mit Bitten. Irrtum: told me that, ohne to, don't statt not to.
- Musterseite `contact-clauses` (2026-11-22): Lerner-Check mit Sub-Agent (Klasse 7/8, 360 und 1280 px) und Sprachprüfung Englisch/Deutsch mit Sub-Agent. Behoben: Chat natürlicher (Kurzformen, Bezug in Nachricht 7, 8, 9, 10, 11), stimmige Beleg-Aufgabe (Snacks statt Buch), Merke und Beispiele ohne Lösungen, Diktat ohne Satz der Seite und ohne einsetzbares that, Perfekt-Varianten in Übersetzungen, Randglossar mit copy, chose, for the part, Same!, Subjekt/Objekt erklärt, Lese-Auftrag vor dem Chat, Hinweise je Aufgabe, Hörliste im Inhaltsführer. Offen: Vorlagenfehler wie in der ersten Version.
- Gesamtcheck der neuen Seiten (2026-11-22): drei Lerner-Checks mit Sub-Agenten (je ein Kapitel, Kind Klasse 7/8, 360 und 1280 px) und zwei Sprachprüfungen Englisch/Deutsch (Kapitel 2 und 3, Kapitel 4). Behoben (je Kapitel ein Korrektur-Agent): Mr Hill nicht mehr als „neuer Lehrer“ (Konventionen: keine neue Figur); Regel und Geschichte stimmen überein (reported-speech: das Gesagte gilt noch, backshift: das Sagen ist vorbei); Kommaregel bei although, while, whereas und in den nicht notwendigen Relativsätzen einheitlich, Diktat prüft die Kommas; gültige Varianten statt Fehler (Kurzformen he’d und we’d, to not, Satzumstellung, wish mit didn’t, past perfect in if-Sätzen); Beispiele und Hörsätze ohne Widersprüche (Peters Hund, Amirs Bruder und Handy); Wiederholungsseiten ohne rohe Ids und ohne Entwicklertext; Randglossar vollständig; Weiter-Abschnitte kurz; Richtige Option in Einzelauswahl nicht mehr immer an erster Stelle (alle Seiten); Textmenge unter 350 Wörtern, keine Hinweise des Checks. Offen (Vorlage): Die Wiederholungsseiten (`recap`) zeigen die Karten-Ids als Linktext (`englisch/past-perfect`), das erzeugt die Vorlage selbst; weitere Vorlagenfehler wie in der ersten Version.
- Umfang: in: die neun Bausteine in drei Kapiteln, je ein Lesestück. Out: Kapitel 5 (indirekte Fragen, satzbezogenes which, cleft sentences, Partizipialsätze, -ing-Formen); mixed conditionals, Inversion in if-Sätzen; Relativsätze mit Präposition. Sprache: Deutsch erklärt, britisches Englisch.
- Voraussetzungen von außen: simple-past (#472 Kapitel 2, gebaut), past-perfect (#472 Stufe 7-8, Inkrement), infinitivkonstruktionen (#480 Stufe 7-8, Inkrement), imperativ (5-6, #470/#480); sie bekommen je Kapitel eine Sammel-Wiederholung (`recap`) oder, wo die Voraussetzung auf der Seite im Chat vorkommt, einen Link (Plan-Phase prüft mit `lernapps check`).
- Quellen, am 2026-11-22 geöffnet (nur Fakten, CC BY-SA, keine Sätze): Wikipedia „English relative clauses“ (that kann weggelassen werden, wenn es nicht Subjekt ist; Zero relative pronoun; nicht notwendige Relativsätze mit Kommas), „English conditional sentences“ (conditional I, II, III), „Reported speech“ (Backshift ist nicht verpflichtend, wenn die Aussage noch gilt), „Subjunctive“ (wishes, conditional clauses), „Conjunction“ (although, whereas, so that als unterordnende Konjunktionen). Lizenz: Wikipedia CC BY-SA 4.0; wir übernehmen keine Sätze. Texte der Seiten sind eigene Lesestücke. Nicht geprüft: Simple English Wikipedia, VOA, Wikinews, African Storybook (nicht benutzt).

## Explore

<!--
- All content questions belong here; Plan maps the answers onto the app. Ask; write no code.
- Skip what earlier answers or the app already tell. At most 2 questions per message, one topic each.
-->

### Tasks

- [x] Read the README of the archetype's template (its path is in skill `lernapps-app`): what the app can do now.
      Tell the creator what is new, if it matters for this increment.
- [x] Load the content guide `.agents/skills/app-content/SKILL.md` and read the earlier plans in `.vibe/plans/`: what
      the app teaches, how its content is made, what is open.
- [x] Interview, one topic per question, the creator's words under "Answers": which competencies, chapters or rounds,
      for which school years; hurdles and examples; the amount; any change of look and feel or of terms. No answer:
      ask once more, then write your assumption with "(guess)".
- [x] Load skill `lernapps-content-research`. Research what the content guide does not cover. Write under "Notes":
      the new competencies by chapter with their ids, the sources you opened.
- [x] Write under "Notes" the didactic approach per competency and the scope (in, out, data range).
- [x] The increment needs a kind of content the guide does not cover (a new page structure, screen, component or kind
      of exercise): load skills `lernapps-explainer-design` and `lernapps-exercise-patterns`. Else skip this task.
- [x] **Checkpoint:** research. Show in plain words: the new competencies by chapter, the didactic approach, the
      scope, every "(guess)", the sources and what is unchecked. Stop and wait. Changes: change them, then ask again.
      Creator: Ja, die neun Seiten mit je einem Lesestück passen, und Sub-Agenten dürfen die drei Kapitel parallel schreiben, nachdem die Musterseite (contact-clauses) steht. Recaps für past-perfect und infinitivkonstruktionen nur kompakt und mit Link zur Karte. Push von increment/02-stufe-7-8 und zweiter Vorschau-PR muss die Ersteller:in erlauben; bis dahin lokal.

### Answers

- Umfang und Stufe: „Baue die Kapitel 2 „Relativsätze genauer“, 3 „Was wäre, wenn …?“ und 4 „Weitersagen, was jemand sagt“ (Stufe 7-8) als Inkrement in dasselbe Repository; Kapitel 5 (9-10) kommt später.“
- Form: „Lesestücke als Kern der Seite, Eigentexte nach Quellen, Figuren 13 bis 14“ (Konventionen Abschnitt 8); „Seiten nach dem Muster der ersten Version (Satzstreifen-Wand), mit den Regeln aus Abschnitt 7.“
- Veröffentlichen: „Vorschau-Pull-Request offen lassen, nichts nach `main`, kein Katalogeintrag.“
- Hürden: aus dem Issue (`issues/481.md`) und den Konventionen; keine weiteren Antworten (guess).

## Plan

<!--
- Map the new content onto the app with the guide's patterns. The creator confirms the plan in one read.
- After the yes you work on your own.
-->

### Tasks

- [x] Load skill `lernapps-content-growth`. Add the tasks of Code as slices, one per competency, in the guide's
      order, one call each: `npx --no -- lernapps plan add --at slices "<task>"`. Say in each which sub-agent may
      write it in parallel, if any.
- [x] Write "Content method": the guide's patterns, figures and components per slice. Anything new: map it as skill
      `lernapps-explainer-design` says, and say why the guide's patterns do not fit.
- [x] (skipped: keine neue Komponente und keine interaktive Übung; der Seitenaufbau steht in .vibe/sketches/lesestueck-seite.md) Draw a sketch of each new component or interactive exercise, in `.vibe/sketches/`.
- [x] Show the creator, short: goal, new competencies by chapter, slices; in plain words what learners see and do and
      what is new. At most 2 questions.
- [x] **Checkpoint:** confirm the plan and the content method. Stop and wait for an explicit yes. Changes: change
      them, then ask again.
      Creator: Ja, Plan und Inhaltsmethode bestätigt. Sophie 13 bis 14, Aussehen wie in Kapitel 1, kein Neuzeichnen. indirekte-aufforderungen darf ein Dialog beim Zettel für die Klassenzimmertür sein. Weiter mit der Musterseite contact-clauses.

### Content method

<!-- One line each: the guide's patterns, figures and components used, and where; anything new, what it does and
cannot. Something new goes into the guide in the slice that adds it. -->
- Aufbau jeder Seite (Stufe 7-8, gleiche Abschnitts-IDs): `einstieg` (Vorwissen-Frage als Einzelauswahl, „Das kannst du danach“), `lesen` (Lesestück 150 bis 300 Wörter in 2 bis 3 Abschnitten, je Abschnitt eine Tabelle „Randglossar“ mit höchstens 6 schweren Wörtern; ein Chat ist eine Tabelle Nr · Wer · Nachricht, damit „Belegen mit Zeile“ eine Nummer nennt), `neu` (Satzstreifen-Figur der neuen Karte oder Weiche, Merke-Kasten, Poster-Tabelle; die Kinder finden die Regel im Lesestück: „Suche im Text …“), `uebung` (Verstehen, Belegen, Grammatik, Meinung; höchstens etwa 25 Items, vier bis sechs Übungen), `anwenden` (Schreib- oder Sprechauftrag, `open-task` oder `speaking-task`), `weiter` (nächster Schritt; letzte Seite eines Kapitels mit Rückblick). Titel sagen, was der Abschnitt tut.
- Muster (neu: Lesestück-Muster, kommt mit der Musterseite in den Inhaltsführer): Verstehen = `single-choice` oder `true-false` mit Begründung; Belegen = `number` („In welcher Nachricht steht das?“) oder `single-choice` mit Zeilennummer; Grammatik = `matching`, `language-task` (choice, write, Übersetzen), `ordering`; Meinung = `open-task` mit Punkten der Form; Hören und Nachsprechen aus kurzen Abschnitten des Lesestücks (je Seite 6 Sätze, neue Sätze, nicht aus dem Lesestück abgeschrieben: Hörliste im Inhaltsführer).
- Lesestück-Sorten je Seite: contact-clauses Chat (Sophie, Amir, Ellie über Bücher und Filme); relativsaetze-nicht-notwendig Tagebucheintrag (Sophie); konjunktionen-although Artikel der Schulzeitung; if-satz-2 Chat „Was würdest du tun, wenn …?“; if-satz-3 Blog-Eintrag über einen verpassten Bus; i-wish Blog-Eintrag (Wünsche); reported-speech Chat mit Bericht; backshift Interview mit Bericht; indirekte-aufforderungen Dialog beim Elternabend-Zettel? (guess) / Gespräch im Klassenzimmer. Orte und Figuren aus Millbrook School, keine neuen Orte; Wort für Fakten im Text: keine realen Fakten, nur Schulalltag (keine Quellenangabe nötig; sonst im Inhaltsführer „Sources“).
- Figuren: Zeichen der Satzstreifen-Familie wie in Kapitel 1; neue Karten mit neuen Farben, keine Farbe zweimal in der App: Kontaktkarte = Relativkarte gestrichelt (darf fehlen), Klammer aus Kommas = (Klammern) um den Streifen, although/while/whereas = dunkelgrau, so that = hellblau, Weiche „unwirklich“ = zwei Gleise unter dem Zeitstrahl (Zeitstrahl aus #472: Spur nach links), I wish = Karte mit Stern, Sprechblase → Streifen mit said that = Sprechblase mit Pfeil; Szenen nur, wo sie etwas zeigen (Chat und Tagebuch als Text, kein Bild nötig). Bilder `satzstreifen-<seite>.svg`, Szenen `szene-<seite>.svg` nach dem Muster von Kapitel 1, Figuren 13 bis 14 (Sophie älter: Zöpfe offen? (guess): Aussehen wie in Kapitel 1, nur größer gezeichnet).
- Wiederholung `das-brauchst-du` in K3 (simple-past, past-perfect) und K4 (past-perfect, infinitivkonstruktionen, imperativ): kompakt, Namen und Link zur Karte, ohne Übung; in K2 nicht nötig (relativsaetze und konjunktionen werden in Kapitel 1 geübt).
- Wörter: Grundwortschatz A1/A2; weniger einfache Wörter und Wörter außerhalb auf der Seite im Randglossar mit Bedeutung und im Inhaltsführer gelistet; B1-Wörter nur, wenn das Lesestück sie braucht (Randglossar).
- Hörtexte: `bf_emma`, ganze Sätze, `regen_audio.py` (neu, mit Fehllaut-Schnitt), keine Namen für den Klang, Hörliste im Inhaltsführer; Dubletten-Skript über alle Seiten.
- Jede Seite: `competencies:` mit Karten-Id; `scope` je Seite und in `app.yaml` ergänzt (Kapitel 5 weiterhin out); Selbsteinschätzung je neuem Kapitel in `chapter.yaml`.
- Wie ein späterer Agent Kapitel 5 anfügt: Muster dieser Seiten, Inhaltsführer, Abschnitt „Adding a chapter or round“.


## Code

<!--
- Build locally on the branch, on your own. After each task: `plan done`, then one commit with the work and this
  plan. The hooks check each commit; a failing check is fixed from its message, as skill `lernapps-cli` says.
- What you cannot decide: choose, write it under "Key decisions" with "(guess)", go on.
- The creator asks for a change: say your reading in one sentence first.
-->

### Tasks

- [x] `git switch -c increment/<NN>-<short name>` from `main`. Commit this plan on it.
- [x] Load skill `lernapps-cli`. Update the app as its section "Update" says. Commit the update alone and fix its
      findings before any content. The update replaces the `lernapps-*` skills: read again those you use.
- [x] Load skill `lernapps-explainer` and the content guide.
- [x] Load skill `lernapps-content-questions`. Read whole, with your file tool:
      `.agents/skills/lernapps-explainer/references/blocks.md` and
      `.agents/skills/lernapps-explainer/references/exercises.md`. A foreign language: also
      `references/language-tasks.md` in the same folder. A component in the plan: also `references/components.md`.
- [x] Decide whether the app needs `scope`, as "`scope`" in
      `.agents/skills/lernapps-explainer/references/structure.md` says. Write the choice under "Key decisions".
- [x] Musterseite relativsaetze-2/contact-clauses (Kapitel relativsaetze-2, Seite 1, ich allein, zuerst): chapter.yaml, app.yaml (scope und chapters), recap das-brauchst-du, Lesestück (Chat, 150-300 Wörter), Aufgaben, 6 Hörtexte, Inhaltsführer um das Lesestück-Muster erweitern; check, Commit
- [x] relativsaetze-2/relativsaetze-nicht-notwendig (Tagebucheintrag): Sub-Agent A, nach der Musterseite, eigener Worktree, nur src/relativsaetze-2/relativsaetze-nicht-notwendig.yaml, Bilder und Audio dieser Seite
- [x] relativsaetze-2/konjunktionen-although (Schulzeitungs-Artikel): Sub-Agent A, nach der Musterseite, nur src/relativsaetze-2/konjunktionen-although.yaml, Bilder und Audio dieser Seite
- [x] was-waere-wenn/das-brauchst-du, if-satz-2 (Chat): Sub-Agent B, nach der Musterseite, nur src/was-waere-wenn/*.yaml dieser Seiten, Bilder und Audio
- [x] was-waere-wenn/if-satz-3 (Blog oder Geschichtenauszug) und i-wish (Blog-Eintrag): Sub-Agent B, nach der Musterseite, nur src/was-waere-wenn/*.yaml, Bilder und Audio
- [x] weitersagen/das-brauchst-du, reported-speech (Chat und Bericht): Sub-Agent C, nach der Musterseite, nur src/weitersagen/*.yaml, Bilder und Audio
- [x] weitersagen/backshift (Interview in der Schulzeitung) und indirekte-aufforderungen (Dialog oder Chat): Sub-Agent C, nach der Musterseite, nur src/weitersagen/*.yaml, Bilder und Audio
- [x] Ich führe die Branches der Sub-Agenten zusammen, trage chapter.yaml und app.yaml ein, prüfe Hörsätze und Wörter über alle Seiten per Skript (keine Dubletten, nichts doppelt), lernapps check
<!-- tasks: slices (8 added): one per competency, as written in Plan -->
- [x] **Checkpoint:** the pattern page, after the first slice. A slice in a pattern the app already has: show it to
      the creator and go on. A new pattern: load skill `lernapps-learner-check`, do its learner check, fix what it
      finds, then ask the creator whether the others may follow it, and wait.
      Creator: Ja, die anderen acht Seiten dürfen nach dem Muster contact-clauses folgen, drei Sub-Agenten mit je einem Worktree sind ok. Antwort des Orchestrators in der Rolle der Ersteller:in, mit deren Erlaubnis.
- [x] Update the content guide so that it describes the app as it is now (`app-content-matches`).
- [x] Run `npx --no -- lernapps check` until it passes.
- [x] Look at every changed screen, at 360 px and on a desktop, as "Look at the app" of skill `lernapps-cli` says.

## Commit

<!--
- Publish with the creator's yes. A push to `main` publishes.
- Open the pull requests (to `main`, to the catalog) without asking: they publish nothing.
-->

### Tasks

- [x] If pages or exercises changed, load skill `lernapps-explainer-self-assessment` and update the self-assessment
      as it says. Commit.
- [ ] Load skill `lernapps-github`. Push the branch, open the preview pull request and see its checks to green, as it
      says.
- [ ] **Checkpoint:** publish. Show what the increment adds and the preview link. Ask whether it may go online. Stop
      and wait for the yes.
- [ ] Load skill `lernapps-commit`. Publish as skill `lernapps-github` says: the pull request squash-merged into
      `main`, the run of `Pages` watched to its end.
- [ ] Open the address the job `deploy` printed and confirm the new content. Never use a derived address.
- [ ] The app is listed and its entry changes (school years, summary): load skill `lernapps-listing` and write the
      changed entry. Else skip this task.
- [ ] Fill the retrospective.
- [ ] Commit this plan on `main` and push it. A push of only `.vibe/` publishes nothing.
- [ ] **Checkpoint:** list. The entry changed: open the pull request to the catalog as skill `lernapps-listing`
      says, without asking first, see it to "bestanden", then show the creator the pull request and its result. The
      entry did not change: tell the creator that the catalog updates the app by itself.
- [ ] If the plan changed since its last push, commit it on `main` and push again.

## Retrospective

<!-- At the end of Commit. Facts, short, no names. Read by review and evals. -->

### Phases reached

<!-- Last phase completed, checkpoints passed. E.g. "commit; confirmed, published". -->

### Creator turns after the plan

<!-- Number of creator messages after the confirmation, topic of each. Target: at most 3. -->

### Where I had to guess

<!-- Each gap in plan, skills, content guide, messages or answers, and your choice. "None" if none. -->
