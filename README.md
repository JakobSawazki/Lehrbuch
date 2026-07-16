# Lehrbuch

Dieses Verzeichnis ist die Arbeitsquelle für ein schülerfreundliches
Informatik-Lehrbuch für das Berufliche Gymnasium Baden-Württemberg.

Es deckt langfristig alle Bildungsplaneinheiten BPE 1 bis BPE 8 ab:
Tabellenkalkulation, Webseiten, Netze, Informationsdarstellung,
Programmierung mit Python, relationale Datenbanken, Algorithmen,
Datenstrukturen und gesellschaftliche Aspekte.

Der technische Projektordner lautet `Lehrbuch`. Der sichtbare Projekttitel
lautet **Lehrbuch**.

## Arbeitsprinzip

- **Das Lehrbuch ist die einzige Projektquelle.** Der frühere Stand unter
  `D:\Google Drive\Codex\PythonWorkbook` wurde vollständig abgeglichen und am
  2026-07-16 in dieses Projekt konsolidiert.
- **Die acht BPE-Dateien bilden die Buchgliederung.** In `chapters/` liegt für
  jede Bildungsplaneinheit genau ein übergeordnetes Kapitel.
- **Die HTML-Lesefassung ist die ausgearbeitete Web-Ausgabe.** Acht
  HTML-Lektionen vertiefen derzeit BPE 5 bis BPE 8. Die Kapitel 1 bis 6 sind
  Unterkapitel zu BPE 5 und BPE 7; BPE 6 und BPE 8 besitzen jeweils eine
  zusammenhängende HTML-Lesefassung. Die Markdown-Dateien bleiben die
  übergeordnete BPE-Quelle.
- **Neue Fachinhalte werden zuerst der passenden BPE zugeordnet.** Danach wird
  entschieden, ob sie als Markdown-Quelltext, HTML-Lektion oder Übung
  umgesetzt werden. Eine parallele Kopie desselben Kapitels wird vermieden.
- **Word und PDF sind Ausgabeformate.** Sie werden später aus dem konsolidierten
  Lehrbuchbestand erzeugt.
- **Lösungen werden vorsichtig behandelt.** Öffentliche Schülerfassung und
  private Lehrkraftfassung sollten getrennt geplant werden.

## Einstieg für Autorinnen und Autoren

1. `book.md` lesen.
2. `curriculum-map.md` lesen.
3. Danach das passende Kapitel in `chapters/` bearbeiten.
4. Neue Aufgaben in `exercises/` sammeln.
5. Lösungen nur bewusst und mit Blick auf die Veröffentlichung in
   `solutions/` ergänzen.

## Kapitelstruktur

Die Kapitel folgen konsequent den Bildungsplaneinheiten:

- `chapters/bpe-1-tabellenkalkulation.md`
- `chapters/bpe-2-entwicklung-von-internetseiten.md`
- `chapters/bpe-3-netze-und-vernetzte-gesellschaft.md`
- `chapters/bpe-4-darstellung-von-informationen.md`
- `chapters/bpe-5-grundlagen-der-programmierung.md`
- `chapters/bpe-6-relationale-datenbanken.md`
- `chapters/bpe-7-algorithmen-und-datenstrukturen.md`
- `chapters/bpe-8-gesellschaftliche-aspekte.md`

Jede BPE-Datei nennt oben kurz Stufe, Zeitrichtwert und fachlichen Kern, damit
beim Lesen immer klar ist, wo man sich im Bildungsplan befindet.

## Zielgruppe

Schülerinnen und Schüler der Eingangsklasse, Jahrgangsstufe 1 und
Jahrgangsstufe 2 am Beruflichen Gymnasium. Der Schwerpunkt der ersten
Ausbaustufe liegt auf **J1 und J2**, weil dort Programmierung,
Datenbanken, Algorithmen und Datenstrukturen zentral sind.

## Projektort

Dieses Lehrbuch ist seit 2026-07-07 ein eigenständiges Projekt und seit
2026-07-16 zugleich der alleinige Nachfolger des früheren Python-Workbooks:

`D:\Google Drive\Codex\Lehrbuch`

## Online

- GitHub: <https://github.com/JakobSawazki/Lehrbuch>
- Web-Ausgabe: <https://jakobsawazki.github.io/Lehrbuch/>

PythonLab und andere Projekte können später darauf verlinken oder Inhalte
daraus ableiten, aber die kanonische Quelle liegt hier.
