---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

„Sätze verbinden mit Satzstreifen“: Explainer (Strang-App `englisch/grammatik`, Format 2, Sprache Deutsch, englische Beispiele) über das Verbinden englischer Sätze. Auftrag: Issue lernapps/apps#481 (Epic lernapps/apps#489, Konventionen dort). Die erste Version baut nur Stufe 5-6 (Kapitel 1 `saetze-verbinden`); die Kapitel 2 bis 4 (Stufe 7-8) und Kapitel 5 (Stufe 9-10) kamen als Inkremente `increment/<NN>-<name>`.

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
5. Hörtexte: Datei `src/audio/<satz>.mp3` und Eintrag in `.agents/skills/app-content/scripts/audio-texte.json` (Datei → Satz, 6 je Seite: je 3 für Diktat und Nachsprechen), erzeugt mit `~/.cache/lernapps/audio/venv/bin/python .agents/skills/app-content/scripts/regen_audio.py .agents/skills/app-content/scripts/audio-texte.json "<Satz>"` (Skript aus hello-millbrook, schneidet das Ausklingen ab); anhören lassen; Sätze nicht zwischen Seiten und nicht wörtlich auf derselben Seite wiederholen; keinen Namen nur wegen des Klangs anhängen; einsilbig endende Sätze in die Hörliste eintragen.
6. Wörter gegen den Grundwortschatz prüfen; `npx --no -- lernapps check`; committen.

## Rules learned from mistakes

Seit Tooling 0.19 (app-templates 0.20): `links` einer Frage dürfen nicht auf die Lernlandkarte zeigen (Regel `explainer-content-valid`). Die Links auf die Karte wurden entfernt; ein Link nur, wenn er genau erklärt, was die Frage fragt (zum Beispiel ein Lexikonartikel), sonst keiner.

Rückmeldung der Ersteller:in (Inkrement 02, gilt für alle Seiten):
- Keine Vorstellung der Figuren, keine Altersangaben, keine Verwandtschaftserklärungen und kein Datum im Fließtext, wenn sie für die Aufgabe nichts beitragen. Die Figuren stehen einmal auf der Startseite (`app.yaml`). Eine Figur wird nur genannt, wo die Aufgabe sie braucht (wer spricht in der Chatzeile). Das gilt auch für Einstiegs-, Lesestück- und „Wie es weitergeht“-Texte, Bildunterschriften und Alt-Texte (Alt-Texte beschreiben nur, was man im Bild sieht).

Aus #470 und #472 übernommen:
- Jede Übung fragt nur Wörter ab, die vorher auf der Seite stehen.
- Eine Tabelle, die eine Übung beantwortet, steht nicht direkt über ihr.
- Englische Aufgaben enthalten kein deutsches Wort.
- Mit `(a|b)` gleichwertige richtige Antworten zulassen; `case: wrong` nur dort, wo die Seite Großschreibung unterrichtet.
- Auswahlaufgaben zur Großschreibung zeigen alle Optionen gleich geschrieben.
- Audio: das Ausklingen der Stimme am Satzende abschneiden (`regen_audio.py`), kein Name nur wegen des Klangs am Satzende: ein Hörsatz bleibt der natürliche Satz, ein Name steht nur als Anrede, wenn der Satz ihn braucht; Sätze, die auf ein einsilbiges Wort enden, stehen in der Hörliste.
- Bilder: Beschriftungen innerhalb des `viewBox`; Bildunterschrift nennt, wer wer ist; das `alt` verrät nie die Lösung.
- Die Antwort einer Frage steht nie im Absatz direkt darüber; das Merke-Kasten nennt andere Wörter als die Übungen, sonst schreiben die Kinder nur ab.
- Als Auswahl nur echte Lernerfehler, keine Unwörter.
- Gleichwertige Kurzformen und Satzumstellungen zulassen, als Gruppe `(a|b)` im `target` (das Feld `accepted` greift nicht).
- Der englische Cue enthält kein deutsches Wort; der deutsche Hinweis steht in `source` oder in der Aufgabe.
- Die Rückmeldung einer Einzelauswahl hängt „: “ an den Optionstext: Optionstexte enden ohne Punkt.
- Eine Auswahl-Übung (`mode: choice`) braucht einen deutschen Satz (`source`) als Start.
- Wörter, die eine Übung braucht, aber nur im Fließtext erklärt sind (like, football), stehen zusätzlich in einer Tabelle.
- Beispiele der Tabellen und Lösungen der Übungen sind nicht dieselben Sätze, sonst schreiben die Kinder nur ab.
- Je Seite höchstens eine kurze Wörtertabelle (Vorgabe der Orchestrator-Session in der Rolle der Ersteller:in nach dem Lerner-Check).
- Diktat und Nachsprechen wiederholen keine Sätze der Seite (auch nicht mit getauschtem Namen oder Farbe): eigenes Muster, andere Wörter.
- Jede Seite hat eine andere Menge an Übungsarten (`explainer-page-variety`).

