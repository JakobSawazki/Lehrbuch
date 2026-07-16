# Lehrbuch

Dieses Verzeichnis ist die Arbeitsquelle fuer ein schuelerfreundliches
Informatik-Lehrbuch fuer das Berufliche Gymnasium Baden-Wuerttemberg.

Es deckt langfristig alle Bildungsplaneinheiten BPE 1 bis BPE 8 ab:
Tabellenkalkulation, Webseiten, Netze, Informationsdarstellung,
Programmierung mit Python, relationale Datenbanken, Algorithmen,
Datenstrukturen und gesellschaftliche Aspekte.

Der technische Projektordner lautet `Lehrbuch`. Der sichtbare Projekttitel
lautet **Lehrbuch**.

## Arbeitsprinzip

- **Das Lehrbuch ist die einzige Projektquelle.** Der fruehere Stand unter
  `D:\Google Drive\Codex\PythonWorkbook` wurde vollstaendig abgeglichen und am
  2026-07-16 in dieses Projekt konsolidiert.
- **Die acht BPE-Dateien bilden die Buchgliederung.** In `chapters/` liegt fuer
  jede Bildungsplaneinheit genau ein uebergeordnetes Kapitel.
- **Die HTML-Lesefassung ist die ausgearbeitete Web-Ausgabe.** Die sechs
  HTML-Lektionen vertiefen derzeit BPE 5 und BPE 7. Sie sind Unterkapitel der
  jeweiligen BPE und keine zweite BPE-Gliederung.
- **Neue Fachinhalte werden zuerst der passenden BPE zugeordnet.** Danach wird
  entschieden, ob sie als Markdown-Quelltext, HTML-Lektion oder Uebung
  umgesetzt werden. Eine parallele Kopie desselben Kapitels wird vermieden.
- **Word und PDF sind Ausgabeformate.** Sie werden spaeter aus dem konsolidierten
  Lehrbuchbestand erzeugt.
- **Loesungen werden vorsichtig behandelt.** Oeffentliche Schuelerfassung und
  private Lehrkraftfassung sollten getrennt geplant werden.

## Einstieg fuer Autorinnen und Autoren

1. `book.md` lesen.
2. `curriculum-map.md` lesen.
3. Danach das passende Kapitel in `chapters/` bearbeiten.
4. Neue Aufgaben in `exercises/` sammeln.
5. Loesungen nur bewusst und mit Blick auf die Veroeffentlichung in
   `solutions/` ergaenzen.

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

Schuelerinnen und Schueler der Eingangsklasse, Jahrgangsstufe 1 und
Jahrgangsstufe 2 am Beruflichen Gymnasium. Der Schwerpunkt der ersten
Ausbaustufe liegt auf **J1 und J2**, weil dort Programmierung,
Datenbanken, Algorithmen und Datenstrukturen zentral sind.

## Projektort

Dieses Lehrbuch ist seit 2026-07-07 ein eigenstaendiges Projekt und seit
2026-07-16 zugleich der alleinige Nachfolger des frueheren Python-Workbooks:

`D:\Google Drive\Codex\Lehrbuch`

## Online

- GitHub: <https://github.com/JakobSawazki/Lehrbuch>
- Web-Ausgabe: <https://jakobsawazki.github.io/Lehrbuch/>

PythonLab und andere Projekte koennen spaeter darauf verlinken oder Inhalte
daraus ableiten, aber die kanonische Quelle liegt hier.
