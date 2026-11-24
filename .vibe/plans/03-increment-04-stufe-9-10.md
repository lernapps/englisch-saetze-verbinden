---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Written by `lernapps plan` and the hooks. Never change a key or a value by hand.
# Archetype, as in the app's first plan. Allowed values: explainer, interactive, quiz.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit.
phase: code
# prePushFailures: failed pre-push runs of this increment, written by the hook.
prePushFailures: 0
# failedChecks: failed rules and runs, written by lernapps check and the hooks.
failedChecks: { checks-pass: 2 }
---

# Increment: increment-04-stufe-9-10

<!--
For you, the assistant. One increment of a published app: new competencies, chapters, pages, rounds, questions, or a
correction. The process is in AGENTS.md; this plan holds the method.
- `npx --no -- lernapps plan next` prints the task to do now, `plan done` ticks it and prints the next one.
- You write only below Goal, Key decisions, Notes, Answers, Content method and Retrospective, in the creator's
  language. Delete the comment of a section once the section is filled.
- The first version's decisions stand: archetype, content method, content guide. Never change an earlier plan.
- Work on the branch `increment/<NN>-<short name>`. Until Commit everything is local: push nothing.
-->

*Started 2026-11-24. Explore, Plan, Code, Commit.*

## Goal

<!-- 1–2 sentences: what learners can do after this increment. -->

## Key decisions

<!-- One line each: decision and reason. Your own choice without the creator: mark "(guess)". -->
- `scope`: Die App hat `scope` in `app.yaml` und je Seite schon (Kapitel 5 stand dort als „out“). Beides wird für Kapitel 5 fortgeschrieben: Kapitel 5 wird aus der Liste „out“ genommen, jede neue Seite bekommt ihr `scope` (was sie lehrt, was nicht hier ist). Sonst keine Änderung.
- Kein Neuzeichnen der Szenen: Kapitel 5 hat keine Szenen mit Kindern, nur Satzstreifen-Figuren und, wo nötig, Tabellen und Karten (Konventionen 2).

## Notes

<!-- New competencies by chapter (ids of the strand), didactic approach, scope, sources and licences, open questions. -->

- Strang `englisch/grammatik`, Karte `https://lernapps.net/apps/map/englisch.json` (am 2026-11-24 geöffnet). Kapitel 5 `verkuerzen-betonen` „Verkürzen, betonen, indirekt fragen“ (Band 9-10), sechs Bausteine, alle Lücken (`practisedBy` leer). „Ich kann“-Sätze wörtlich aus der Karte:
  - `indirekte-fragen` (Schritt 1, braucht backshift und fragewoerter): Ich kann Fragen indirekt wiedergeben und höflich indirekt fragen (He asked where I lived. Can you tell me where …?).
  - `which-satzbezug` (Schritt 1, braucht relativsaetze-nicht-notwendig): Ich kann mit „which“ einen Relativsatz an einen ganzen Satz anschließen (He was late, which annoyed me.).
  - `cleft-sentences` (Schritt 1, braucht relativsaetze): Ich kann einen Satzteil mit „It is … who/that …“ oder „What … is …“ hervorheben.
  - `partizip-statt-relativsatz` (Schritt 1, braucht relativsaetze und passiv): Ich kann einen Relativsatz durch ein Partizip verkürzen (the boy sitting next to me, a book written in 1990).
  - `partizip-satzverknuepfung` (Schritt 2, braucht partizip-statt-relativsatz und konjunktionen-although): Ich kann Sätze mit Partizipien verknüpfen (Walking home, I met Tom.).
  - `ing-formen` (Schritt 2, braucht gerund-oder-infinitiv und partizip-statt-relativsatz): Ich kann erkennen, ob eine -ing-Form Verlaufsform, Gerundium oder Partizip ist, und sie von Infinitivkonstruktionen abgrenzen.
