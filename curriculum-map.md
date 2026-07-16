# Bildungsplan-Abdeckung

Quelle:

`D:\Google Drive\Codex\PythonLab\resources\29-TB02-Inhalt-Band 2a-AG-3 Informatik.pdf`

Stand dieser Karte: 2026-07-16.

Diese Datei ist die fachliche Landkarte für das Lehrbuch. Sie zeigt,
welche Bildungsplaneinheiten im Lehrbuch vorkommen sollen und welche davon
zuerst ausgearbeitet werden.

## Gesamtüberblick

| Stufe | BPE | Thema | Zeitrichtwert | Status im Lehrbuch |
|---|---:|---|---:|---|
| Eingangsklasse | 1 | Tabellenkalkulation | 16 h | Überblick vorgesehen |
| Eingangsklasse | 2 | Entwicklung von Internetseiten | 14 h | Überblick vorgesehen |
| Eingangsklasse | 3 | Netze und vernetzte Gesellschaft | 14 h | Überblick vorgesehen |
| Eingangsklasse | 4 | Darstellung von Informationen | 6 h | Überblick vorgesehen |
| J1 | 5 | Grundlagen der Programmierung | 20 h | HTML-Lesefassung ausgebaut |
| J1 | 6 | Relationale Datenbanken | 30 h | HTML-Lesefassung ausgebaut |
| J2 | 7 | Algorithmen und Datenstrukturen | 30 h | HTML-Lesefassung ausgebaut |
| J2 | 8 | Gesellschaftliche Aspekte | 10 h | HTML-Lesefassung ausgebaut |

## Kapiteldateien

| BPE | Kapiteldatei | Kurzrolle |
|---:|---|---|
| 1 | `chapters/bpe-1-tabellenkalkulation.md` | Daten in Tabellen verstehen |
| 2 | `chapters/bpe-2-entwicklung-von-internetseiten.md` | Struktur und Gestaltung im Web |
| 3 | `chapters/bpe-3-netze-und-vernetzte-gesellschaft.md` | Kommunikation, Sicherheit, Gesellschaft |
| 4 | `chapters/bpe-4-darstellung-von-informationen.md` | Codierung und Datenrepräsentation |
| 5 | `chapters/bpe-5-grundlagen-der-programmierung.md` | Python, EVA, Struktogramme, Kontrollstrukturen |
| 6 | `chapters/bpe-6-relationale-datenbanken.md` | ER-Modell, Relationenmodell, SQL |
| 7 | `chapters/bpe-7-algorithmen-und-datenstrukturen.md` | Arrays, Suchen, Sortieren, dynamische Strukturen |
| 8 | `chapters/bpe-8-gesellschaftliche-aspekte.md` | Algorithmen im Alltag, Graphen, Bewertung |

## Eingangsklasse als Fundament

Die Eingangsklasse wird im Lehrbuch zunächst als kompakte Orientierung
aufgenommen. Sie ist wichtig, weil spätere Themen darauf aufbauen, aber der
erste Schwerpunkt des Projekts liegt auf J1 und J2.

### BPE 1: Tabellenkalkulation

Kernideen:

- Daten eingeben, formatieren und auswerten
- Formeln und Funktionen nutzen
- relative und absolute Zellbezüge verstehen
- einfache und geschachtelte Bedingungen nutzen
- Diagramme passend zum Datentyp wählen

Mögliche Lehrbuchrolle:

- Vorkapitel "Daten in Tabellen verstehen"
- Brücke zu Arrays: Werte stehen an Positionen, Formeln verarbeiten Daten
- Brücke zu Datenbanken: Tabellen sind hilfreich, aber nicht immer genug

### BPE 2: Entwicklung von Internetseiten

Kernideen:

- HTML-Struktur
- CSS-Gestaltung
- Pfade, Dateinamen und Medien
- rechtliche Grundlagen beim Veröffentlichen
- lokaler Server oder Upload

Mögliche Lehrbuchrolle:

- optionales Projektkapitel
- Verbindung zu PythonLab und statischen Webseiten
- später gute Grundlage für kleine Web-Interfaces zu Python-Projekten

### BPE 3: Netze und vernetzte Gesellschaft

Kernideen:

- Client-Server-Prinzip
- Datenpakete, Adressen und Routing
- Netzwerkkomponenten
- Cloud, Datensicherheit und Verschlüsselung
- Datenschutz, Privatsphäre und Suchmaschinen

Mögliche Lehrbuchrolle:

- Kontextkapitel für Daten, Sicherheit und gesellschaftliche Verantwortung
- Brücke zu BPE 8

### BPE 4: Darstellung von Informationen

Kernideen:

- Dezimal-, Binär- und Hexadezimalsystem
- Bit und Byte
- ASCII und Codierung
- Aufbau und Manipulation von Medieninhalten

Mögliche Lehrbuchrolle:

- Fundament für Variablen, Datentypen, Zeichenketten und Bilder
- kurze Wiederholungsboxen in späteren Kapiteln

## Jahrgangsstufe 1

### BPE 5: Grundlagen der Programmierung

Zielrichtung:

- einfache Programme planen, implementieren und testen
- Programme mit Struktogrammen dokumentieren
- Variablen, Eingabe, Verarbeitung und Ausgabe nutzen
- Unterprogramme einsetzen
- Alternativen und Wiederholungen verstehen

Lehrbuchkapitel:

- `chapters/bpe-5-grundlagen-der-programmierung.md`

Ausbaupriorität: hoch.

### BPE 6: Relationale Datenbanken

Zielrichtung:

- Situationen der realen Welt analysieren
- Datenmodelle entwickeln
- ER-Modelle in Relationenmodelle überführen
- relationale Datenbanken mit mehreren Tabellen anlegen
- SQL zur Erfassung und Auswertung nutzen
- Chancen und Risiken von Massendaten diskutieren

Geplantes Lehrbuchkapitel:

- `chapters/bpe-6-relationale-datenbanken.md`

Status: vollständige HTML-Lesefassung mit ER-Modell, Relationenmodell,
Normalisierung, SQL, Massendaten, Übungen, Lösungen und Checkliste.

## Jahrgangsstufe 2

### BPE 7: Algorithmen und Datenstrukturen

Zielrichtung:

- Arrays beschreiben und implementieren
- Such- und Sortieralgorithmen verstehen, anwenden und implementieren
- dynamische Datenstrukturen beschreiben und modellieren
- passende Datenstrukturen für Problemstellungen auswählen

Geplantes Lehrbuchkapitel:

- `chapters/bpe-7-algorithmen-und-datenstrukturen.md`

Ausbaupriorität: hoch, weil J2 die Abschlussklasse vor dem Abitur ist.

### BPE 8: Gesellschaftliche Aspekte

Zielrichtung:

- algorithmische Einflüsse im Alltag identifizieren
- Graphen als Modell für lebensnahe Situationen nutzen
- Chancen und Risiken algorithmischer Systeme beurteilen

Lehrbuchkapitel:

- `chapters/bpe-8-gesellschaftliche-aspekte.md`
- `bpe-8-gesellschaftliche-aspekte.html`

Status: vollständige HTML-Lesefassung zu BPE 8.1 bis 8.3 mit algorithmischem
Einfluss im Alltag, Informationsvorauswahl und Filterblase, Graphbegriffen,
sozialem Netzwerk, gewichteter Wegsuche, Beurteilungsraster, Übungen,
Lösungen, Quizfragen und Ich-kann-Checkliste. Grundlage sind Bildungsplan
Seite 18 und das lokale offizielle BPE-8-Materialpaket mit drei
Lernfortschritten.
