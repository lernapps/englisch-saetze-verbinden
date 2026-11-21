---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Written by `lernapps plan` and the hooks. Never change a key or a value by hand.
# Archetype, null until chosen in Explore. Allowed values: explainer, interactive, quiz.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit.
phase: commit
# prePushFailures: failed pre-push runs, written by the hook.
prePushFailures: 2
# failedChecks: failed rules and runs, written by lernapps check and the hooks.
failedChecks: { checks-pass: 4 }
---

# Plan: englisch-saetze-verbinden, first version

<!--
For you, the assistant. The process is in AGENTS.md; this plan holds the method.
- `npx --no -- lernapps plan next` prints the task to do now, `plan done` ticks it and prints the next one.
- You write only below Goal, Key decisions, Notes, Answers, Entry draft, Content method and Retrospective, in the
  creator's language. Delete the comment of a section once the section is filled.
- Work on the branch `work`, locally: push nothing before Commit.
-->

*Started 2026-11-21. Explore, Plan, Code, Commit.*

## Goal

Kinder der Klasse 5-6 verbinden auf Satzstreifen kurze englische Sätze mit and, but, or, because, when und so, schließen mit that Gedanken an, bestimmen mit who, which, that und whose eine Person oder Sache näher und sagen mit if, was unter einer Bedingung passiert. Gebaut wird nur Kapitel 1 „Sätze verbinden“; die Kapitel 2 bis 5 kommen später als Inkremente.

## Key decisions

- Archetyp `explainer`, Strang-App `englisch/grammatik` (Format 2): Die Kinder brauchen Erklärung mit Satzstreifen-Figuren, Tabellen und Übungen je Seite; nichts davon ist ein Spiel oder ein Zeitdruck-Training. Bestätigt von der Ersteller:in.
- Eine Seite je Baustein, Reihenfolge nach `requires`: konjunktionen → that-saetze und relativsaetze → if-satz-1 zuletzt (bestätigt).
- Am Kapitelanfang eine Sammel-Wiederholung `recap: [englisch/personalpronomen, englisch/simple-present, englisch/will-future]` ohne Übung, weil `if-satz-1` simple present und will braucht und die Streifen Pronomen verwenden (Karte, bestätigt).
- Geschichte (guess): Mr Hill hängt eine „Satzstreifen-Wand“ ins Klassenzimmer; Sophie, Ellie, Peter und Amir hängen Streifen und Verbindungskarten auf und schreiben am Ende den Aushang für den Elternabend. Keine neue Figur, kein neuer Ort.
- Begriffe: Satzstreifen, Verbindungskarte, Weiche (für if), „Ausdruck“ (bestätigt).
- `scope` in `src/app.yaml` und auf jeder Seite (auch der Wiederholungsseite): ja, weil jede Seite eine `open-task` hat, deren Antworten der Tutor nach dem Scope beurteilt; wie in #472.

## Notes

- Fach Englisch, Strang `grammatik`, Karte `https://lernapps.net/apps/map/englisch.json`, Fokus `competency`. Auftrag: Issue lernapps/apps#481 (Kopie in `/tmp/auftraege/orchestrierung/issues/481.md`), Konventionen Epic #489. Der Inhalt kommt vom Auftrag; die Ersteller:in bringt kein weiteres Material.
- Kapitel 1 „Sätze verbinden“ (Stufe 5-6), alle vier Bausteine sind Lücken der Karte (`practisedBy` leer):
  - `konjunktionen` (Schritt 1, öffnet 12): Ich kann Sätze mit and, but, or, because, when und so verbinden.
  - `that-saetze` (Schritt 2, öffnet 8, braucht konjunktionen): that-Satz (I think that …).
  - `relativsaetze` (Schritt 1, öffnet 9): notwendige Relativsätze mit who, which, that und whose.
  - `if-satz-1` (Schritt 3, öffnet 3, braucht will-future und simple-present): if + simple present, will im anderen Streifen.
  - Wiederholung `personalpronomen`, `simple-present`, `will-future` (Sammel-Wiederholung, kompakt, ohne Übung). Vorbild: `das-brauchst-du` in #472 (englisch-zeiten).
