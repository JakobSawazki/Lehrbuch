# Bildungsplan-Abdeckung

Quelle:

`D:\Google Drive\Codex\PythonLab\resources\29-TB02-Inhalt-Band 2a-AG-3 Informatik.pdf`

Stand dieser Karte: 2026-07-07.

Diese Datei ist die fachliche Landkarte fuer das Lehrbuch. Sie zeigt,
welche Bildungsplaneinheiten im Lehrbuch vorkommen sollen und welche davon
zuerst ausgearbeitet werden.

## Gesamtueberblick

| Stufe | BPE | Thema | Zeitrichtwert | Status im Lehrbuch |
|---|---:|---|---:|---|
| Eingangsklasse | 1 | Tabellenkalkulation | 16 h | Ueberblick vorgesehen |
| Eingangsklasse | 2 | Entwicklung von Internetseiten | 14 h | Ueberblick vorgesehen |
| Eingangsklasse | 3 | Netze und vernetzte Gesellschaft | 14 h | Ueberblick vorgesehen |
| Eingangsklasse | 4 | Darstellung von Informationen | 6 h | Ueberblick vorgesehen |
| J1 | 5 | Grundlagen der Programmierung | 20 h | zuerst ausbauen |
| J1 | 6 | Relationale Datenbanken | 30 h | danach ausbauen |
| J2 | 7 | Algorithmen und Datenstrukturen | 30 h | danach ausbauen |
| J2 | 8 | Gesellschaftliche Aspekte | 10 h | danach ausbauen |

## Kapiteldateien

| BPE | Kapiteldatei | Kurzrolle |
|---:|---|---|
| 1 | `chapters/bpe-1-tabellenkalkulation.md` | Daten in Tabellen verstehen |
| 2 | `chapters/bpe-2-entwicklung-von-internetseiten.md` | Struktur und Gestaltung im Web |
| 3 | `chapters/bpe-3-netze-und-vernetzte-gesellschaft.md` | Kommunikation, Sicherheit, Gesellschaft |
| 4 | `chapters/bpe-4-darstellung-von-informationen.md` | Codierung und Datenrepraesentation |
| 5 | `chapters/bpe-5-grundlagen-der-programmierung.md` | Python, EVA, Struktogramme, Kontrollstrukturen |
| 6 | `chapters/bpe-6-relationale-datenbanken.md` | ER-Modell, Relationenmodell, SQL |
| 7 | `chapters/bpe-7-algorithmen-und-datenstrukturen.md` | Arrays, Suchen, Sortieren, dynamische Strukturen |
| 8 | `chapters/bpe-8-gesellschaftliche-aspekte.md` | Algorithmen im Alltag, Graphen, Bewertung |

## Eingangsklasse als Fundament

Die Eingangsklasse wird im Lehrbuch zunaechst als kompakte Orientierung
aufgenommen. Sie ist wichtig, weil spaetere Themen darauf aufbauen, aber der
erste Schwerpunkt des Projekts liegt auf J1 und J2.

### BPE 1: Tabellenkalkulation

Kernideen:

- Daten eingeben, formatieren und auswerten
- Formeln und Funktionen nutzen
- relative und absolute Zellbezuege verstehen
- einfache und geschachtelte Bedingungen nutzen
- Diagramme passend zum Datentyp waehlen

Moegliche Lehrbuchrolle:

- Vorkapitel "Daten in Tabellen verstehen"
- Bruecke zu Arrays: Werte stehen an Positionen, Formeln verarbeiten Daten
- Bruecke zu Datenbanken: Tabellen sind hilfreich, aber nicht immer genug

### BPE 2: Entwicklung von Internetseiten

Kernideen:

- HTML-Struktur
- CSS-Gestaltung
- Pfade, Dateinamen und Medien
- rechtliche Grundlagen beim Veroeffentlichen
- lokaler Server oder Upload

Moegliche Lehrbuchrolle:

- optionales Projektkapitel
- Verbindung zu PythonLab und statischen Webseiten
- spaeter gute Grundlage fuer kleine Web-Interfaces zu Python-Projekten

### BPE 3: Netze und vernetzte Gesellschaft

Kernideen:

- Client-Server-Prinzip
- Datenpakete, Adressen und Routing
- Netzwerkkomponenten
- Cloud, Datensicherheit und Verschluesselung
- Datenschutz, Privatsphaere und Suchmaschinen

Moegliche Lehrbuchrolle:

- Kontextkapitel fuer Daten, Sicherheit und gesellschaftliche Verantwortung
- Bruecke zu BPE 8

### BPE 4: Darstellung von Informationen

Kernideen:

- Dezimal-, Binaer- und Hexadezimalsystem
- Bit und Byte
- ASCII und Codierung
- Aufbau und Manipulation von Medieninhalten

Moegliche Lehrbuchrolle:

- Fundament fuer Variablen, Datentypen, Zeichenketten und Bilder
- kurze Wiederholungsboxen in spaeteren Kapiteln

## Jahrgangsstufe 1

### BPE 5: Grundlagen der Programmierung

Zielrichtung:

- einfache Programme planen, implementieren und testen
- Programme mit Struktogrammen dokumentieren
- Variablen, Eingabe, Verarbeitung und Ausgabe nutzen
- Unterprogramme einsetzen
- Alternativen und Wiederholungen verstehen

Geplantes Lehrbuchkapitel:

- `chapters/bpe-5-grundlagen-der-programmierung.md`

Ausbauprioritaet: hoch.

### BPE 6: Relationale Datenbanken

Zielrichtung:

- Situationen der realen Welt analysieren
- Datenmodelle entwickeln
- ER-Modelle in Relationenmodelle ueberfuehren
- relationale Datenbanken mit mehreren Tabellen anlegen
- SQL zur Erfassung und Auswertung nutzen
- Chancen und Risiken von Massendaten diskutieren

Geplantes Lehrbuchkapitel:

- `chapters/bpe-6-relationale-datenbanken.md`

Ausbauprioritaet: mittel bis hoch, weil BPE 6 in J1 einen grossen Umfang hat.

## Jahrgangsstufe 2

### BPE 7: Algorithmen und Datenstrukturen

Zielrichtung:

- Arrays beschreiben und implementieren
- Such- und Sortieralgorithmen verstehen, anwenden und implementieren
- dynamische Datenstrukturen beschreiben und modellieren
- passende Datenstrukturen fuer Problemstellungen auswaehlen

Geplantes Lehrbuchkapitel:

- `chapters/bpe-7-algorithmen-und-datenstrukturen.md`

Ausbauprioritaet: hoch, weil J2 die Abschlussklasse vor dem Abitur ist.

### BPE 8: Gesellschaftliche Aspekte

Zielrichtung:

- algorithmische Einfluesse im Alltag identifizieren
- Graphen als Modell fuer lebensnahe Situationen nutzen
- Chancen und Risiken algorithmischer Systeme beurteilen

Geplantes Lehrbuchkapitel:

- `chapters/bpe-8-gesellschaftliche-aspekte.md`

Ausbauprioritaet: mittel. Inhaltlich passt BPE 8 sehr gut als Abschluss, weil
sie technische und gesellschaftliche Perspektiven verbindet.
