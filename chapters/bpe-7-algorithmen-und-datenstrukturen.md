# BPE 7: Algorithmen und Datenstrukturen

**Stufe:** Jahrgangsstufe 2
**Zeitrichtwert:** 30 Stunden
**Worum es geht:** Arrays, Such- und Sortieralgorithmen sowie dynamische
Datenstrukturen verstehen, anwenden und modellieren.

**Rolle dieser Datei:** Übergeordnetes BPE-Kapitel und redaktionelle
Inhaltsquelle. Die bereits ausgearbeiteten Web-Unterkapitel sind
[Arrays](../kapitel-4-arrays.html),
[Sortieren und Suchen](../kapitel-5-sortieren-suchen.html) und
[dynamische Datenstrukturen](../kapitel-6-datenstrukturen.html). Diese Inhalte
werden nicht noch einmal als getrennte Parallelkapitel angelegt.

## Warum diese BPE wichtig ist

In der J2 geht es staerker darum, Programme und Daten nicht nur zu schreiben,
sondern auch strukturiert zu analysieren. Du vergleichst Algorithmen,
beschreibst Datenstrukturen und begruendest, welche Loesung zu welchem Problem
passt.

## Lernziele

Nach dieser BPE kannst du:

- eindimensionale Arrays beziehungsweise Python-Listen verwenden
- per Index auf Werte zugreifen
- Listen mit Schleifen durchlaufen
- typische Array-Algorithmen entwerfen
- Bubble Sort und Selection Sort erklaeren
- lineare und binaere Suche unterscheiden
- verkettete Listen, Stack, Queue und Baum beschreiben
- Datenstrukturen fuer Problemsituationen auswaehlen

## Kapitelweg innerhalb der BPE

### 7.1 Arrays und Listen

Arrays speichern mehrere gleichartige Werte unter einem Namen.

```python
temperaturen = [18, 21, 20, 23, 19]
print(temperaturen[0])
print(len(temperaturen))
```

### 7.2 Sortieren und Suchen

Such- und Sortieralgorithmen zeigen, wie systematische Schrittfolgen Probleme
loesen.

```python
werte = [31, 42, 28, 55]
gesucht = 42

for wert in werte:
    if wert == gesucht:
        print("gefunden")
```

### 7.3 Dynamische Datenstrukturen

Verkettete Listen, Stacks, Queues und Baeume werden beschrieben und modelliert.
Hier steht besonders das Verstehen des Aufbaus im Vordergrund.

## Verbindung zum Abitur

BPE 7 ist fuer Pruefungsaufgaben besonders ergiebig:

- Algorithmen von Hand ausfuehren
- Zwischenstaende notieren
- Schreibtischtests durchfuehren
- Datenstrukturen skizzieren
- Vor- und Nachteile begruenden
- passende Modellierung fuer eine Situation waehlen