## Hörliste

Hörsätze, die auf ein einsilbiges Wort enden (nach dem Erzeugen mit `regen_audio.py` gezielt anhören, ob am Ende ein Fehllaut bleibt):

- `konjunktionen`: „You can have tea or you can have milk.“ (`you-can-have-tea-or-you-can-have-milk.mp3`)
- `that-saetze`: „I think that you are right.“ (`i-think-that-you-are-right.mp3`), „They know that Sophie is right.“ (`they-know-that-sophie-is-right.mp3`)
- `relativsaetze`: „We have a teacher who is nice.“ (`we-have-a-teacher-who-is-nice.mp3`), „I have a sister who sings every day.“ (`i-have-a-sister-who-sings-every-day.mp3`)
- `if-satz-1`: „If the bus is late, we will walk to school.“ (`if-the-bus-is-late-we-will-walk-to-school.mp3`), „If you are late, I will wait for you.“ (`if-you-are-late-i-will-wait-for-you.mp3`)

Geschnitten mit der Regel `valley_cut` (Fehllaut nach dem letzten Wort, `regen_audio.py` vom 2026-11-22; 4 von 24 Dateien, je zusätzlich zum Schnitt des Ausklingens): 
- „Peter has a dog and Ellie has a rabbit.“ (`peter-has-a-dog-and-ellie-has-a-rabbit.mp3`): 65 ms; endet zweisilbig, hier gezielt hören, ob „bit“ ganz da ist
- „They know that Sophie is right.“ (`they-know-that-sophie-is-right.mp3`): 45 ms
- „I think that you are right.“ (`i-think-that-you-are-right.mp3`): 75 ms
- „Sophie says that English is difficult.“ (`sophie-says-that-english-is-difficult.mp3`): 25 ms; endet dreisilbig, hier gezielt hören, ob „-cult“ ganz da ist

Hörsätze, die zwei- oder mehrsilbig enden (Risiko, dass eine Silbe angeschnitten wird; nicht geschnitten, außer rabbit und difficult oben): `konjunktionen` Sophie, Sunday, sister, happy; `that-saetze` hungry, happy, Millbrook; `relativsaetze` Millbrook, yellow, purple, English; `if-satz-1` sandwich, early, outside (zwei Sätze).

## Stufe 7-8: Seiten mit Lesestück (Inkrement 02, Kapitel 2 bis 4)

Die Kapitel `relativsaetze-2` (Relativsätze genauer), `was-waere-wenn` (Was wäre, wenn …?) und `weitersagen` (Weitersagen, was jemand sagt) gehören zur Stufe 7-8. Sophie ist jetzt 13 bis 14, Ellie und Amir sind 13, Peter 11; Aussehen und Orte wie in Kapitel 1 (Millbrook School, Satzstreifen-Wand). Die Seiten sind Lesestück-Seiten (Konventionen Abschnitt 8):

