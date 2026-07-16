# BPE 5: Grundlagen der Programmierung

**Stufe:** Jahrgangsstufe 1
**Zeitrichtwert:** 20 Stunden
**Worum es geht:** Einfache Programme planen, implementieren, testen und mit
Struktogrammen dokumentieren.

**Rolle dieser Datei:** Übergeordnetes BPE-Kapitel und redaktionelle
Inhaltsquelle. Die bereits ausgearbeiteten Web-Unterkapitel sind
[Kara und Struktogramme](../kapitel-1-kara.html),
[Python-Grundlagen](../kapitel-2-python-grundlagen.html) und
[Kontrollstrukturen](../kapitel-3-kontrollstrukturen.html). Diese Inhalte
werden nicht noch einmal als getrennte Parallelkapitel angelegt.

## Warum diese BPE wichtig ist

Diese BPE ist der Einstieg in das eigentliche Programmieren. Du lernst, wie ein
Programm Daten entgegennimmt, verarbeitet und wieder ausgibt. Aus einzelnen
Anweisungen werden nachvollziehbare Ablaeufe.

## Lernziele

Nach dieser BPE kannst du:

- Variablen verwenden
- Werte zuweisen, auslesen und berechnen
- Eingabe, Verarbeitung und Ausgabe unterscheiden
- eigene Funktionen oder Unterprogramme nutzen
- einseitige und zweiseitige Alternativen programmieren
- logische Operatoren verwenden
- `for`- und `while`-Schleifen unterscheiden
- Struktogramme als Entwurf und Dokumentation einsetzen

## Kapitelweg innerhalb der BPE

### 5.1 Kara als Einstieg

Kara macht Programmablauf sichtbar. Du siehst, wie ein Befehl nach dem anderen
ausgefuehrt wird, und erkennst Bedingungen und Wiederholungen direkt in einer
kleinen Welt.

```python
if kara.onLeaf():
    kara.removeLeaf()
else:
    kara.move()
```

### 5.2 Python-Grundlagen

Python verarbeitet Eingaben, speichert Werte in Variablen und gibt Ergebnisse
aus.

```python
laenge = float(input("Laenge: "))
breite = float(input("Breite: "))
flaeche = laenge * breite
print("Flaeche:", flaeche)
```

### 5.3 Kontrollstrukturen

Kontrollstrukturen entscheiden, welche Anweisungen ausgefuehrt werden und wie
oft sie ausgefuehrt werden.

```python
alter = int(input("Alter: "))

if alter < 14:
    preis = 4
else:
    preis = 8
```

## Denkwerkzeug: EVA

| Schritt | Frage | Beispiel |
|---|---|---|
| Eingabe | Welche Daten brauche ich? | Alter, Laenge, Breite |
| Verarbeitung | Was wird berechnet oder entschieden? | Preis, Flaeche |
| Ausgabe | Was soll sichtbar werden? | Ergebnistext |

## Verbindung zum Abitur

BPE 5 liefert die Sprache, in der spaetere Aufgaben geloest werden. Besonders
wichtig sind:

- Code lesen
- Ablaufe mit Schreibtischtest nachvollziehen
- Bedingungen sauber formulieren
- Schleifen sicher begruenden
- Struktogramme in Code uebertragen und umgekehrt