- Von außerhalb nötig und in dieser App nicht geübt: `fragewoerter` (Explainer „Sätze bauen“), `passiv` und `gerund-oder-infinitiv` (noch von keiner App geübt, Karte). Eine Wiederholungsseite `das-brauchst-du` am Kapitelanfang (`recap: [englisch/fragewoerter, englisch/passiv, englisch/gerund-oder-infinitiv]`), kompakt und ohne Übung. Aus dieser App gebraucht: backshift und relativsaetze-nicht-notwendig, Seiten stehen schon.
- Seiten (Reihenfolge nach `requires`): `das-brauchst-du`, `indirekte-fragen`, `which-satzbezug`, `cleft-sentences`, `partizip-statt-relativsatz`, `partizip-satzverknuepfung`, `ing-formen` (6 Lernseiten + 1 Wiederholungsseite; eine Seite je Baustein, Konventionen und Leitidee des Auftrags).
- Form der Seiten (Konventionen 2 und 8, guess zur Umsetzung): Lesestück 300 bis 600 Wörter als Kern, jede Seite nach dem Aufbau der 7-8-Seiten (`einstieg`, `lesen` mit Randglossar, `neu`, `uebung`, `anwenden`, `weiter`), Aufgaben in drei Stufen. Ein realer oder realistischer Fall mit Daten, Quellen und einer Entscheidung je Seite, keine erfundenen Kinder. Ton sachlich. Keine Figuren-Vorstellung im Seitentext (Rückmeldung 7-8).
- Vorschlag für die Fälle (guess, Ersteller:in entscheidet; Daten werden beim Schreiben der Seite aus geöffneten Quellen genommen, ohne Beleg kein Satz): (1) `indirekte-fragen`: Anfragen per E-Mail und am Telefon an ein Museum und einen Verkehrsbetrieb, höflich indirekt fragen, dazu ein Bericht „Sie fragte, ob …“; (2) `which-satzbezug`: Wetter- und Klimadaten Großbritanniens in einem kurzen Sachtext (Met Office, OGL); (3) `cleft-sentences`: ein Sachtext über eine Entdeckung oder Erfindung („It was … who …“, „What … needed was …“), Fakten aus Wikipedia oder NASA; (4) `partizip-statt-relativsatz`: ein Artikel über ein Gebäude oder eine Sammlung („the books kept in …“, „people living in …“); (5) `partizip-satzverknuepfung`: ein Bericht über eine Wanderung oder Reise („Walking along the coast, we …“); (6) `ing-formen`: ein Artikel mit vielen -ing-Formen (Verlaufsform, Gerundium, Partizip), zum Sortieren. Bei der Entscheidung („Welche Reise nehmen wir?“) bekommt die Leser:in Daten und Quellen. Sophie (15 bis 16) bleibt als Stimme der Briefe, Berichte und Aufgaben, die anderen Kinder treten nicht mehr als Handelnde auf, Mr Hill darf vorkommen (guess; die Konventionen sagen „keine erfundenen Kinder“ und nennen Sophie mit 15 bis 16).
- Figuren und Look: die Satzstreifen-Familie wird fortgesetzt (Partizip ersetzt Relativkarte oder Konjunktion, Betonung als Spaltung des Streifens, indirekte Frage gibt den Helfer do ab); jede Kartenfarbe nur einmal; neue Bilder statt Szenen mit Kindern; ein Bild nur, wo es etwas zeigt.
- Umfang: sechs Lernseiten plus Wiederholungsseite, je Seite höchstens etwa 25 Items und 350 Wörter Erklärtext; Hörsätze je Seite sechs (drei Diktat, drei Nachsprechen), Hörurteile bestätigt der Orchestrator. Nicht hier: Zeitformen, Passiv selbst, Gerundium und Infinitiv selbst (Wiederholung), Inversion, Konjunktiv, mixed conditionals, Kapitel 6.
- Didaktik je Baustein (Satzstreifen tragen weiter; Irrtümer sind die typischen Lernerfehler, je eine eigene Meldung):
  - `indirekte-fragen`: Die Frage gibt ihren Helfer do ab und wird ein Streifen mit Subjekt vor dem Verb (He asked where I lived, nicht „where did I live“); Entscheidungsfragen bekommen if oder whether; höflich fragen mit Can you tell me where …?/Do you know if …?; Zeitverschiebung wie in Kapitel 4. Irrtümer: Inversion und do bleiben, Fragezeichen am Ende der indirekten Frage, that statt if.
  - `which-satzbezug`: Das Komma und which greifen den ganzen Streifen auf (The train was late, which annoyed everyone.); Unterschied zu who/which mit Nomen aus Kapitel 2. Irrtümer: that statt which, kein Komma, what statt which.
  - `cleft-sentences`: Der Streifen wird gespalten, ein Teil steht vorn in It is … that/who … oder What … is …; Betonung statt neue Information. Irrtümer: that statt who bei Personen ist erlaubt (kein Fehler), falsches Verb (It are …), What-Satz mit falscher Form des Verbs.
  - `partizip-statt-relativsatz`: -ing ersetzt who/which + Verlaufsform oder einfaches Aktiv, -ed oder -en ersetzt Passiv (the book written in 1990). Irrtümer: Relativkarte bleibt stehen, falsche Form (writing statt written), Partizip bei Zeitenfolge.
  - `partizip-satzverknuepfung`: Das Partizip ersetzt Konjunktion und Subjekt (Walking home, I met Tom.), das Subjekt des Partizips ist das Subjekt des Hauptsatzes (kein „dangling participle“). Irrtümer: anderes Subjekt, Konjunktion plus Partizip doppelt.
  - `ing-formen`: Rolle des Wortes im Streifen: Verlaufsform (is walking), Gerundium (Walking is healthy), Partizip (the boy walking); Abgrenzung zu to-Infinitiv (I like to walk, I like walking). Irrtümer: Gerundium und Partizip verwechselt, Infinitiv nach Präposition.