- Abschnitte in dieser Reihenfolge: `einstieg` (Vorwissen-Frage als Einzelauswahl mit drei Optionen, „Das kannst du danach“), `lesen` (Lesestück 150 bis 300 Wörter, in Abschnitten; ein Chat ist eine Tabelle Nr · Wer · Nachricht, jede Nachricht nummeriert; nach jedem Abschnitt eine Tabelle „Randglossar“ mit höchstens sechs Wörtern), `neu` (Satzstreifen-Figur, Poster-Tabelle, Merke; „Schau in den Chat“ führt zur Regel), `uebung`, `anwenden`, `weiter`.
- Aufgaben in drei Stufen: Verstehen (`single-choice` oder `true-false` über den Text), Belegen (`number`: „In welcher Nachricht …?“, Antwort ist die Nummer), Meinung (`open-task` in `anwenden`); dazu die Grammatik-Übungen wie in Kapitel 1 (`multiple-choice`, `language-task` write und Übersetzen, `matching`, `ordering`, Diktat, Nachsprechen). Höchstens etwa 25 Items je Seite. Die Länge des Lesestücks zählt nicht zu den 350 Wörtern Erklärtext (die Tabellen werden nicht gezählt).
- Das Lesestück ist ein eigener Text, erfundene Schule und Personen, keine echten Fakten (sonst mit Quelle unter „Sources“). Die Hör- und Nachsprechsätze stehen nicht im Lesestück.
- `contact-clauses` (Seite 1 von Kapitel 2) ist die Musterseite: Chat „Class 8B“ mit zwölf Nachrichten, `satzstreifen-contact-clauses.svg` (gestrichelte Karte „(that)“ in Klammern darf fehlen, `who` als Subjekt-Ersatz bleibt), Poster „Karte weglassen?“.
- Wiederholung am Kapitelanfang (`das-brauchst-du`, `recap`) nur, wo ein Baustein von außerhalb gebraucht wird: Kapitel 3 simple-past und past-perfect, Kapitel 4 past-perfect, infinitivkonstruktionen und imperativ; kompakt, ohne Übung, mit Link zur Karte.

Hörliste Kapitel 2, `contact-clauses` (`regen_audio.py` mit `valley_cut`; Dateien in `src/audio/`):
- einsilbig am Ende: „I lost the key my mother gave me.“ (`i-lost-the-key-my-mother-gave-me.mp3`), „The teacher I like best is Mr Hill.“ (`the-teacher-i-like-best-is-mr-hill.mp3`), „The cake we ate on Sunday was great.“ (`the-cake-we-ate-on-sunday-was-great.mp3`, Fehllaut-Schnitt 45 ms)
- zwei- oder mehrsilbig am Ende (Risiko angeschnittener Silbe): „The video you sent me is really funny.“, „The woman we asked was very helpful.“, „Where is the ticket I bought yesterday?“

## Kapitel 2 bis 4 (Stufe 7-8) im Überblick

