# Lehrbuch · BPE 1 bis BPE 8

**Projektdokumentation und Gedächtnisstütze für alle Beteiligten (Mensch + KI-Agenten).**

**Inhalt:**
[1 Projektüberblick](#1-projektüberblick) ·
[2 Dateistruktur](#2-dateistruktur) ·
[3 Konventionen](#3-konventionen--wichtige-bausteine-gedächtnisstütze-für-ki-agenten) ·
[4 Änderungsprotokoll](#4-änderungsprotokoll) ·
[5 Offene Punkte](#5-offene-punkte--to-do) ·
[6 Verifikation](#6-verifikation-stand-v24) ·
[7 Quellenrollen](#7-quellenrollen-und-konsolidierung)

> ⚠️ **Regel für alle KI-Agenten (Claude, Codex, …):** Wer etwas am Lehrbuch ändert,
> trägt es unten im [Änderungsprotokoll](#4-änderungsprotokoll) ein (Datum **mit
> Uhrzeit**, Autor, Änderung) und aktualisiert bei Bedarf die
> [offenen Punkte](#5-offene-punkte--to-do). Diese Datei zuerst lesen, dann arbeiten.

---

## 1. Projektüberblick

| | |
|---|---|
| **Ziel** | Übersichtliches, anschauliches Informatik-Lehrbuch für Schüler |
| **Zielgruppe** | Informatik, Berufliches Gymnasium Baden-Württemberg, Eingangsklasse, Jahrgangsstufen 1 und 2 |
| **Umfang (Zielstruktur)** | **BPE 1 bis BPE 8** in Bildungsplan-Reihenfolge; HTML-Lesefassung aktuell für **BPE 5 bis BPE 8** ausgearbeitet |
| **Anrede** | Kapitel, Spickzettel und Checklisten nutzen überwiegend **„Sie“** wie die offiziellen Materialien; Startseite, Inhaltsverzeichnis und Glossar sind schülernah mit **„du“** formuliert. Vollständige Vereinheitlichung ist ein offener Redaktionspunkt. |
| **Sprache** | Deutsch |
| **Technik** | Reines HTML/CSS/Vanilla-JS, **keine Frameworks, keine CDN-Abhängigkeiten** – muss komplett **offline** funktionieren (Doppelklick auf `index.html` genügt) |
| **Projektort** | `D:\Google Drive\Codex\Lehrbuch` |
| **GitHub** | <https://github.com/JakobSawazki/Lehrbuch> |
| **Web-Ausgabe** | <https://jakobsawazki.github.io/Lehrbuch/> |
| **Kanonische Quelle** | Ausschliesslich dieses Verzeichnis; der fruehere Ordner `D:\Google Drive\Codex\PythonWorkbook` wurde am 2026-07-16 nach vollstaendigem Vergleich entfernt |
| **Integration in PythonLab** | PythonLab verweist über den Reiter **Lehrbuch** auf das eigenständige Projekt (`../Lehrbuch/`). Die Lehrbuchseiten enthalten oben den Rücklink `← PythonLab`. |
| **Auftraggeber** | Jakob Sawazki (Lehrer) |

### Inhaltliche Quellen (nicht verändern, nur lesen!)

- **Bildungsplan** (Grundlage für alles):
  [`D:\Google Drive\Codex\PythonLab\resources\29-TB02-Inhalt-Band 2a-AG-3 Informatik.pdf`](../PythonLab/resources/29-TB02-Inhalt-Band%202a-AG-3%20Informatik.pdf)
  – BPE 5 auf S. 14–15 · BPE 6 „Relationale Datenbanken“ auf S. 15–16 · **BPE 7 auf S. 17–18** · BPE 8 „Gesellschaftliche Aspekte“ auf S. 18 · Operatorenliste ab S. 19
- **Materialien zur BPE 5** (Landesbildungsserver BW):
  `D:\Google Drive\Codex\PythonLab\resources\bpe-5-grundlagen-der-programmierung-version-mit-python\bpe-5-gdp_python`
  (Lernfortschritt 1 = Kara, Lernfortschritt 2 = Python-Grundlagen/Thonny, Lernfortschritt 3 = Kontrollstrukturen; jeweils Informationen / Aufgaben / Lösungen + Ich-Kann-Listen)
- **Materialien zur BPE 7** (Landesbildungsserver BW):
  `D:\Google Drive\Codex\PythonLab\resources\bpe-7-algorithmen-datenstrukturen-python`
  (Lernfortschritt 1 = Datenstrukturen/Arrays, Lernfortschritt 2 = Algorithmik: Bubble/Selection Sort + lineare/binäre Suche, Lernfortschritt 3 = verkettete Liste/Stack/Queue/Baum; jeweils Informationsmaterial / Arbeitsaufträge / Lösungen inkl. `.py`-Programme + Ich-Kann-Listen + Kompetenzraster)
- **Materialien zur BPE 8** (Landesbildungsserver BW):
  `D:\Google Drive\Codex\PythonLab\resources\bpe-8-gesellschaftliche-aspekte`
  (Lernfortschritt 1 = Einfluss von Algorithmen im Alltag und optionale KI-Vertiefung;
  Lernfortschritt 2 = Graphgrundlagen, Modellierung, kürzeste Wege und KI-Bezüge;
  Lernfortschritt 3 = Chancen und Risiken; jeweils Arbeitsaufträge, Lösungen,
  Ich-Kann-Liste und Kompetenzraster)
- **BPE 6:** Der fachliche Ausbau folgt direkt dem Bildungsplan S. 15–16.
  Im lokalen Ressourcenbestand wurde am 2026-07-16 kein separates offizielles
  BPE-6-Materialpaket gefunden; Beispiele und Übungen wurden daher eigenständig
  und lehrplangetreu entwickelt.
- **PythonKara** (SwissEduc):
  <https://www.swisseduc.ch/informatik/karatojava/pythonkara/>
  (offizielle Seite für Download und lokale Ausführung von PythonKara; im Lehrbuch bei Kapitel 1, Glossar, Spickzettel und Werkzeugübersicht verlinkt)
- Übungen im Lehrbuch referenzieren die Original-Arbeitsblätter per Kürzel (z. B. „L3_2_2“ bzw. bei BPE 7 mit Zusatz „(BPE 7)“).

---

## 2. Dateistruktur

```
Lehrbuch/
├── README.md                         Arbeitsprinzip und Einstieg
├── book.md                           Gesamtaufbau des Fachbuchs
├── curriculum-map.md                 Bildungsplan-Abdeckung BPE 1 bis BPE 8
├── chapters/                         genau ein übergeordnetes Markdown-Kapitel je BPE
├── exercises/                        BPE-bezogene Aufgabensammlungen
├── solutions/                        bewusst getrennte Lösungsplanung
├── index.html                        Startseite der Web-Lesefassung
├── inhaltsverzeichnis.html           Lernlandkarte und Detailnavigation
├── kapitel-1-kara.html               BPE 5: Kara und Struktogramme
├── kapitel-2-python-grundlagen.html  BPE 5: Python-Grundlagen
├── kapitel-3-kontrollstrukturen.html BPE 5: Kontrollstrukturen
├── bpe-6-relationale-datenbanken.html BPE 6: vollständige Datenbank-Lesefassung
├── kapitel-4-arrays.html             BPE 7: Arrays
├── kapitel-5-sortieren-suchen.html   BPE 7: Sortieren und Suchen
├── kapitel-6-datenstrukturen.html    BPE 7: dynamische Datenstrukturen
├── bpe-8-gesellschaftliche-aspekte.html BPE 8: vollständige Abschluss-Lesefassung
├── glossar.html                      Glossar und Befehlsübersicht
├── referenz.html                     Spickzettel
├── checklisten.html                  interaktive Ich-kann-Checklisten
├── DOKUMENTATION.md                  diese Datei
└── assets/
    ├── style.css                     zentrales Stylesheet
    ├── lehrbuch.js                   Syntax-Highlighter, Quiz und Checklisten
    ├── kara.js                       Kara-Simulator
    ├── lehrbuch-logo.png             fotorealistisches PNG-Logo
    ├── lehrbuch-favicon.png          Browser-Tab-Icon
    └── lehrbuch-apple-touch.png      Touch-Icon
```

Die acht HTML-Lektionen vertiefen BPE 5 bis BPE 8. Die sechs nummerierten
Kapitel sind fachliche Unterkapitel von BPE 5 und BPE 7; BPE 6 und BPE 8
liegen als zusammenhängende HTML-Lesefassungen vor. Die acht Dateien in `chapters/`
bilden dagegen die einmalige BPE-Hauptebene. Neue
Inhalte werden einer dieser Ebenen zugeordnet und nicht als Parallelfassung
angelegt.

---

## 3. Konventionen & wichtige Bausteine (Gedächtnisstütze für KI-Agenten)

### Didaktische HTML-Bausteine (zentral in `assets/style.css` definiert)

| Baustein | Markup | Zweck |
|---|---|---|
| Lernziele | `<div class="box box-ziel">` | 🎯 am Abschnittsanfang |
| Information | `<div class="box box-info">` | ℹ️ Hintergrundwissen |
| Merke | `<div class="box box-merke">` | 📌 Kernaussagen (gelb) |
| Achtung | `<div class="box box-achtung">` | ⚠️ typische Stolperfallen (rot) |
| Tipp/Ausprobieren | `<div class="box box-tipp">` | 💡 Experimentier-Aufträge (grün) |
| Code | `<pre class="code">` | wird von `lehrbuch.js` automatisch als Python hervorgehoben; SQL mit `data-lang="sql"` |
| Konsolen-Ausgabe | `<pre class="output">` | Benutzereingaben darin: `<span class="eingabe">`, Fehler: `<span class="fehler">` |
| Übungsaufgabe | `<div class="uebung">` mit `.uebung-kopf` + `.uebung-inhalt` | Lösung als `<details class="loesung">` (aufklappbar) |
| Quiz | `<div class="quiz" data-erklaerung="…">` | Antworten als `<button class="antwort">`, richtige mit `data-richtig` |
| Checkliste | `<div class="checkliste">` | Checkboxen mit `id` → Zustand in `localStorage` (Präfix `pywb-`) |
| Zwei Spalten | `<div class="vergleich">` | z. B. Struktogramm neben Code |
| Array-Grafik | `<div class="arr">` mit `.zelle` (`.wert` + `.idx`), Hervorhebung: `.hervor`/`.neu` | indizierte Speicherzellen (Kapitel 4/5) |
| Verkettete Liste | `<div class="vkette">` mit `.anker`, `.knoten` (`.daten` + `.zeiger`), `.pfeil`, `.nullm` | Kapitel 6 |
| Stack / Queue | `.stapel-wrap`/`.stapel` bzw. `.queue` mit `.element` | LIFO/FIFO-Grafiken (Kapitel 6) |
| Bäume | Inline-SVG direkt in `kapitel-6-datenstrukturen.html` | Wurzel gelb, innere Knoten blau, Blätter grün |
| Datenbankmodelle | `.er-modell`, `.schema-grid`, `.normalform-weg`, `.daten-ampel` | BPE 6: ER-Modell, Relationen, Normalisierung und Datenbewertung |
| Algorithmus-Wirkung | `.algo-weg`, `.entscheidung-fluss` | BPE 8: Daten, Regeln, Ergebnis und gesellschaftliche Wirkung |
| Graphmodelle | `.graph-visual`, `.graph-knoten`, `.graph-kante`, `.graph-gewicht` | BPE 8: Netzwerke und gewichtete Wege als responsive SVG-Grafiken |
| Beurteilung | `.bewertungsraster`, `.fallvergleich` | BPE 8: Kriterienraster und Fallvergleiche |

### Struktogramme (Nassi-Shneiderman, reines CSS)

- Container: `<div class="stg">`, Titel: `.stg-titel`, Anweisung: `.stg-zeile`
- Schleife: `.stg-schleife` → `.stg-schleife-kopf` + `.stg-schleife-koerper` (eingerückt)
- Verzweigung: `.stg-if` → `.stg-if-kopf` (mit `<span class="bed">`, `<span class="ja">`, `<span class="nein">`) + `.stg-if-zweige` (zwei `<div>`; leerer Zweig: `<div class="leer">∅</div>`)
- **Die Diagonalen der Verzweigung** werden per SVG-Data-URI in `.stg-if-kopf::before` gezeichnet:
  von den **oberen Ecken zur Mitte unten** (klassische Form: Bedingung im oberen Dreieck,
  „Ja“ unten links, „Nein“ unten rechts). Nicht wieder umdrehen!

### Weitere Regeln

- Navigation: identische `<nav class="topnav">` auf **allen** Seiten – bei neuen Seiten überall ergänzen.
- Anker-IDs bleiben stabil (`#for`, `#while`, `#alternative`, …) – Checklisten und Inhaltsverzeichnis verlinken darauf.
- Der bestehende localStorage-Praefix `pywb-` bleibt aus Kompatibilitaetsgruenden erhalten, damit bereits gespeicherte Checklistenstaende nicht verloren gehen.
- Druckansicht ist vorbereitet (`@media print`): Lösungen werden ausgeklappt, Nav/Simulator ausgeblendet.
- Dezimalzahlen in Code-Beispielen mit Punkt; Fachbegriffe wie im Original (Zählerschleife, kopfgesteuerte Schleife, …).
- Lokaler Test-Server: im Ordner `D:\Google Drive\Codex` mit `python -m http.server 8750`; Lehrbuch dann unter `/Lehrbuch/` öffnen.

---

## 4. Änderungsprotokoll

Neue Zeilen tragen das Datum **mit Uhrzeit** im Format `JJJJ-MM-TT HH:MM`
(Wunsch von Jakob, 2026-07-07 – an einem Tag passiert oft viel).
Ältere Zeilen ohne Uhrzeit bleiben unverändert.

| Datum | Version | Autor | Änderungen |
|---|---|---|---|
| 07.07.2026 | 1.0 | Claude (Fable 5) | Grundgerüst erstellt: Quellenanalyse (Bildungsplan-PDF + alle 124 Original-Dokumente der Lernfortschritte 1–3), Startseite, Kapitel 1–3, Spickzettel (`referenz.html`), interaktive Ich-kann-Checklisten, zentrales CSS (Boxen, CSS-Struktogramme, Druckansicht), `workbook.js` (Python-Syntax-Highlighter, Quiz, localStorage-Checklisten), 21 Übungsaufgaben mit aufklappbaren Lösungen aus den Originalmaterialien |
| 07.07.2026 | 1.1 | Claude (Fable 5) | Interaktiver **Kara-Simulator** (`assets/kara.js`) in Kapitel 1: freies Steuern + 4 Schritt-für-Schritt-Programmszenarien (Sequenz, for, while, while+Alternative) mit Code-Zeilen-Hervorhebung; **Schreibtischtest-Übung** (Übung 9, klausurtypisch) in Kapitel 3 |
| 07.07.2026 | 1.2 | Codex | **Glossar** (`glossar.html`: Begriffe, Python-/Kara-/tkinter-Befehle, Operatoren), **Inhaltsverzeichnis** (`inhaltsverzeichnis.html` mit Lernlandkarte), Navigation auf allen Seiten vereinheitlicht/gekürzt (K1/K2/K3 + Inhalt + Glossar), Querverweis Spickzettel↔Glossar, Struktogramm-Diagonalen von CSS-Gradient auf SVG umgestellt |
| 07.07.2026 | 1.3 | Claude (Fable 5) | Struktogramm-Diagonalen **korrigiert**: Linien laufen jetzt von den oberen Ecken zur Mitte unten (klassische Nassi-Shneiderman-Form, Wunsch von Jakob per Skizze) – zentral in `style.css`, wirkt auf alle Seiten; `DOKUMENTATION.md` angelegt |
| 07.07.2026 | 1.4 | Claude (Fable 5) | **BPE 7 „Algorithmen und Datenstrukturen“ komplett eingepflegt** (Quellen: neuer Materialordner `bpe-7-…` + Bildungsplan S. 17–18): drei neue Kapitel `kapitel-4-arrays.html` (Datenstrukturen-Überblick, Arrays inkl. Schreibtischtest, Wetterstation, Kapitalrechner), `kapitel-5-sortieren-suchen.html` (Algorithmus-Eigenschaften, Bubble/Selection Sort mit offiziellen Implementierungen, lineare/binäre Suche, Vergleich) und `kapitel-6-datenstrukturen.html` (verkettete Liste, Stack, Queue, Baum/Binärbaum mit SVG-Grafiken). Dazu: Navigation auf allen Seiten um K4–K6 erweitert, Startseite (Titel, Hero, JG2-Lernweg-Karten, TOC-Blöcke, Bildungsplan-Tabelle BPE 7.1–7.3), Inhaltsverzeichnis (Lernlandkarte-Etappen 4–6 + Abschnittslisten), drei neue Ich-kann-Checklisten (`#bpe7lf1–3`, nach offiziellen Ich-Kann-Listen), Spickzettel-Abschnitte Arrays / Sortieren & Suchen / dynamische Datenstrukturen, neue CSS-Bausteine (`.arr`, `.vkette`, `.stapel`, `.queue`) |
| 07.07.2026 | 1.5 | Codex | **BPE-7-Abschlussrunde:** `glossar.html` um zentrale BPE-7-Begriffe erweitert (Array, Index, Datenstruktur, Bubble/Selection Sort, lineare/binäre Suche, verkettete Liste, Stack/LIFO, Queue/FIFO, Baum/Binärbaum, Knoten, Wurzel, Zeiger) und eine BPE-7-Befehlsübersicht ergänzt (`append()`, `insert()`, `pop()`, `remove()`, Indexzugriff, `len()`, Such-/Tauschmuster, Stack/Queue-Modellierung). Fußzeilen in `glossar.html`, `referenz.html`, `inhaltsverzeichnis.html` und `checklisten.html` auf BPE 5 + BPE 7 aktualisiert; mobile Tabellen/Code-Vergleiche gegen horizontales Überlaufen abgesichert; Stylesheet-Link mit `?v=1.5.1` cache-sicher gemacht; Dokumentation bereinigt. |
| 07.07.2026 | 1.6 | Codex | Startseiten-Symbol „Struktogramme“ in `assets/style.css` neu gezeichnet: weiterhin blau, rote/irritierende Markierungen entfernt. Drei Zusatzübungen für BPE 7 ergänzt: Kapitel 4 „Laufzeiten auswerten“ (parallele Arrays, Minimum, Durchschnitt, Zählen), Kapitel 5 „Binäre Suche: nicht gefunden“ (Trace mit leerem Suchbereich), Kapitel 6 „Dateisystem als Baum“ (Wurzel, Blätter, Höhe, Binärbaum, Pfad). Stylesheet-Link auf `?v=1.6` aktualisiert. |
| 07.07.2026 | 1.7 | Codex | Workbook-Kopie in `PythonLab/workbook/` integriert: alle Seiten erhielten in der Topnavigation den Rücklink `← PythonLab`; `assets/style.css` um die Klasse `.lab-ruecklink` erweitert. Die Originalquelle `D:\Google Drive\Codex\PythonWorkbook` bleibt als eigenständiger Arbeitsordner erhalten. |
| 07.07.2026 | 1.8 | Codex | Eigenes fotorealistisches PNG-Logo (`assets/workbook-logo.png`) und daraus abgeleitete Favicons eingebunden; Topnavigation zeigt nun Bildmarke + Text. Startseite zeigt das Workbook-Logo im Hero. Offizielle SwissEduc-PythonKara-Seite in Werkzeugübersicht, Kapitel 1, Glossar und Spickzettel verlinkt. Stylesheet-/Script-Links auf `?v=1.8` aktualisiert. |
| 07.07.2026 | 1.9 | Codex | Footer der Workbook-Startseite aufgeräumt: BPE-/Quellenhinweise stehen nun in einem kleinen Info-Button unten links (`details.footer-info`), rechts steht `Designed by Sawazki Electronics` mit Link auf die Sawazki-Electronics-Homepage. Startseite lädt `assets/style.css?v=1.9` und `assets/workbook.js?v=1.9`. |
| 07.07.2026 | 2.0 | Codex | Lehrbuch aus PythonLab herausgeloest und als eigenstaendiges Projekt nach `D:\Google Drive\Codex\Lehrbuch` verschoben. Markdown-Quelle konsequent nach BPE 1 bis BPE 8 strukturiert (`chapters/bpe-1-...` bis `bpe-8-...`). HTML-Startseite um BPE-1-bis-BPE-8-Uebersicht erweitert, Navigation auf BPE5/BPE7-Kapitelbezeichnungen angepasst, Ruecklink zeigt nun auf `../PythonLab/`. PythonLab verlinkt ueber den Reiter `Lehrbuch` auf `../Lehrbuch/`. |
| 2026-07-16 08:14 | 2.1 | Codex | Standalone-Projekt `PythonWorkbook` vollständig mit dem Lehrbuch verglichen: sämtliche Inhalte waren bereits enthalten, die Lehrbuchfassungen waren die neueren bzw. erweiterten Varianten. Das Lehrbuch als einzige Quelle festgelegt, Rollen von BPE-Markdown und HTML-Unterkapiteln dokumentiert, Assets von `workbook-*` auf `lehrbuch-*` umbenannt, Cache-Versionen auf `2.1` vereinheitlicht und den veralteten Doppelordner nach der Verifikation entfernt. |
| 2026-07-16 08:26 | 2.1 | Codex | Eigenständiges öffentliches GitHub-Repository `JakobSawazki/Lehrbuch` erstellt und erfolgreich über GitHub Pages veröffentlicht. Private Memory-, Ideen-, Ressourcen- und Implementierungsdateien bleiben per `.gitignore` ausgeschlossen. |
| 2026-07-16 08:51 | 2.2 | Codex | **BPE 6 „Relationale Datenbanken“ vollständig als HTML-Lesefassung ausgebaut:** Lehrpfad vom ER-Modell über Relationen, Schlüssel und 3. Normalform bis zu `CREATE`, `INSERT`, `SELECT`, `JOIN`, Aggregatfunktionen, Gruppierung und der Bewertung personalisierter Massendaten. Sieben Übungen mit Lösungen, Quizfragen, responsive ER-/Schema-Grafiken, SQL-Syntaxhervorhebung, zwölf Ich-kann-Ziele sowie Einbindung in Startseite, Lernlandkarte, Inhaltsverzeichnis, Glossar und Spickzettel ergänzt. Grundlage: Bildungsplan S. 15–16; ein separates offizielles BPE-6-Materialpaket lag lokal nicht vor. |
| 2026-07-16 09:21 | 2.3 | Claude (Fable 5) | **Gesamtsichtung + Lesbarkeits-Optimierung:** (1) Öffentliche Markdown-Dateien (chapters, exercises, solutions, book.md, curriculum-map.md, README.md) von ASCII-Umschrift auf echte Umlaute konvertiert (wortlistenbasiert, Code/Dateinamen geschützt; „Quelle/Queue/zuerst“ etc. unangetastet) + Tippfehler „Ablaufe“→„Abläufe“. (2) Startseite: BPE-6-Lernweg-Block auf „du“ angeglichen (Seite war intern gemischt); BPE-5-/BPE-7-Karten verlinken jetzt auf die HTML-Kapitel statt auf rohe Markdown-Dateien. (3) BPE-6 Übung 2: Kardinalitäts-Lösung Lehrkraft–Kurs macht die Modellannahme explizit (n:m vs. 1:n). (4) **Lehrbuch-Typografie in style.css:** Fließtext auf `--lese-breite: 76ch` begrenzt (vorher ~108 Zeichen/Zeile, jetzt ~79), Tabellen/Code/Grafiken behalten volle Breite; deutsche Silbentrennung (`hyphens: auto`), `text-wrap: pretty/balance`, Zeilenhöhe 1.7 im Fließtext. (5) `lehrbuch-logo.png` von 2 MB/1254 px auf 75 KB/660 px komprimiert (Original in `tmp/lehrbuch-logo-original.png`), Cache-Buster am Hero-Logo ergänzt. Cache-Versionen überall auf `?v=2.3`. (6) **Sicherheit:** `tmp/` in `.gitignore` aufgenommen – der Ordner enthält Renderings des privaten Bildungsplan-PDFs und das Logo-Original und war bisher untracked (Gefahr bei `git add -A`). Browser-geprüft: 12 Seiten fehlerfrei, keine kaputten Links, kein Overflow (Desktop + 390 px), Kara-Simulator und Quiz funktionieren. Nicht committet – Push entscheidet Jakob. |
| 2026-07-16 10:33 | 2.4 | Codex | **BPE 8 „Gesellschaftliche Aspekte“ vollständig ausgebaut:** eigenständige HTML-Lesefassung zu BPE 8.1–8.3 mit algorithmischem Einfluss, Informationsvorauswahl und Filterblase, Graphbegriffen, sozialem Netzwerk, gewichteter Wegsuche, Beurteilungsraster, drei Quizfragen sowie acht Übungen mit Lösungen. 15 Ich-kann-Ziele, Graphen-Spickzettel und Glossarbegriffe ergänzt; Startseite, Lernlandkarte, Inhaltsverzeichnis und Navigation vollständig verknüpft. Grundlage: Bildungsplan S. 18 und das lokale offizielle BPE-8-Paket mit drei Lernfortschritten. Cache-Version auf `2.4.1` vereinheitlicht, mobile Befehlsübersichten gegen Überbreite abgesichert und Markdown-, Projekt- sowie Memory-Dokumentation aktualisiert. |

---

## 5. Offene Punkte / To-do

- [ ] **BPE 1 bis BPE 4** schrittweise als vollständige HTML-Lesefassungen ausbauen; mit BPE 1 „Tabellenkalkulation“ beginnen.
- [ ] Kapitel 1: ggf. kleine Weltbilder/Grafiken zu den Übungsaufgaben (Ausgangs-/Ziel-Welt), damit die Aufgaben ohne PythonKara-Datei eindeutig sind.
- [ ] **Anrede vereinheitlichen:** Kapitel 1–6, Spickzettel, Checklisten nutzen „Sie“; die Codex-Seiten (Startseite, Inhaltsverzeichnis, Glossar) nutzen „du“. Jakob entscheiden lassen, dann konsequent umstellen.
- [ ] Optional: Abschlussquiz pro Kapitel (5–8 Fragen) als Klassenarbeits-Simulation.
- [ ] Bei neuen Seiten: Navigation (inzwischen 13 Einträge – bei weiteren Kapiteln über ein Dropdown „Kapitel“ nachdenken), Inhaltsverzeichnis und ggf. Checklisten mitpflegen.

---

## 6. Verifikation (Stand v2.4)

- BPE-8-Check v2.4: alle 13 HTML-Seiten geparst; sämtliche lokalen
  `href`-/`src`-Ziele und Sprungmarken vorhanden; Navigation und Cache-Version
  `2.4.1` auf allen Seiten konsistent. JavaScript-Syntax und `git diff --check`
  fehlerfrei.
- BPE 8 im Browser auf 1440 × 900 und 390 × 844 geprüft: zwei responsive
  Graphmodelle mit 13 Knoten, drei Quizfragen und acht Übungen rendern ohne
  Seitenüberlauf. Quiz-Feedback, 15 Ich-kann-Ziele und Speicherung nach
  Neuladen funktionieren; der Testhaken wurde anschließend zurückgesetzt.
- Glossarblock `#graphbegriffe` mit zwölf Begriffen sowie Spickzettelblock
  `#graphen` mobil geprüft. Befehls-Karten besitzen `min-width: 0`, damit auch
  die SQL-Übersicht auf schmalen Displays innerhalb der Seite bleibt.
- Alle Seiten laden ohne Konsolenfehler und ohne fehlgeschlagene Netzwerk-Requests (getestet über lokalen `http.server`).
- Interaktiv getestet: Quiz-Feedback, Syntax-Highlighting, Checklisten-Speicherung (übersteht Neuladen), Kara-Simulator (Schritt/Abspielen/Zurücksetzen), Struktogramm-Rendering (einfach + verschachtelt), neue Kapitel 4–6 inkl. Quiz und Grafiken (Array-Zellen, Listen-/Stack-/Queue-Diagramme, SVG-Bäume).
- Statischer Link-/Ankercheck: alle lokalen HTML-Ziele und Sprungmarken vorhanden.
- Browsercheck nach v1.6: `index.html` und Kapitel 4–6 auf Desktopbreite sowie mobil (390 × 844) geprüft; keine Konsolenfehler, kein horizontales Seiten-Overflow. Das Startseiten-Symbol `.mini-stg` rendert mit Blauwerten (`#344bb8`) und ohne Rotanteile; die drei neuen Übung-7-Blöcke sind sichtbar.
- Browsercheck nach v1.8: PythonLab-Workbook-Route, Workbook-Startseite, Kapitel 1, Glossar und Spickzettel lokal geprüft; PNG-Favicons und Logo-Bilder laden, SwissEduc-PythonKara-Links sind vorhanden, Desktop-Topnav bleibt einzeilig, Mobilbreite 390 × 844 ohne Seiten-Overflow.
- Browsercheck nach v1.9: Footer der Workbook-Startseite lokal geprüft; Info-Button öffnet die BPE-/Quellenhinweise, Sawazki-Electronics-Link ist sichtbar, Desktop- und Mobilbreite ohne Seiten-Overflow.
- Konsolidierungscheck v2.1: alle 15 fachlichen bzw. technischen Dateien des
  alten `PythonWorkbook`-Bestands gegen das Lehrbuch verglichen. `kara.js` und
  das Interaktionsskript waren bytegleich; HTML, CSS und Dokumentation lagen im
  Lehrbuch als neuere, erweiterte Fassungen vor. Keine fehlende Übung, Grafik,
  Funktion oder Referenz wurde festgestellt.
- Nach der Asset-Umbenennung wurden alle lokalen `href`-/`src`-Ziele, alle
  HTML-Sprungmarken sowie Startseite, Glossar, Checklisten und Kara-Simulator
  erneut geprüft.
- Live-Check am 2026-07-16: Pages-Build erfolgreich; der sichtbare
  PythonLab-Reiter `Lehrbuch` öffnet `https://jakobsawazki.github.io/Lehrbuch/`.
  Titel, Logo und `lehrbuch.js` laden dort ohne Konsolenfehler oder
  horizontalen Seitenüberlauf.

---

## 7. Quellenrollen und Konsolidierung

Das Projekt **Lehrbuch** vereint seit 2026-07-16 die frühere HTML-Workbook-
Lesefassung und die BPE-1-bis-BPE-8-Buchstruktur. Es gibt keinen zweiten
Arbeitsordner und keine zweite kanonische Fassung mehr.

- `README.md` beschreibt Arbeitsprinzip, Zielgruppe und Rolle von Markdown.
- `book.md` entwirft den Gesamtaufbau des Fachbuchs.
- `curriculum-map.md` dokumentiert die Bildungsplan-Abdeckung fuer
  Eingangsklasse, J1 und J2.
- `chapters/` enthaelt Kapiteldateien in Bildungsplan-Reihenfolge:
  `bpe-1-...` bis `bpe-8-...`.
- `exercises/` enthaelt erste Uebungs-Sammeldateien.
- `solutions/README.md` haelt fest, dass Loesungen wegen oeffentlicher
  Veroeffentlichung bewusst getrennt geplant werden sollen.

Der technische Ordnername lautet `Lehrbuch`; der sichtbare Projekttitel lautet
**Lehrbuch**. Die Markdown-Dateien in `chapters/` bilden die BPE-Hauptebene.
Die HTML-Dateien sind die detaillierte Web-Lesefassung und enthalten derzeit
die ausgebauten Bereiche BPE 5 bis BPE 8. Bei einer späteren
Konvertierung nach Word oder PDF wird aus diesen Rollen eine gemeinsame
Ausgabe erzeugt, ohne Inhalte parallel neu zu schreiben.

PythonLab zeigt den Navigationspunkt nun als **Lehrbuch** an und verlinkt auf
`../Lehrbuch/`. Der interne Routename `workbook` bleibt aus
Kompatibilitaetsgruenden zunaechst bestehen.