- Didaktik: Jeder Satz ist ein Satzstreifen. Eine Verbindungskarte hängt zwei Streifen aneinander (and, but, or, because, when, so, that). Beim Relativsatz ersetzt die Karte who/which/that ein Nomen des zweiten Streifens und schiebt den Streifen in den ersten; whose ersetzt das Possessivwort. Die Weiche bei if zeigt, welche Zeitformen zusammenpassen; in Stufe 5-6 nur die erste Stellung (wirklich: if + simple present, will).
- Übungsarten (Fremdsprachen-Muster): zuordnen (matching), ordnen (ordering: Streifen und Karten in Reihenfolge), Lücke und Auswahl (language-task gap/choice), Form schreiben mit Cue (write), Hören und Schreiben, Nachsprechen, am Ende ein open-task (Aushang). Jede Übung mit eigener Rückmeldung je typischem Fehler.
- Hürden (aus Issue und Reihe): and/but verwechseln, because/so vertauschen (Grund und Folge), that nach think/say auslassen oder nach that das Komma setzen, who für Sachen und which für Personen, whose mit who’s verwechseln, if + will im if-Streifen („If it will rain“), Komma nach dem if-Streifen am Satzanfang.
- Nicht hier: Zeitformen (#472), Fragen im einfachen Satz (#473), Infinitiv und Gerundium (#480), Verbindungswörter für Erzählung und Argumentation (#479, #487); contact clauses, nicht notwendige Relativsätze, although und whereas (Kapitel 2), If-Sätze Typ 2 und 3, I wish (Kapitel 3), indirekte Rede (Kapitel 4), Verkürzen und Betonen (Kapitel 5).
- Wörter: A1/A2 aus dem Grundwortschatz; Zeiten und Figuren wie in #472.
- Audio: Stimme bf_emma, ganze Sätze, Namen am Satzende zweisilbig, `regen_audio.py`.
- Nachprüfung (zweiter Lerner-Check, Sub-Agent, Klasse 5/6, nur geänderte Stellen) und `lernapps check` grün: Funde behoben: Das Feld `accepted` einer Aufgabe wird von der Prüfung nicht beachtet (Doku sagt: weitere ganze Antworten in Modus write), darum stehen alle gleichwertigen Sätze als Gruppe `(a|b)` im `target`; „Ellie friert“ → „Ihr ist kalt“; Wörter like, football, stay at home, doesn't und das -s bei he, she, it stehen vor den Übungen; Optionstexte der Einzelauswahl ohne Schlusspunkt (die Rückmeldung hängt „: “ an den Text). Vorlagenfehler für `app-templates`: `accepted` wirkungslos; Meldungen (`mistakes`) im Modus `choice` werden nicht angezeigt, nur „N: nicht richtig.“; Optionstext + „: “ + Info.
- Gesamtcheck der fertigen App (2026-11-21): Lerner-Check mit Sub-Agent (Kind Klasse 5/6, alle fünf Seiten, 360 und 1280 px) und Sprachprüfung Englisch/Deutsch mit Sub-Agent. Behoben: Streit „Mr Hill oder Peter fragt“; Bildunterschriften (Ellie hängt den Streifen auf, Amir steht neben Sophie); Zuordnung who/which/that eindeutig; Merke-Beispiele und Tabellenbeispiele nicht mehr gleich den Lösungen; deutsche Sätze der if-Übungen mit „morgen“, Distraktoren echte Fehler; Kommas in Diktaten; Kurzformen und Varianten; Wörter in den Tabellen; Mr Hill als Lehrer eingeführt; Rückblick; Relativ-that darf nicht fehlen (Merke); Weiche erklärt; Karten-Farben je Karte eigen; recap ohne „Ich kann“-Sätze für Kinder lesbar (Namen der Bausteine); Elternabend schon am Ende von relativsaetze angekündigt; if-Streifen vorn mit Komma. Nicht behoben: viele Wörter in Tabellen auf konjunktionen (zwei Tabellen), Wiederholung der Satzstreifen-Wand-Erklärung auf Seite 1 und 2; Meldungen der Vorlage (siehe oben) und die Satzzeichen-Meldung „hungry,.“ der Vorlage.
- Prüfung der Musterseite `konjunktionen` (2026-11-21): Lerner-Check mit Sub-Agent (Kind Klasse 5/6, 360 und 1280 px) und Sprachprüfung Englisch/Deutsch mit Sub-Agent. Behoben: Bild 1 und 2 erklären Streifen, Karten, Farben und Bedeutung; Wörter der Übungen stehen vorher in den Tabellen (eat, live, have, from, can, does not, Germany, England, Wochentage, Tiere); Tabellenbeispiele ähneln nicht mehr den Lösungen; „Gegenteil“ → „Gegensatz“; Merke-Kasten mit anderen Wörtern; Übersetzen mit deutschem Satz und gelisteten Varianten (Kurzformen, Satz mit Karte am Anfang); Meldungen als Denkanstoß statt Lösung; Ordnen mit deutschem Satz; Diktat ändert sich (zwei Sätze ersetzt); offene Aufgabe ohne Fachwörter. Nicht behoben (Vorlage, an `lernapps/app-templates` melden): Standardmeldung „Deine Fassung kann trotzdem richtig sein“ bei jeder falschen Eingabe, Hilfe-Knopf fehlt, „Lösung“ sperrt die Felder, Meldungen zur Groß-/Kleinschreibung listen auch richtige Wörter, Ordnen nur mit Auswahlfeldern, doppelter Doppelpunkt in der Rückmeldung einer Einzelauswahl.
- Quellen, geöffnet am 2026-11-21: Lernlandkarte `englisch.json` und die vier Baustein-Seiten `https://lernapps.net/apps/map/englisch/c/<id>/` (alle Quelle KMK, Bildungsstandards für die erste Fremdsprache, i.d.F. vom 22.06.2023; Lücken, Stufe 5-6); Wikipedia „English relative clauses“ (Fakten: who, which, that, whose; that nur in notwendigen Relativsätzen und ohne Komma; who für Personen) und „Conditional sentence“ (Fakten zur Bedingung, CC BY-SA, nur Fakten, keine Sätze); Grundwortschatz `https://lernapps.net/apps/map/englisch/grundwortschatz/` (Wörter der Übungen). Nicht geprüft: „English conjunctions“ (Seite 404 auf Wikipedia), kein Lehrplan nötig (Karte gibt die Reihenfolge), kein Klexikon-Artikel gelesen. Beispielsätze sind eigene aus dem Alltag der Figuren. Vorbilder zum Aufbau: Pull-Requests der Repositories englisch-zeiten, englisch-pronomen, englisch-verbketten (Branch work).
- Karte lückenhaft? Kein Fehler gefunden; `konjunktionen` heißt „and, but, because“, die Ich-kann-Aussage nennt aber auch or, when, so, und `relativsaetze` nennt whose. Die Seiten üben alles, was die Ich-kann-Sätze nennen (Hinweis für `map-review`, kein Fehler).
- Seiten und Kapitel (ein Kapitel `saetze-verbinden`, „Sätze verbinden“): `das-brauchst-du` (recap: englisch/personalpronomen, englisch/simple-present, englisch/will-future, ohne Übung) → `konjunktionen` (konjunktionen) → `that-saetze` (that-saetze) → `relativsaetze` (relativsaetze) → `if-satz-1` (if-satz-1, Kapitelende mit Rückblick). Die Reihenfolge `relativsaetze` vor `that-saetze` wäre ebenfalls erlaubt (beide Schritt 1/2); gewählt wie im Issue. Von außen braucht Kapitel 1 nur simple-present, will-future und personalpronomen (siehe Recap); keine Seite steht vor einer Voraussetzung (`ahead` nicht nötig).
- Pro Baustein, wie die Kinder dort ankommen und welchen Irrtum die Rückmeldung fängt:
  - konjunktionen: Sie hängen zwei Streifen mit je einer Verbindungskarte zusammen und sehen, welche Karte welche Beziehung zeigt (und = dazu, but = Gegensatz, or = Auswahl, because = Grund, so = Folge, when = Zeit). Irrtum: because und so vertauscht (Grund vor Folge), but statt and, Komma-Regel nicht nötig, Satzstreifen ohne Subjekt.
  - that-saetze: Sie schieben einen fertigen Streifen hinter I think / I know / Ellie says und sehen, dass that wegfallen darf. Irrtum: that mit Komma, that vor Fragen, Streifen ohne Verb, Wortstellung wie im Deutschen (Verb ans Ende).
  - relativsaetze: Sie ersetzen im zweiten Streifen das Nomen (Pronomen) durch who/which/that und schieben ihn hinter das Nomen des ersten. Irrtum: who für Sachen, which für Personen, Pronomen bleibt stehen („the girl who she…“), whose und who’s verwechselt, Komma wie im Deutschen.
  - if-satz-1: Sie stellen die Weiche: if-Streifen im simple present, anderer Streifen mit will. Irrtum: „If it will rain“, beide Streifen mit will, Komma-Gewohnheit, Reihenfolge der Streifen.
- Scope: in: and, but, or, because, when, so (Hauptsätze verbinden, when auch als Zeitwort), that-Sätze nach think, know, say, hope, see, notwendige Relativsätze mit who, which, that, whose, if-Sätze Typ 1 (if + simple present, will; auch if am Satzanfang mit Komma). Datenbereich: nur diese Karten, keine stille Auswahl: alle Verbindungswörter der Ich-kann-Sätze kommen vor. Sprache: Deutsch, Beispiele Englisch (britisch). Out: siehe „Nicht hier“.

## Explore

<!--
- Find out what the app teaches, for whom, how much and how it looks. Ask; write no code, run no `create`.
- An answer counts only in the creator's words under "Answers". At most 2 questions per message, one topic each.
-->

### Tasks

- [x] Check the start: the folder `.agents/skills/lernapps-app` exists (else stop and tell the creator that the folder
      was not started with `init`), and `git branch --show-current` prints `work` (else `git switch -c work`).
- [x] Load skill `lernapps-app`. Tell the creator in two sentences what a lernapps app is and where it will live: at
      their own address, free and public, and once listed as a copy on lernapps.net. Say that the technical part
      (GitHub) comes at the end and that you do it.
- [x] Interview: ask the topics "Goal" and "Learners" of "Answers".
- [x] Load skill `lernapps-map-assignment` and read the learning map of the subject as it says. The creator brings
      the content themselves (material, a word list, the pages): note under "Notes" which competencies of the map it
      covers. Else write the skill's assignment, with its story; the creator's yes answers the topics Content and
      Amount. A subject without a map: skip this task and say so.
- [x] Load skill `lernapps-exercise-patterns` and read its reference for the subject. Note under "Notes" how learners
      will practise what the goal names.
- [x] Choose the archetype as skill `lernapps-app` says: read the README of each archetype in question, then tell the
      creator in plain words what the chosen one can and cannot do. Write the archetype and its reason under "Key
      decisions".
- [x] Run `npx --no -- lernapps skills --archetype <name>` with the chosen archetype. It installs the archetype's
      skills and adds the archetype's tasks to this plan.
- [x] Load skill `lernapps-explainer-design`. An explainer has the look of the runtime: write "fixed by the
      archetype" under the topic "Look and feel" of "Answers".
- [x] Interview: ask every other topic of "Answers", in order. Leave out only a topic that an answer of the creator
      already covers, and note which answer. A topic nobody answered is asked once before you write an assumption
      with "(guess)".
- [x] Load skill `lernapps-content-research` and research as it says. Write under "Notes": the strand or subject, the
      competencies by chapter with their ids, the sources you opened.
- [x] Write under "Notes" which competency goes on which page and which pages form a chapter, as "Map the content" of
      skill `lernapps-explainer-design` says. Per page, name the prerequisites the app does not practise.
- [x] Write under "Notes", one line per competency: how learners get there (they derive it, they do not only read it
      off), and which misconception the feedback catches.
- [x] Write under "Notes" the scope: what is in, what is out and why, the data range (for example "all main-group
      elements", never a silent "1–20"), the languages.
- [x] **Checkpoint:** research. Show in plain words: the strand or why none, the competencies by chapter, the didactic
      approach, the scope, every "(guess)", the sources and what is unchecked, the archetype and its reason. Stop and
      wait. Changes: change them, then ask again.
      Creator: Ja, Plan-Phase. Kapitel 1 saetze-verbinden mit Sammel-Wiederholung, konjunktionen → that-saetze → relativsaetze → if-satz-1 passt. Satzstreifen-Idee trägt. Zwei Sätze zu neuer Szene/Ort in der Plan-Meldung; or, when, so, whose trotzdem üben; Wörter A1/A2, Namen am Satzende zweisilbig.

### Answers

<!-- The interview: per topic the creator's answer, in their words. Keep the topics. -->

- Goal: „Ja, deine Lesart passt zum Issue (and/but/because/when/so, that-Sätze, notwendige Relativsätze mit who/which/that/whose, if-Sätze Typ 1 mit if + simple present und will im anderen Streifen).“
- Learners: „Ja, Englisch Klasse 5-6, kennen Hello, Millbrook!, Personalpronomen und Zeiten aus #472; die bekannten Figuren.“
- Model and focus: „Vorbilder sind die fertigen Pull-Requests `englisch-pronomen`, `englisch-zeiten`, `englisch-verbketten`.“
- Hurdles: „Hürden aus dem Issue und den Seiten der Reihe (and/but, because/so, that auslassen, who/which, if + will).“
- Content: „Inhalt schreibst du aus dem Issue.“ Kein eigenes Material der Ersteller:in.
- Amount: „nur Kapitel 1, die Kapitel 2 bis 5 später als Inkremente.“
- Languages: „Sprache Deutsch mit englischen Beispielen.“
- Look and feel: „Aussehen von der Runtime vorgegeben.“ (fixed by the archetype)
- Terms: „Begriffe „Ausdruck“, Satzstreifen, Verbindungskarte, Weiche.“
- Finding the app: „Suchbegriffe (guess).“ Meine Annahme (guess): Sätze verbinden Englisch, and but because, that-Satz, Relativsatz who which, if-Satz Typ 1, Klasse 5 6.

## Plan

<!--
- Map the confirmed content onto the archetype. No new content questions: a gap in the content goes back to Explore.
- The creator confirms the plan in one read. After the yes you work on your own.
-->

### Tasks

- [x] Map the content as "Map the content" of skill `lernapps-explainer-design` says, and write the result under
      "Content method".
- [x] Choose a pattern per competency as skill `lernapps-exercise-patterns` says, and add it to "Content method".
- [x] Add to "Content method" one line per page, as "Engagement" of skill `lernapps-explainer-design` says: the
      opening task, the change of activity, the reward, the story.
- [x] Add the tasks of Code, each one a piece of work that ends in a commit. First the pattern: one complete page or
      screen, `npx --no -- lernapps plan add --at pattern "<task>"`. Then the others, one call each:
      `npx --no -- lernapps plan add --at pages "<task>"`. Each task says what it builds and what it shows.
- [x] Draw a sketch of each screen, component or interactive exercise: a static SVG or image, or the steps with what
      learners see after each. Keep the files in `.vibe/sketches/`.
- [x] Show the creator, short: goal, competencies by chapter, the Code tasks, the sketches, and the content method in
      plain words (what learners see and do, what the app cannot do). At most 2 questions.
- [x] **Checkpoint:** confirm the plan and the content method. Stop and wait for an explicit yes. Changes: change
      them, then ask again.
      Creator: Ja, so bauen. Bedingungen: competencies mit Karten-Ids, Recap ohne; je Seite mindestens zwei Übungen mit eigener Fehlermeldung je typischem Fehler; Satzstreifen-Wand-Absatz im Inhaltsführer als Szene (Wo, Wer, Wann); vor Musterseite Lerner-Check mit Sub-Agent (Klasse 5/6) und Sprachprüfung.

### Content method

<!-- One line each: the patterns and where; the figures and how they are made; the data files; each component, what it
checks and what it cannot; how a later agent adds a chapter. It becomes the content guide in Code. -->
<!-- An explainer: per figure, model and component its learning action in two to four sentences
(`explainer-representation-explained`); per page its prerequisites the app does not practise, and which get a recap
page, which a link. -->

- Strang-App `englisch/grammatik`, Format 2, Sprache `[de]`, ein Kapitel `saetze-verbinden`, Seiten `das-brauchst-du` (recap, ohne Übung), `konjunktionen`, `that-saetze`, `relativsaetze`, `if-satz-1`. Keine Komponente (`prefer-built-in-block`: zuordnen, ordnen, Lücke, Auswahl, schreiben, Diktat und Nachsprechen decken alles ab; ein Ziehen von Streifen wäre ein Wunsch für ein Inkrement). Keine Datendateien: jede Tatsache steht einmal in ihrer Seite.
- Geschichte und Orte (Antwort auf den Hinweis des Orchestrators): Kein neuer Ort. Mr Hill hängt im Klassenzimmer von Millbrook School an die Rückwand ein Brett, die „Satzstreifen-Wand“: Papierstreifen mit je einem Satz und bunte Verbindungskarten (and, but, because, …). Sie wird in einer Woche im November benutzt, die vier Seiten sind vier Tage dieser Woche. Wer: Mr Hill, Sophie, Ellie, Peter, Amir. Am Ende (Seite 4, `anwenden`) schreiben die Kinder den Zettel für den Elternabend an der Klassenzimmertür (ein Zettel, kein neuer Ort). Nicht benutzt: Zeitstrahl-Wandbild (#472), Schulfest und Lagerraum (#475), „Our Millbrook“-Ausstellung im Schulflur (#476), Schilder im Flur und Café (#480). Neue Figur: keine.
- Aufbau jeder Seite (gleiche Abschnitts-IDs): `einstieg` (Szene als Bild, kurze Aufgabe mit Einzelauswahl und Begründung, „Das kannst du danach“, Tabelle „Klassenzimmer-Poster · Neue Wörter“), `neu` (Streifen-Figur, Verbindungskarte, Merke-Kasten, Poster-Tabelle), `uebung` (mindestens vier, leicht → schwer), `anwenden` (`open-task` oder `speaking-task`), `weiter` (nächster Schritt; Seite 4 mit Rückblick auf alle Karten). Höchstens 350 Wörter Text; Tabellen heißen „Klassenzimmer-Poster · …“ und „Schulkalender · …“ wie in #472.
- Wörter: Quelle Grundwortschatz A1/A2 (`https://lernapps.net/apps/map/englisch/grundwortschatz/`); jedes Wort steht vor der Übung auf der Seite mit Bedeutung; ein Wort außerhalb der Liste wird erklärt und im Inhaltsführer gelistet. Namen am Satzende zweisilbig (Sophie, Ellie, Peter, Amir).
- Muster (Name · Kompetenz · Form):
  - Streifen verbinden · konjunktionen, that-saetze · `language-task` mode `choice` (Karte als Lücke zwischen zwei Streifen, `distractors`); als Auswahl nur echte Lernerfehler.
  - Beziehung zuordnen · konjunktionen · `matching` Situation ↔ Karte (and = dazu, but = Gegensatz, or = Auswahl, because = Grund, so = Folge, when = Zeit).
  - Streifen ordnen · alle · `ordering` der Wörter eines langen Satzes (Stellung von because, that, who, if).
  - Streifen schreiben · alle · `language-task` mode `write` mit `cue` (zum Beispiel `Ellie is tired · she went to bed early · so`), `mistakes` je typischem Fehler, gleichwertige Antworten mit `(a|b)`.
  - Relativ-Karte wählen · relativsaetze · mode `choice` who/which/that/whose; `matching` Nomen ↔ Karte (Person, Sache, gehört dazu).
  - Weiche stellen · if-satz-1 · `ordering` und `choice`: if + simple present, will im anderen Streifen; der Fehler „If it will rain“ bekommt eine eigene Meldung.
  - Entscheiden mit Begründung · `single-choice` mit `info` je Option.
  - Hören und schreiben · `language-task` mit `audio` (Diktat, drei ganze Sätze je Seite); Nachsprechen · `speaking-task` (drei Sätze je Seite); zusammen 24 Hörtexte in `audio-texte.json`, keine Wiederholung zwischen Seiten.
  - Anwenden · `open-task`: Seite 1 zwei eigene Streifen zu einem Satz verbinden, Seite 2 „I think …“ über ein Schulfach, Seite 3 eine Person und eine Sache näher beschreiben, Seite 4 der Zettel für die Tür mit if.
- Figuren und was die Kinder daran tun (`explainer-representation-explained`):
  - Satzstreifen-Familie `src/images/satzstreifen-<seite>.svg` (eigene Zeichnung, `CC-BY-4.0`, gleiche Zeichen auf jeder Seite): Ein Satzstreifen ist ein cremefarbenes Rechteck (#f4efe2) mit dem Satz. Die Verbindungskarte ist eine kleine bunte Karte zwischen zwei Streifen (and #138d75, but #c0392b, or #8e44ad, because #2c6fd8, so #d35400, when #7f8c8d); die that-Karte ist gestrichelt, weil sie fehlen darf. Die Kinder lesen daran ab, welche Beziehung die Karte zwischen den Streifen herstellt und was vor oder nach der Karte stehen muss; in Aufgaben zeigt die Figur nur die Legende, nie das Ergebnis.
  - Relativ-Figur: Der zweite Streifen verliert sein Nomen (the girl → who) und schiebt sich mit einem Pfeil hinter das Nomen des ersten Streifens. Die Kinder sehen, dass die Relativkarte das Nomen ersetzt und der Streifen in den Satz hineinrückt.
  - Weiche (if-satz-1): ein Gleis, das sich in zwei Gleise teilt; auf dem Gleis „wirklich“ steht links der if-Streifen im simple present, rechts der andere Streifen mit will. Die Kinder wählen die Zeitform je Streifen; Zusatzgleise (unwirklich jetzt und früher) sind erst Kapitel 3.
  - Szenen `src/images/szene-<seite>.svg` mit den Figuren als `<g id>` kopiert aus `millbrook-klassenzimmer.svg` von hello-millbrook; Quelle „eigene Zeichnung“, Lizenz `CC-BY-4.0`; `alt` verrät nie die Lösung; Beschriftung innerhalb des `viewBox`, Schrift mindestens 16 im 480er viewBox; Skizzen in `.vibe/sketches/`.
- Voraussetzungen, die die App nicht übt: `personalpronomen`, `simple-present`, `will-future` (stehen aus #471 und #472); sie bekommen eine Sammel-Wiederholung `das-brauchst-du` am Kapitelanfang (kompakt: Pronomen-Tabelle, simple present mit -s, will + Verb), sonst keine Wiederholung und kein Link nötig.
- Engagement je Seite (Eröffnung · Wechsel · Belohnung · Geschichte):
  - das-brauchst-du: Poster-Tabellen, keine Übung; Geschichte: Mr Hill zeigt das neue Brett. Nächster Schritt: die erste Verbindungskarte.
  - konjunktionen: Eröffnung: zwei Streifen und drei Karten zur Wahl; Wechsel: ansehen, zuordnen, ordnen, schreiben, hören; Belohnung: ein langer Satz aus zwei Streifen; Geschichte: Peter und Amir planen den Nachmittag.
  - that-saetze: Eröffnung: Ellie sagt „I think …“, welcher Streifen hängt dran; Belohnung: Gedanken mit that anschließen, auch ohne that; Geschichte: Sophie und Mr Hill über Meinungen.
  - relativsaetze: Eröffnung: „Which girl?“, ohne nähere Angabe passt keiner der Streifen; Belohnung: Personen und Sachen näher bestimmen; Geschichte: Amir sucht ein Heft.
  - if-satz-1: Eröffnung: Wetter und Pausenplan, eine Weiche; Belohnung: der Zettel für die Klassenzimmertür; Rückblick auf alle Karten; Geschichte: Planung für den Elternabend.
- Hinweise: `or`, `when`, `so` (konjunktionen) und `whose` (relativsaetze) werden geübt, auch wenn die Baustein-Titel sie nicht nennen. Komma nur dort geübt, wo es zur Regel gehört (if-Streifen am Satzanfang), sonst `punctuation: hint`.
- Ein späterer Agent erweitert das Kapitel oder fügt ein Kapitel an (Inkrement): neue Karte oder neue Operation am Streifen, das Poster wächst, Wörter gegen den Grundwortschatz, Hörtexte in `audio-texte.json`; Vorgehen im Inhaltsführer, Abschnitt „Adding a chapter or round“.

## Code

<!--
- Build the app, locally on `work`, on your own. After each task: `plan done`, then one commit with the work and this
  plan. The hooks check each commit; a failing check is fixed from its message, as skill `lernapps-cli` says.
- What you cannot decide: choose, write it under "Key decisions" with "(guess)", go on.
- The creator asks for a change: say your reading in one sentence first, then change every place it holds for
  (`feedback-applied-everywhere`).
-->

### Tasks

- [x] Load skill `lernapps-cli`. Create the app as its section "Create" says:
      `npx --no -- lernapps create --archetype explainer`.
- [x] Fill the content guide `.agents/skills/app-content/SKILL.md` from "Notes" and "Content method": every heading,
      no "FILL IN" left. Commit it before any content.
- [x] Load skill `lernapps-explainer`.
- [x] Load skill `lernapps-content-questions`. Read whole, with your file tool:
      `.agents/skills/lernapps-explainer/references/blocks.md` and
      `.agents/skills/lernapps-explainer/references/exercises.md`. A foreign language: also
      `references/language-tasks.md` in the same folder. A component in the plan: also `references/components.md`.
- [x] Decide whether the app needs `scope`, as "`scope`" in
      `.agents/skills/lernapps-explainer/references/structure.md` says. Write the choice under "Key decisions".
- [x] Pattern page konjunktionen: src/app.yaml, chapter.yaml, satzstreifen-konjunktionen.svg und szene-konjunktionen.svg, die ganze Seite (einstieg, neu, mindestens fünf Übungen, anwenden, weiter), 6 Hörtexte mit regen_audio.py; Wörter gegen A1/A2; lernapps check; committen
<!-- tasks: pattern (1 added): the one page or screen that is the pattern for the others -->
- [x] **Checkpoint:** the pattern page. Load skill `lernapps-learner-check` and do its learner check on the page. Fix
      what it finds. Then show the creator the page and ask whether the others may follow it. Stop and wait. A
      change: change the pattern first.
      Creator: Ja, die anderen vier Seiten dürfen nach diesem Muster folgen, wenn die Auflagen aus dem unabhängigen Check zuerst auf konjunktionen und danach auf allen Seiten gleich umgesetzt werden (feedback-applied-everywhere). Auflagen A bis H (Nachprüfung, Ellie hat kalt, Distraktoren mit eigenen Meldungen, home, Pillen, accepted, pycache, höchstens eine kurze Wörtertabelle).
- [x] Seite das-brauchst-du (recap: personalpronomen, simple-present, will-future, kompakt, ohne Übung) mit Satzstreifen-Wand als Einstieg; committen
- [x] Seite that-saetze: Figur und Szene, Übungen (that-Karte, ordnen, schreiben, Diktat, Nachsprechen), anwenden; 6 Hörtexte; committen
- [x] Seite relativsaetze: Relativ-Figur und Szene, who, which, that, whose geübt, Übungen, anwenden; 6 Hörtexte; committen
- [x] Seite if-satz-1: Weiche-Figur und Szene, Übungen, anwenden (Zettel für die Klassenzimmertür), Rückblick auf alle Karten; 6 Hörtexte; committen
- [x] Poster-Tabellen und Wörter über alle Seiten prüfen (nur A1/A2, sonst erklärt und im Inhaltsführer gelistet), Medienübersicht, Audio anhören lassen; committen
<!-- tasks: pages (5 added): the other pages or screens, after the pattern -->
- [x] Update the content guide so that it describes the app as built (`app-content-matches`).
- [x] Run `npx --no -- lernapps check` until it passes.
- [x] Look at every screen and state, at 360 px and on a desktop, as "Look at the app" of skill `lernapps-cli` says.
      Compare each with its sketch.
- [x] Do the whole-app check of skill `lernapps-learner-check`. Fix what it finds and write under "Notes" what you
      fixed.

## Commit

<!--
- Put the app on GitHub, publish it with the creator's yes, then list it. A push to `main` publishes.
- Open the pull requests (to `main`, to the catalog) without asking: they publish nothing.
- The creator asked to stop before publishing (a trial): stop here and say so.
-->

### Tasks

- [x] Load skill `lernapps-explainer-self-assessment`. Add the self-assessment as it says, or write under "Key
      decisions" why the app has none. Commit.
- [x] Load skill `lernapps-github`. Set up the repository and Pages as it says. Ask for the repository's name and
      every click only the creator can make, in one message.
- [x] Push `work`, open the preview pull request and see its checks to green, as skill `lernapps-github` says.
- [ ] **Checkpoint:** publish. Show what the app does and the preview link from the comment "Vorschau der App". Ask
      whether it may go online. Stop and wait for the yes.
- [ ] Load skill `lernapps-commit`. Publish as skill `lernapps-github` says: `work` into `main` as one squash commit,
      the run of `Pages` watched to its end.
- [ ] Open the address the job `deploy` printed and confirm that the app shows. Never use a derived address.
- [ ] Load skill `lernapps-listing`. Write the entry under "Entry draft" as it says, with the creator's answer to
      "Finding the app".
- [ ] Fill the retrospective.
- [ ] Commit this plan on `main` and push it: the listing check and the review read it there.
- [ ] **Checkpoint:** list. Open the listing pull request as skill `lernapps-listing` says, without asking first: the
      pull request is the review. See it to "bestanden", then show the creator the pull request and its result.
- [ ] If the plan changed since its last push, commit it on `main` and push again.

### Entry draft

<!-- YAML valid against the entry schema the listing skill names. Only known values, never invented. -->

```yaml
```

## Retrospective

<!-- At the end of Commit, before the listing pull request. Facts, short, no names. Read by review and evals. -->

### Phases reached

<!-- Last phase completed, checkpoints passed. E.g. "commit; confirmed, published". -->

### Creator turns after the plan

<!-- Number of creator messages after the confirmation, topic of each. Target: at most 3. -->

### Where I had to guess

<!-- Each gap in plan, skills, messages or answers, and your choice. "None" if none. -->