- Datenbereich: Zahlen und Daten stehen nur, wenn eine geöffnete Quelle sie nennt und im Inhaltsführer steht; sonst keine Zahlen. Keine echten Personen als Figuren der Fälle, keine Zitate echter Menschen (guess).
- Quellen, geöffnet am 2026-11-24 (nur Fakten, keine Sätze; Wikipedia CC BY-SA 4.0): „English clause syntax“ (Fragesatz als Nebensatz: Subjekt steht vor allen Verben, if oder whether bei Entscheidungsfragen, ohne do), „Reported speech“ (indirekte Frage, Pronomen, Orts- und Zeitwörter, Zeitenfolge), „English relative clauses“ (which bezieht sich auf einen ganzen Satz: The cake was burnt, which made me angry), „Participle“ (zwei Partizipien: -ing und -ed oder -en, Gebrauch als Adjektiv, bei Verlaufsform, Perfekt und Passiv), „Dangling modifier“ (das Subjekt der Partizipgruppe ist das Subjekt des Hauptsatzes). Nicht geprüft: Wikipedia „Cleft (syntax)“ und „Gerund“ (HTTP 429 beim Öffnen, nicht erneut versucht), Met Office, NASA und weitere Quellen der Fälle (werden beim Schreiben der jeweiligen Seite geöffnet; sonst entfällt der Fall). Nichts aus dem Material der Ersteller:in.

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
- [x] (skipped: Die Seiten haben den Aufbau der Stufe 7-8 mit Lesestück, das der Inhaltsführer schon beschreibt; neu ist nur die Stufe, keine neue Seitenart und keine neue Übungsart) The increment needs a kind of content the guide does not cover (a new page structure, screen, component or kind
      of exercise): load skills `lernapps-explainer-design` and `lernapps-exercise-patterns`. Else skip this task.
- [x] **Checkpoint:** research. Show in plain words: the new competencies by chapter, the didactic approach, the
      scope, every "(guess)", the sources and what is unchecked. Stop and wait. Changes: change them, then ask again.
      Creator: Recherche bestätigt: Sophie bleibt als Stimme ohne Figuren-Einführung, Ellie, Amir und Peter treten nicht auf, Mr Hill darf; Fälle einverstanden mit der Zahlenregel (nur Zahlen aus geöffneter Quelle, im Inhaltsführer nennen, keine echten Personen oder Zitate); eine Wiederholungsseite das-brauchst-du; Cleft (syntax) und Gerund später erneut öffnen. Antwort der Orchestrator-Session in der Rolle der Ersteller:in

### Answers

<!-- The creator's answers, in their words, one bullet each. -->

- Auftrag der Orchestrator-Session (in der Rolle der Ersteller:in), 2026-11-24: „Starte das Stufe-9-10-Inkrement `increment/04-stufe-9-10` auf eigenem Branch von aktuellem `main`: Kapitel 5 „Verkürzen, betonen, indirekt fragen“ (9-10). Ablauf wie bei den 7-8-Inkrementen (Plan-Checkpoint, Musterseite, Gesamtcheck und Sprachprüfung mit Sub-Agenten, Vorschau-PR, nicht mergen). Beachte `konventionen.md` (keine Figuren-Einführung im Seitentext, Vokabelblock, Hörurteile bestätigt der Orchestrator). Tooling vorher auf den neuesten Stand.“ Damit sind Kapitel, Stufe, Ablauf und Umfang (sechs Bausteine laut Karte) gesetzt; ein Mensch hat dazu nichts gesagt.
- Rückfragen ausgelassen, weil Auftrag und Konventionen (Abschnitt 8) sie beantworten: Stufe 9-10 heißt realer oder realistischer Fall mit Daten, Quellen und einer Entscheidung, keine erfundenen Kinder, Ton sachlich (guess: Sophie, Ellie, Amir, Peter treten nicht als handelnde Kinder auf; die Satzstreifen-Wand bleibt als Bild für Satzbau).

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
- [x] (skipped: Keine neue Komponente und keine interaktive Übung, der Seitenaufbau steht im Inhaltsführer) Draw a sketch of each new component or interactive exercise, in `.vibe/sketches/`.
- [x] Show the creator, short: goal, new competencies by chapter, slices; in plain words what learners see and do and
      what is new. At most 2 questions.