- Kapitel `relativsaetze-2` („Relativsätze genauer“): `contact-clauses` (Chat „Year 8B“, Muster), `relativsaetze-nicht-notwendig` (Tagebuch von Sophie, Kommas als Klammer), `konjunktionen-although` (Artikel der Schülerzeitung „Millbrook News“, although, while, whereas, so that). Karten-Ids: `contact-clauses`, `relativsaetze-nicht-notwendig`, `konjunktionen-although`.
- Kapitel `was-waere-wenn` („Was wäre, wenn …?“): `das-brauchst-du` (Wiederholung `recap: [englisch/simple-past, englisch/past-perfect]`), `if-satz-2` (Chat, Weiche „unwirklich jetzt“), `if-satz-3` (Blog über einen verpassten Bus, Weiche „unwirklich früher“), `i-wish` (Blog, I wish und If only). Karten-Ids: `if-satz-2`, `if-satz-3`, `i-wish`.
- Kapitel `weitersagen` („Weitersagen, was jemand sagt“): `das-brauchst-du` (`recap: [englisch/past-perfect, englisch/infinitivkonstruktionen, englisch/imperativ]`), `reported-speech` (Chat), `backshift` (Interview mit Mr Hill in „Millbrook News“ und Bericht), `indirekte-aufforderungen` (Dialog an der Klassenzimmertür beim Zettel für den Elternabend). Karten-Ids: `reported-speech`, `backshift`, `indirekte-aufforderungen`.
- Figuren (`src/images/satzstreifen-<seite>.svg`, eigene Zeichnungen, CC-BY-4.0, jede Kartenfarbe nur einmal in der App): although, while, whereas #546e7a, so that #7cb342, would und would have #8d6e63, wish und If only #f9a825, said that #00838f, told … to #827717; die alten Farben stehen im Abschnitt „Figures“.
- Wörter: Vokabeln stehen im Block `vocabulary` (`caption`, `languages: { source: de, target: en }`, `entries` mit `target` und `source`), nicht in einer Tabelle „Ausdruck · Bedeutung“; ein Randglossar hat höchstens sechs Einträge je Abschnitt. Alle englischen Inhaltswörter stammen aus A1/A2, Ausnahmen stehen im Randglossar der Seite (diary, poster, project, Wales, programme; alarm, battery, charge; final, goal, regret).
- Quellen der Fakten (geöffnet am 2026-11-22, nur Fakten, keine Sätze, Wikipedia CC BY-SA 4.0): „English relative clauses“ (Kontaktsatz, nicht notwendige Relativsätze mit Kommas), „English conditional sentences“ (Typen 2 und 3), „Reported speech“ (Backshift, nicht verpflichtend, wenn das Gesagte noch gilt), „English subjunctive“ (Wünsche), „Conjunction“ (although, whereas, so that). Die Lesestücke sind eigene Texte mit erfundenen Orten und Texten (die Schülerzeitung „Millbrook News“ ist erfunden), keine fremden Sätze; die Figuren sind die bekannten, ab Kapitel 2 zwei Jahre älter (Sophie 13 bis 14, Ellie und Amir 13, Peter 11).
- Selbsteinschätzung je Kapitel: je Seite eine Aufgabe „Karte wählen“ oder „Form wählen“ und eine Übersetzen-Aufgabe (`chapter.yaml`).
- Hörliste Kapitel 2 bis 4 (Fehllaut-Schnitt durch `regen_audio.py` mit `valley_cut`; 54 Hörsätze, die Ersteller:in hört gezielt):
  - Geschnitten: „Sophie went to bed early so that she could get up at six.“ (75 ms), „If the shop had been open, I would have bought a present.“ (35 ms, endet zweisilbig), „I wish I lived closer to my cousins.“ (65 ms, zweisilbig), „I wish we had a cinema in the village.“ (55 ms, zweisilbig), „I wish the rain would stop.“ (75 ms, einsilbig), „My uncle, who lives in Wales, has two dogs.“ (75 ms, einsilbig), „Mrs Parker said that she could not find her glasses.“ (55 ms, zweisilbig).
  - Einsilbig am Ende: „Amir, who is thirteen, has a new phone.“, „Our classroom, which is on the first floor, is warm.“, „Although the film was long, nobody left.“, „My brother would be happy if he had a cat.“, „If it were Saturday, we would sleep in.“, „Ellie said that she liked the film.“, „Peter says that he never eats fish.“, „Sophie says that she is very happy here.“, „Mr Hill says that the lesson starts at nine.“, „Amir said that he had forgotten his bag.“, „Mum asked me to buy some bread.“, „Mr Hill told us to turn the page.“, „Ellie asked me to carry her bag.“
  - Dazu alle Hörsätze, die zwei- oder mehrsilbig enden, als Risiko für angeschnittene Silben (Dateien in `src/audio/`, Sätze in `audio-texte.json`).

