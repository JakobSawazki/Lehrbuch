# BPE 6: Relationale Datenbanken

**Stufe:** Jahrgangsstufe 1
**Zeitrichtwert:** 30 Stunden
**Worum es geht:** Daten aus realen Situationen modellieren, in relationalen
Datenbanken speichern und mit SQL auswerten.

## Warum diese BPE wichtig ist

Tabellenkalkulation reicht nicht immer aus. Sobald Daten miteinander
zusammenhaengen, mehrfach genutzt werden und widerspruchsfrei bleiben sollen,
braucht man Datenbanken.

## Lernziele

Nach dieser BPE kannst du:

- reale Situationen analysieren
- Entitaeten, Attribute und Beziehungen erkennen
- Kardinalitaeten beschreiben
- ER-Modelle entwerfen
- Relationenmodelle ableiten
- Primaer- und Fremdschluessel erklaeren
- Redundanz und Normalisierung einordnen
- Daten mit SQL anlegen und auswerten
- Chancen und Risiken von Massendaten diskutieren

## Leitbeispiel: Schulbibliothek

Eine Schulbibliothek verwaltet Buecher, Personen und Ausleihen.

Modellfragen:

- Welche Dinge gibt es?
- Welche Eigenschaften haben sie?
- Welche Beziehungen bestehen zwischen ihnen?
- Welche Daten duerfen nicht doppelt oder widerspruechlich gespeichert werden?

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

Wichtig sind nicht nur SQL-Befehle, sondern auch Begruendungen:

- Warum braucht diese Tabelle einen Primaerschluessel?
- Welche Beziehung liegt vor?
- Wo entsteht Redundanz?
- Welche Auswertung beantwortet eine konkrete Frage?
