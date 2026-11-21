---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

„Sätze verbinden mit Satzstreifen“: Explainer (Strang-App `englisch/grammatik`, Format 2, Sprache Deutsch, englische Beispiele) über das Verbinden englischer Sätze. Auftrag: Issue lernapps/apps#481 (Epic lernapps/apps#489, Konventionen dort). Die erste Version baut nur Stufe 5-6 (Kapitel 1 `saetze-verbinden`); die Kapitel 2 bis 5 (Stufen 7-8 und 9-10) kommen als Inkremente `increment/<NN>-<name>`.

## Curriculum

Englisch als erste Fremdsprache, Klasse 5-6 (erstes und zweites Lernjahr, Stufe 5-6 der Karte). Kein Lehrplan: Reihenfolge und Bausteine kommen aus der Lernlandkarte `https://lernapps.net/apps/map/englisch.json` (Fokus `competency`; diese App ist eine Strang-App des Strangs `grammatik`; Quelle der Bausteine laut Karte: KMK, Bildungsstandards für die erste Fremdsprache, i.d.F. vom 22.06.2023). Vorwissen: Hello, Millbrook! (#470), Personalpronomen (#471), simple present und will-future (#472). Nicht hier: Zeitformen (#472), Fragen im einfachen Satz (#473), Infinitiv und Gerundium (#480), Verbindungswörter für Erzählung und Argumentation (#479, #487); contact clauses, nicht notwendige Relativsätze, although und whereas (Kapitel 2); If-Sätze Typ 2 und 3, I wish (Kapitel 3); indirekte Rede (Kapitel 4); Verkürzen, Betonen, indirekte Fragen (Kapitel 5).

## Competencies

Alle vier sind Lücken der Karte, Band 5-6. Eine Seite je Baustein, Ordnung nach `requires`. Von außen braucht Kapitel 1 nur `personalpronomen`, `simple-present` und `will-future`.

1. Kapitel `saetze-verbinden` („Sätze verbinden“)
   - Wiederholung `recap: [englisch/personalpronomen, englisch/simple-present, englisch/will-future]` → `saetze-verbinden/das-brauchst-du` (ohne Übung, ohne `competencies`)
   - `konjunktionen` → `saetze-verbinden/konjunktionen` (Musterseite): „Ich kann Sätze mit and, but, or, because, when und so verbinden.“
   - `that-saetze` → `saetze-verbinden/that-saetze`: „Ich kann Gedanken und Aussagen mit einem that-Satz anschließen (I think that …).“
   - `relativsaetze` → `saetze-verbinden/relativsaetze`: „Ich kann notwendige Relativsätze mit who, which, that und whose bilden.“
   - `if-satz-1` → `saetze-verbinden/if-satz-1`: „Ich kann mit if-Sätzen Typ 1 sagen, was unter einer Bedingung wahrscheinlich passiert (If it rains, we will stay at home.).“

Die „Ich kann“-Sätze stehen wie in der Karte in `src/<kapitel>/<seite>.yaml` (nicht umformulieren). Die Baustein-Titel der Karte nennen or, when, so und whose nicht; die Ich-kann-Sätze tun es: Die Seiten üben alles, was die Ich-kann-Sätze nennen. Übungs-IDs: Präfix = Seite (`konjunktionen-…`), Diktat `<seite>-hoeren`, Nachsprechen `<seite>-nachsprechen`.

## Content structure

- Pfad: `src/saetze-verbinden/chapter.yaml`, Seiten `src/saetze-verbinden/<seite>.yaml`.
- Jede Seite (außer der Wiederholungsseite) hat dieselben Abschnitts-IDs in dieser Reihenfolge: `einstieg` (Szene als Bild, erste leichte Aufgabe, „Das kannst du danach“, Tabelle „Klassenzimmer-Poster · Neue Wörter“), `neu` (Satzstreifen-Figur, Verbindungskarte, Merke-Kasten, Poster-Tabelle), `uebung` (mindestens vier Übungen, leicht → schwer, mindestens zwei mit eigener Fehlermeldung je typischem Fehler), `anwenden` (`open-task` oder `speaking-task`), `weiter` (nächster Schritt; am Kapitelende ein Rückblick auf alle Karten). Titel sagen, was der Abschnitt tut. Die Wiederholungsseite hat nur Text und Tabellen.
- Länge: höchstens 350 Wörter Text, höchstens 4 Textblöcke hintereinander, Bild oder Übung in den ersten vier Blöcken. Jede Seite bringt einen neuen Schritt (`explainer-one-step`).
- Szene (Wo, Wer, Wann): Wo: im Klassenzimmer von Millbrook School, an der Rückwand hängt die „Satzstreifen-Wand“, ein Brett mit Papierstreifen (je ein Satz) und bunten Verbindungskarten. Wer: Mr Hill hängt sie auf, Sophie, Ellie, Peter und Amir arbeiten daran. Wann: eine Schulwoche im November, jede Seite ist ein Tag dieser Woche; am Ende schreiben die Kinder den Zettel für den Elternabend an der Klassenzimmertür (kein neuer Ort). Kein neuer Ort und keine neue Figur. Nicht benutzt, weil andere Explainer sie haben: Zeitstrahl-Wandbild (#472), Schulfest und Lagerraum (#475), „Our Millbrook“-Ausstellung im Schulflur (#476), Schilder im Flur und Café (#480). Die Kapitel 2 bis 5 setzen die Satzstreifen-Wand fort: Das Brett bekommt neue Karten (although, whereas, Klammern aus Kommas, unwirkliche Weiche, Sprechblasen), die Kinder werden älter (Stufe 7-8: Nachrichten und Chats).
- Figuren und Orte wie in #470 (nicht ändern): Sophie (blond, Zöpfe, grüne Jacke, aus Deutschland, wohnt bei den Parkers, 11 bis 12), Ellie Parker (11, roter Pferdeschwanz, rote Jacke), Peter Parker (9, kurze braune Haare, gelbe Jacke, Ellies Bruder), Amir (11, schwarze Locken, Brille, blaue Jacke), Mr Hill (Englischlehrer, graue Haare, braune Jacke), Mrs Parker. Millbrook School, Schultag ab 8:45. Geburtstage: Peter 5. Mai, Ellie 10. Juli, Amir 12. Oktober, Sophie 14. Oktober. Tabellen heißen „Klassenzimmer-Poster · …“ und „Schulkalender · …“.
- Anrede „du“.

## Terminology

- „Ausdruck“ (fester Ausdruck), nie „Wendung“. Fachbegriffe noun, verb, adjective, sentence, tense (aus #470).
- Satzstreifen (ein Streifen = ein Satz), Verbindungskarte (and, but, or, because, so, when, that), Relativkarte (who, which, that, whose; ersetzt ein Nomen), Weiche (bei if: welche Zeitformen zusammenpassen). Immer dieselben Wörter.
- Britisches Englisch (favourite, colour). Englische Aufgaben enthalten kein deutsches Wort. Englisches immer mit deutscher Bedeutung, wo ein Wort neu ist.
- Aussprache: keine Lesehilfe und keine Lautschrift (IPA gehört zu #482); Hörtexte nur als ganze Sätze.
- Wörter: Grundwortschatz A1/A2; jedes Wort steht vor der Übung auf der Seite mit Bedeutung; ein Wort außerhalb der Liste steht erklärt auf der Seite und unten unter „Sources“.

## Exercise patterns

Aufbau leicht → schwer: wählen/zuordnen → Lücke → ordnen → schreiben mit Cue → Diktat und Nachsprechen → freie Aufgabe. Je Übung `mistakes` mit eigener Meldung und `hint`; gleichwertige Antworten mit `(a|b)`.

- Streifen verbinden (`language-task`, mode `choice`): Karte als Lücke zwischen zwei Streifen, `distractors` aus echten Lernerfehlern.
- Beziehung zuordnen (`matching`): Situation ↔ Karte (and = dazu, but = Gegensatz, or = Auswahl, because = Grund, so = Folge, when = Zeit).
- Streifen ordnen (`ordering`): Wörter eines langen Satzes (Stellung von because, that, who, if).
- Streifen schreiben (`language-task`, mode `write`, `cue: "Ellie is tired · she went to bed early · so"`).
- Relativ-Karte wählen (`language-task` choice; `matching` Nomen ↔ Karte).
- Weiche stellen (`ordering`, `choice`): if + simple present, will im anderen Streifen.
- Entscheiden mit Begründung (`single-choice` mit `info` je Option).
- Hören und schreiben (`language-task` mit `audio`; je Seite drei ganze Sätze, keine Wiederholung zwischen Seiten); Nachsprechen (`speaking-task`, drei Sätze je Seite).
- Anwenden (`open-task`): Seite 1 zwei eigene Streifen verbinden, Seite 2 „I think …“ über ein Schulfach, Seite 3 Person und Sache näher beschreiben, Seite 4 der Zettel für die Tür mit if.
- Typische Fehler (jeweils `mistakes`): because und so vertauscht (Grund und Folge), and statt but, that mit Komma, Verb ans Ende wie im Deutschen, who für Sachen und which für Personen, das Pronomen bleibt stehen („the girl who she …“), who’s statt whose, „If it will rain“, beide Streifen mit will.
- Übungsarten je Seite (damit `explainer-page-variety` nicht warnt, hat jede Seite einen anderen Satz von Arten): `konjunktionen` Einzelauswahl, zuordnen, Karte wählen, ordnen, schreiben, Übersetzen, Diktat, Nachsprechen, offene Aufgabe; `that-saetze` Einzelauswahl, Mehrfachauswahl (Welche Streifen können hinter „I think“ hängen?), Karte wählen, schreiben, Übersetzen, Diktat, Nachsprechen, offene Aufgabe; `relativsaetze` Einzelauswahl, zuordnen, Karte wählen, schreiben, Übersetzen, Diktat, Nachsprechen, offene Aufgabe; `if-satz-1` Einzelauswahl (Weiche), Formen wählen, ordnen, schreiben, Übersetzen, Diktat, Nachsprechen, offene Aufgabe (Zettel).
- Gleichwertige Antworten stehen als Gruppe `(a|b)` im `target` (auch ganze Sätze, nicht verschachtelt, zum Beispiel `(If it rains we will stay in.|We will stay in if it rains.)`). Das Feld `accepted` einer Aufgabe wird von der Prüfung nicht beachtet. Satzzeichen zählen nicht (`form: { punctuation: hint }`), darum kann ein Komma nicht als Fehler gemeldet werden; die Fehlermeldungen (`mistakes`) im Modus `choice` zeigt die Vorlage derzeit nicht an, sie stehen trotzdem im Text für den Tutor.
- Eine kurze Wörtertabelle je Seite („Klassenzimmer-Poster · Neue Wörter“ oder „… · Wörter dieser Seite“) mit den neuen oder weniger einfachen Wörtern; einfache Wörter (read, play, go) gelten als bekannt und stehen nicht darin; `das-brauchst-du` hat keine Wörter. Seiten nach `konjunktionen` führen nur die Wörter auf, die im Kapitel neu sind. Szenen und Streifen-Figuren erzeugt ein kleines Skript, das nicht im Repository liegt: Die SVG-Dateien in `src/images/` sind die Quelle.
- Keine Komponente (`prefer-built-in-block`); ein Ziehen der Streifen wäre ein Wunsch für ein Inkrement. Keine Datendateien: jede Tatsache steht einmal in ihrer Seite.

## Figures

- Gebaut: `satzstreifen-streifen` (das-brauchst-du), `satzstreifen-konjunktionen` (Streifen, Karte, Streifen und alle sechs Karten mit deutscher Bedeutung), `satzstreifen-that-saetze` (mit und ohne gestrichelte that-Karte), `satzstreifen-relativsaetze` (who ersetzt she, der Streifen rückt dahinter), `satzstreifen-if-satz-1` (Weiche, Streifen vorn und hinten); Szenen `szene-konjunktionen`, `szene-that-saetze`, `szene-relativsaetze`, `szene-if-satz-1`. Satzstreifen-Familie `src/images/satzstreifen-<seite>.svg` (eigene Zeichnung, `CC-BY-4.0`, gleiche Zeichen auf jeder Seite; Hintergrund #f4efe2; Schrift mindestens 16 im 480er viewBox; Beschriftung innerhalb des `viewBox`): Satzstreifen = weißes Rechteck mit Satz; Verbindungskarten farbig (and #138d75, but #c0392b, or #8e44ad, because #2c6fd8, so #d35400, when #7f8c8d); that gestrichelt (darf fehlen); Relativkarten und if haben eigene Farben, damit keine Farbe zwei Karten bedeutet (who #0b6e8a, which #9a5b1e, whose #b0306f, if #3f4a9c); Relativkarte ersetzt das Nomen und der Streifen rückt mit Pfeil hinter das Nomen; Weiche als Gleis mit zwei Streifen (if: simple present, anderer: will).
- Szenen `src/images/szene-<seite>.svg` mit den Figuren als `<g id>` kopiert aus `millbrook-klassenzimmer.svg` von hello-millbrook und gleich gelassen; keine Fotos, keine Figuren aus Büchern, Filmen oder Marken. Quelle „eigene Zeichnung“, Lizenz `CC-BY-4.0`. `alt` sagt, was die Szene zeigt, nie die Lösung; in Aufgaben zeigt die Figur nur die Legende. Bildunterschrift nennt, wer wer ist.
- Skizzen in `.vibe/sketches/`.
- Poster und Kalender sind `table`-Blöcke.

## Sources

Karte `https://lernapps.net/apps/map/englisch.json` und die Baustein-Seiten `https://lernapps.net/apps/map/englisch/c/<id>/`; Grundwortschatz `https://lernapps.net/apps/map/englisch/grundwortschatz/` (A1/A2). Fakten aus Wikipedia (nur Fakten, keine Sätze, CC BY-SA): „English relative clauses“ (who, which, that, whose; that nur in notwendigen Relativsätzen, ohne Komma), „Conditional sentence“, geöffnet am 2026-11-21. Nicht geprüft: Wikipedia „English conjunctions“ (404), kein Klexikon-Artikel gelesen. Beispielsätze sind eigene aus dem Alltag der Figuren. Audio: KI-Stimme `bf_emma` (britisch, weiblich), mit Skill `lernapps-audio` erzeugt und als KI-generiert markiert. Alle englischen Inhaltswörter der Übungen, Tabellen und Hörtexte stehen im Grundwortschatz (A1, nur bike, purple, rabbit, cat und test sind A2); keines liegt außerhalb. Prüfung am 2026-11-21 mit der Wortliste der Karte. Material der Ersteller:in: keines.

## Adding a chapter or round

1. Baustein auf der Karte wählen; die Voraussetzungen müssen auf früheren Seiten stehen oder eine Wiederholungsseite bekommen.
2. Seite `src/<kapitel>/<seite>.yaml` mit den Abschnitten `einstieg`, `neu`, `uebung`, `anwenden`, `weiter` anlegen, in `chapter.yaml` eintragen, Competency-ID setzen.
3. Satzstreifen-Figur um die neuen Karten oder Operationen erweitern (Kapitel 2: Relativkarte darf fehlen, Klammern aus Kommas, although/whereas; Kapitel 3: Weiche mit zwei weiteren Stellungen; Kapitel 4: Sprechblase wird Streifen) und das Poster um die Zeilen der Seite.
4. Übungen aus den Mustern oben, je mit `mistakes` und `hint`; 1 bis 3 ihrer Übungen in `selfAssessment` aufnehmen, wie Skill `lernapps-explainer-self-assessment` sagt (Kapitel 1: je Seite die Übungen „Karte wählen“ und „Übersetzen“, weil sie einen deutschen Satz als Start haben und ohne die Seite verständlich sind).
5. Hörtexte: Datei `src/audio/<satz>.mp3` und Eintrag in `.agents/skills/app-content/scripts/audio-texte.json` (Datei → Satz, 6 je Seite: je 3 für Diktat und Nachsprechen), erzeugt mit `~/.cache/lernapps/audio/venv/bin/python .agents/skills/app-content/scripts/regen_audio.py .agents/skills/app-content/scripts/audio-texte.json "<Satz>"` (Skript aus hello-millbrook, schneidet das Ausklingen ab); anhören lassen; Sätze nicht zwischen Seiten wiederholen, Namen am Satzende zweisilbig.
6. Wörter gegen den Grundwortschatz prüfen; `npx --no -- lernapps check`; committen.

## Rules learned from mistakes

Aus #470 und #472 übernommen:
- Jede Übung fragt nur Wörter ab, die vorher auf der Seite stehen.
- Eine Tabelle, die eine Übung beantwortet, steht nicht direkt über ihr.
- Englische Aufgaben enthalten kein deutsches Wort.
- Mit `(a|b)` gleichwertige richtige Antworten zulassen; `case: wrong` nur dort, wo die Seite Großschreibung unterrichtet.
- Auswahlaufgaben zur Großschreibung zeigen alle Optionen gleich geschrieben.
- Audio: das Ausklingen der Stimme am Satzende abschneiden (`regen_audio.py`), Namen am Satzende zweisilbig (Sophie, Peter, Ellie, Amir).
- Bilder: Beschriftungen innerhalb des `viewBox`; Bildunterschrift nennt, wer wer ist; das `alt` verrät nie die Lösung.
- Die Antwort einer Frage steht nie im Absatz direkt darüber; das Merke-Kasten nennt andere Wörter als die Übungen, sonst schreiben die Kinder nur ab.
- Als Auswahl nur echte Lernerfehler, keine Unwörter.
- Gleichwertige Kurzformen und Satzumstellungen zulassen, als Gruppe `(a|b)` im `target` (das Feld `accepted` greift nicht).
- Der englische Cue enthält kein deutsches Wort; der deutsche Hinweis steht in `source` oder in der Aufgabe.
- Die Rückmeldung einer Einzelauswahl hängt „: “ an den Optionstext: Optionstexte enden ohne Punkt.
- Eine Auswahl-Übung (`mode: choice`) braucht einen deutschen Satz (`source`) als Start.
- Wörter, die eine Übung braucht, aber nur im Fließtext erklärt sind (like, football), stehen zusätzlich in einer Tabelle.
- Beispiele der Tabellen und Lösungen der Übungen sind nicht dieselben Sätze, sonst schreiben die Kinder nur ab.
- Je Seite höchstens eine kurze Wörtertabelle (Vorgabe der Ersteller:in nach dem Lerner-Check).
- Diktat und Nachsprechen wiederholen keine Sätze der Seite (auch nicht mit getauschtem Namen oder Farbe): eigenes Muster, andere Wörter.
- Jede Seite hat eine andere Menge an Übungsarten (`explainer-page-variety`).