## Stufe 9-10: Kapitel 5 `verkuerzen-betonen` (Inkrement 04)

- Kapitel „Verkürzen, betonen, indirekt fragen“, sechs Lernseiten und eine Wiederholungsseite in der Reihenfolge der Karte: `das-brauchst-du` (`recap: [englisch/fragewoerter, englisch/passiv, englisch/gerund-oder-infinitiv]`), `indirekte-fragen` (Musterseite), `which-satzbezug`, `cleft-sentences`, `partizip-statt-relativsatz`, `partizip-satzverknuepfung`, `ing-formen`. Karten-Ids wie die Dateinamen. Sophie ist 15 bis 16 und bleibt als Stimme (E-Mail, Bericht), ohne Figuren-Einführung; Ellie, Amir und Peter treten nicht mehr auf, Mr Hill darf vorkommen. Keine Szenenbilder mit Kindern, nur Satzstreifen-Figuren.
- Aufbau wie in Stufe 7-8 (Abschnitte `einstieg`, `lesen`, `neu`, `uebung`, `anwenden`, `weiter`), Lesestück 300 bis 600 Wörter zu einem realistischen Fall mit Daten und einer Entscheidung; sachlicher Ton. Zahlen und Fakten nur aus einer geöffneten Quelle, hier unter „Sources“ mit Datum. Das Museum und die Gesprächspartner in `indirekte-fragen` sind erfunden (keine echten Daten, keine echten Personen).
- Neue Karte (`satzstreifen-indirekte-fragen.svg`): Fragewort-Karten in Goldbraun #b8860b (Farbe nur hier), `if` bleibt #3f4a9c; die Figur zeigt, wie das do wegfällt und das Subjekt vor das Verb rückt.
- Quellen (geöffnet am 2026-11-24, nur Fakten, Wikipedia CC BY-SA 4.0): „English clause syntax“ (Fragesatz als Nebensatz: Subjekt vor allen Verben, if oder whether bei Ja/Nein-Fragen, Fragewort als Subjekt unverändert), „Reported speech“ (indirekte Frage, Pronomen, Zeitenfolge), „English relative clauses“ (which bezieht sich auf einen ganzen Satz), „Participle“ (zwei Partizipien auf -ing und -ed oder -en), „Dangling modifier“ (Subjekt der Partizipgruppe ist das Subjekt des Hauptsatzes). Nicht geprüft: „Cleft (syntax)“ und „Gerund“ (HTTP 429).
- Hörliste `indirekte-fragen` (`regen_audio.py`, kein Fehllaut-Schnitt nötig, nur das Ausklingen abgeschnitten): einsilbig am Ende: „Do you know when the concert starts?“ (endet auf „starts“), „He asked me where I had put my keys.“ (`keys`), „I would like to know when the new shop opens.“ (`opens`, zweisilbig); zwei- oder mehrsilbig: „She asked me whether I had finished my homework.“, „I wonder how many people live in this village.“, „Can you tell me which bus goes to the station?“.
- Selbsteinschätzung je Seite: „Karte wählen“ und „Übersetzen“ (`chapter.yaml`: `ifragen-karte`, `which-karte`, `cleft-karte`, `partrel-karte`, `partsatz-karte`, `ing-rolle`, je mit `-uebersetzen`).
- Die sechs Lesestücke (alle erfunden, kein echter Mensch, keine echten Daten; Sophie schreibt, Mr Hill darf vorkommen): `indirekte-fragen` E-Mail an ein Museum, Antwort und Bericht (336 Wörter); `which-satzbezug` Beschwerde über eine lange Schlange, Antwort mit Plänen A bis C (336); `cleft-sentences` Blog zur Schulweg-Umfrage mit Budget und drei Optionen (310); `partizip-statt-relativsatz` Artikel über eine Bibliothek in einer Mühle mit Karte oder Einzelkarte (324); `partizip-satzverknuepfung` Wanderbericht mit Streckenwahl (322); `ing-formen` Blog über einen Tennisclub an der Schule mit Trainerstunden oder neuen Schlägern (329). Zahlen darin sind erfunden und stehen im `scope` jeder Seite als erfunden; echte Fakten stammen nur aus den Quellen unten.
- Figuren: `satzstreifen-which-satzbezug.svg` (Klammer über den ganzen Streifen, which #9a5b1e), `satzstreifen-cleft-sentences.svg` (gespaltener Streifen, Karten #1b5e20 dunkelgrün), `satzstreifen-partizip-statt-relativsatz.svg` und `satzstreifen-partizip-satzverknuepfung.svg` (Partizip-Karte #4e342e dunkelbraun), `satzstreifen-ing-formen.svg` (keine neue Farbe: Rollen als Tag-Formen, grau, Partizip braun).
- Quelle für `which-satzbezug` zusätzlich: Wikipedia „English relative clauses“ (which greift einen ganzen Satz auf), geöffnet am 2026-11-24.
- Hörliste Kapitel 5 (30 Hörsätze, `regen_audio.py`, Schnitt des Ausklingens bei allen; zusätzlicher Fehllaut-Schnitt nur wo genannt; alle Urteile gibt die Orchestrator-Session in Namen der Ersteller:in ab, keiner wurde von mir gehört):
  - einsilbig am Ende: `indirekte-fragen` „Do you know when the concert starts?“, „He asked me where I had put my keys.“; `which-satzbezug` „Our neighbour plays the piano at night, which annoys everyone in the street.“ (Fehllaut-Schnitt 35 ms), „My brother cooks every day, which I really like.“ (Fehllaut-Schnitt 55 ms), „It was sunny all week, which was great for our trip.“, „The shop opens at six, which is too early for me.“, „He sings very well, which surprised his friends.“ (Fehllaut-Schnitt 55 ms); `cleft-sentences` „It was my grandmother who taught me to cook.“, „It was the cat that drank all the milk.“, „What surprised me most was the price.“; `partizip-statt-relativsatz` „The woman working in the shop is very kind.“, „The lemonade poured into the jug tastes sweet.“ (Fehllaut-Schnitt 35 ms), „The tickets bought online are cheaper than the ones at the door.“; `partizip-satzverknuepfung` „Leaving the house early, she caught the first train.“, „Sitting in the garden, he drank a cup of tea.“, „Having missed the bus, we walked to school.“; `ing-formen` „Learning a new language takes a lot of time.“, „We are meeting outside the library after school.“, „Carrying two heavy bags, the old man crossed the road.“, „Are you interested in joining the tennis club?“.
  - zwei- oder mehrsilbig am Ende (Risiko angeschnittener Silbe): die übrigen Hörsätze der sechs Seiten, besonders „Having read the menu, we ordered two pizzas.“ (Fehllaut-Schnitt 85 ms, auf „-zas“ achten) „My brother is learning to play the guitar.“ (auf „-tar“ achten), „The sofa chosen last week is very comfortable.“ (auf „-ble“ achten) und „The boy riding a red bike is my cousin.“ (auf „-sin“ achten).
- Wörter: Vokabeln als Block `vocabulary` (Randglossar je Lesestück-Teil, höchstens sechs Einträge, und „Wörter für die Übungen“); Wörter außerhalb von A1/A2 stehen im Randglossar oder in „Wörter für die Übungen“ vor ihrer Übung. Prüfung gegen die Wortliste der Karte am 2026-11-24: alle Inhaltswörter der Übungen, Tabellen und Hörsätze, die nicht in der Liste stehen, sind in einem Glossar der Seite erklärt (wo es fehlte, ergänzt: workshop, matter, cause, result, duck, hike).