- [x] **Checkpoint:** confirm the plan and the content method. Stop and wait for an explicit yes. Changes: change
      them, then ask again.
      Creator: Plan und Inhaltsmethode bestätigt, so bauen. Gesamtcheck am Ende mit Sub-Agenten, nach der Musterseite indirekte-fragen und ihrem Lerner-Check melden, erst danach schreiben die drei Sub-Agenten die übrigen Seiten. Antwort der Orchestrator-Session in der Rolle der Ersteller:in

### Content method

<!-- One line each: the guide's patterns, figures and components used, and where; anything new, what it does and
cannot. Something new goes into the guide in the slice that adds it. -->
<!-- An explainer: per figure, model and component its learning action in two to four sentences
(`explainer-representation-explained`); per page its prerequisites the app does not practise, and which get a recap
page, which a link. -->
- Aufbau jeder Seite wie in Stufe 7-8 (gleiche Abschnitts-IDs `einstieg`, `lesen`, `neu`, `uebung`, `anwenden`, `weiter`; Lesestück-Muster steht im Inhaltsführer): Vorwissen-Frage als Einzelauswahl mit drei Optionen, Lesestück 300 bis 600 Wörter in Abschnitten mit Randglossar (höchstens sechs Wörter je Abschnitt), Aufgaben in drei Stufen (Verstehen, Belegen mit `number` auf die Zeilennummer, Meinung als `open-task`), Grammatik-Übungen, Schreib- oder Sprechauftrag, höchstens etwa 25 Items, 350 Wörter Erklärtext. Vokabeln als Block `vocabulary`.
- Neu gegenüber 7-8 nur die Form des Lesestücks (Konventionen 2 und 8): ein realer oder realistischer Fall mit Daten, Quellen und einer Entscheidung, sachlicher Ton, keine erfundenen Kinder. Sorten: E-Mail- und Telefon-Anfragen (`indirekte-fragen`), Sachtext mit Wetterdaten (`which-satzbezug`), Sachtext über eine Entdeckung (`cleft-sentences`), Artikel über ein Gebäude oder eine Sammlung (`partizip-statt-relativsatz`), Reisebericht mit Entscheidung (`partizip-satzverknuepfung`), Artikel mit vielen -ing-Formen (`ing-formen`). Tabellen mit Daten sind `table`-Blöcke mit Quelle in der Bildunterschrift; Sophie (15 bis 16) bleibt Stimme der Briefe und Berichte. Die Seitenart ist dieselbe, es gibt keine Komponente und keine neue Übungsart.
- Figuren (Satzstreifen-Familie `src/images/satzstreifen-<seite>.svg`, eigene Zeichnung, CC-BY-4.0, jede Kartenfarbe nur einmal in der App; die Farben der Kapitel 1 bis 4 stehen im Inhaltsführer): `indirekte-fragen` Frage-Streifen gibt den Helfer do ab und rückt das Subjekt vor das Verb, if oder whether als Karte; `which-satzbezug` Komma-Karte which greift den ganzen Streifen mit Bogen auf; `cleft-sentences` ein Streifen wird gespalten, Karte „It is … that“ hebt einen Teil hervor; `partizip-statt-relativsatz` die Relativkarte verschwindet und das Partizip steht hinter dem Nomen; `partizip-satzverknuepfung` das Partizip ersetzt Konjunktion und Subjekt, Pfeil zum Subjekt des Hauptsatzes; `ing-formen` Wort in Streifen mit Rollen (Verlaufsform, Gerundium, Partizip). Jede Figur sagt, was die Lernenden tun sollen (sortieren, ersetzen, spalten), nie die Lösung der Aufgabe.
- Wiederholung `das-brauchst-du` (`recap: [englisch/fragewoerter, englisch/passiv, englisch/gerund-oder-infinitiv]`): kompakt, ohne Übung, mit Links zur Karte; backshift, relativsaetze und relativsaetze-nicht-notwendig sind Seiten dieser App (Verweis im Text, kein Recap).
- Zahlen und Fakten: nur aus einer geöffneten Quelle, im Inhaltsführer unter „Sources“ mit Datum; ohne Beleg kein Satz. Erlaubte Quellen nach Konventionen 8 (Wikipedia, NASA, Met Office, VOA, Wikinews); keine Sätze übernehmen.
- Hörtexte: `bf_emma`, ganze Sätze (6 je Seite: 3 Diktat, 3 Nachsprechen), `regen_audio.py`, Hörliste im Inhaltsführer, keine Namen nur wegen des Klangs, Dubletten-Skript über alle Seiten (jetzt auch gegen Kapitel 1 bis 4); die Orchestrator-Session bestätigt die Hörurteile.
- Selbsteinschätzung je Seite zwei Übungen (Formen wählen oder Karte wählen, Übersetzen), wie in Kapitel 2 bis 4. `scope` je Seite und in `app.yaml` ergänzt.
- Wie ein späterer Agent ein Kapitel 6 anfügt: Muster dieser Seiten, Inhaltsführer, Abschnitt „Adding a chapter or round“.

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
- [x] Slice 1, Musterseite: Kapitel 5 `verkuerzen-betonen` anlegen (chapter.yaml, app.yaml: Kapitel, Intro ohne Alter, Scope) und Baustein `indirekte-fragen` mit Lesestück 300 bis 600 Wörter, Satzstreifen-Figur, Übungen, 6 Hörsätze; Wiederholungsseite `das-brauchst-du` (recap fragewoerter, passiv, gerund-oder-infinitiv); Guide, Inhaltsführer und Hörliste. Nur ich, kein Sub-Agent.
- [ ] Slice 2: Baustein `which-satzbezug` (Seite, Figur satzstreifen-which-satzbezug.svg, Lesestück, 6 Hörsätze). Ein Sub-Agent im eigenen Worktree darf diese Seite schreiben; chapter.yaml, app.yaml, Inhaltsführer und audio-texte.json bleiben bei mir.
- [ ] Slice 3: Baustein `cleft-sentences` (Seite, Figur satzstreifen-cleft-sentences.svg, Lesestück, 6 Hörsätze). Sub-Agent im eigenen Worktree, zusammen mit Slice 2 (zwei Seiten, eigene Dateien).
- [ ] Slice 4: Baustein `partizip-statt-relativsatz` (Seite, Figur satzstreifen-partizip-statt-relativsatz.svg, Lesestück, 6 Hörsätze). Ein zweiter Sub-Agent im eigenen Worktree darf diese Seite schreiben.
- [ ] Slice 5: Baustein `partizip-satzverknuepfung` (Seite, Figur satzstreifen-partizip-satzverknuepfung.svg, Lesestück, 6 Hörsätze). Derselbe zweite Sub-Agent wie Slice 4, andere Seitendatei.
- [ ] Slice 6: Baustein `ing-formen` (Seite, Figur satzstreifen-ing-formen.svg, Lesestück, 6 Hörsätze, Rückblick auf alle Karten des Kapitels). Ein dritter Sub-Agent im eigenen Worktree darf diese Seite schreiben.
- [ ] Slice 7: Zusammenführen: Sub-Agent-Branches einzeln mergen, chapter.yaml mit selbstEinschätzung (selfAssessment) je Seite, app.yaml, Inhaltsführer (Überblick, Quellen mit Datum, Hörliste), audio-texte.json, Dubletten-Skript über alle Seiten, Gesamtcheck der App und Sprachprüfung mit Sub-Agenten. Nur ich.
<!-- tasks: slices (7 added): one per competency, as written in Plan -->
- [ ] **Checkpoint:** the pattern page, after the first slice. A slice in a pattern the app already has: show it to
      the creator and go on. A new pattern: load skill `lernapps-learner-check`, do its learner check, fix what it
      finds, then ask the creator whether the others may follow it, and wait.
- [ ] Update the content guide so that it describes the app as it is now (`app-content-matches`).
- [ ] Run `npx --no -- lernapps check` until it passes.
- [ ] Look at every changed screen, at 360 px and on a desktop, as "Look at the app" of skill `lernapps-cli` says.

## Commit

<!--
- Publish with the creator's yes. A push to `main` publishes.
- Open the pull requests (to `main`, to the catalog) without asking: they publish nothing.
-->

### Tasks

- [ ] If pages or exercises changed, load skill `lernapps-explainer-self-assessment` and update the self-assessment
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
