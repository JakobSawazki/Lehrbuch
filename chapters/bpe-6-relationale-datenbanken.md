# BPE 6: Relationale Datenbanken

**Stufe:** Jahrgangsstufe 1
**Zeitrichtwert:** 30 Stunden
**Worum es geht:** Daten aus realen Situationen modellieren, in relationalen
Datenbanken speichern und mit SQL auswerten.

**Rolle dieser Datei:** BPE-Überblick und redaktionelle Quelle. Die vollständige
Web-Lesefassung mit Grafiken, Quizfragen, Übungen und Lösungen liegt unter
[`bpe-6-relationale-datenbanken.html`](../bpe-6-relationale-datenbanken.html).

## Warum diese BPE wichtig ist

Tabellenkalkulation reicht nicht immer aus. Sobald Daten miteinander
zusammenhängen, mehrfach genutzt werden und widerspruchsfrei bleiben sollen,
braucht man Datenbanken.

## Lernziele

Nach dieser BPE kannst du:

- reale Situationen analysieren
- Entitäten, Attribute und Beziehungen erkennen
- Kardinalitäten beschreiben
- ER-Modelle entwerfen
- Relationenmodelle ableiten
- Primär- und Fremdschlüssel erklären
- Redundanz und Normalisierung einordnen
- Daten mit SQL anlegen und auswerten
- Chancen und Risiken von Massendaten diskutieren

## Leitbeispiel: Schulbibliothek

Eine Schulbibliothek verwaltet Bücher, Personen und Ausleihen.

Modellfragen:

- Welche Dinge gibt es?
- Welche Eigenschaften haben sie?
- Welche Beziehungen bestehen zwischen ihnen?
- Welche Daten dürfen nicht doppelt oder widersprüchlich gespeichert werden?

## SQL als Werkzeug

Typische Befehle:

```sql
CREATE TABLE buch (
  buch_id INTEGER PRIMARY KEY,
  titel TEXT
);

INSERT INTO buch VALUES (1, 'Python verstehen');

SELECT titel
FROM buch
ORDER BY titel;
```

## Verbindung zum Abitur

Wichtig sind nicht nur SQL-Befehle, sondern auch Begründungen:

- Warum braucht diese Tabelle einen Primärschlüssel?
- Welche Beziehung liegt vor?
- Wo entsteht Redundanz?
- Welche Auswertung beantwortet eine konkrete Frage?

## Weiterarbeiten

- [HTML-Lesefassung öffnen](../bpe-6-relationale-datenbanken.html)
- [SQL-Spickzettel](../referenz.html#sql)
- [Ich-kann-Checkliste](../checklisten.html#bpe6)
- [Redaktionelle Übungsübersicht](../exercises/bpe6-uebungen.md)
