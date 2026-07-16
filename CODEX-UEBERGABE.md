# Übergabe an Codex auf dem Laptop

**Stand:** 2026-07-16 22:20

**Projekt:** Lehrbuch Informatik für das Berufliche Gymnasium Baden-Württemberg

## 1. Hier weiterarbeiten

Das **Lehrbuch** ist die einzige kanonische Quelle für diese Inhalte.

- Desktop-Pfad: `D:\Google Drive\Codex\Lehrbuch`
- Auf dem Laptop: denselben Ordner innerhalb des synchronisierten
  Google-Drive-Verzeichnisses verwenden. Der Laufwerksbuchstabe kann abweichen.
- GitHub: <https://github.com/JakobSawazki/Lehrbuch>
- Live-Seite: <https://jakobsawazki.github.io/Lehrbuch/>
- Branch: `main`

Der frühere Ordner `PythonWorkbook` wurde vollständig in das Lehrbuch
überführt und wird **nicht** mehr verwendet.

## 2. Einstieg auf dem Laptop

```powershell
cd "D:\Google Drive\Codex\Lehrbuch"
git status
git pull --ff-only origin main
```

Falls der Google-Drive-Pfad auf dem Laptop anders lautet, zuerst nach dem
Ordner `Codex\Lehrbuch` suchen und den Befehl entsprechend anpassen.

Danach in dieser Reihenfolge lesen:

1. `CODEX-UEBERGABE.md`
2. `DOKUMENTATION.md`
3. `README.md`
4. `curriculum-map.md`
5. falls über Google Drive vorhanden: `memory/project-context.md`,
   `memory/html-context.md` und `memory/content-map.md`

## 3. Aktueller fachlicher Stand

Die Buchstruktur folgt konsequent **BPE 1 bis BPE 8**.

| Bereich | Stand |
|---|---|
| BPE 1 bis BPE 4 | Markdown-Überblick vorhanden; noch keine vollständigen HTML-Lesekapitel |
| BPE 5 Grundlagen der Programmierung | vollständig in drei HTML-Kapiteln ausgebaut |
| BPE 6 Relationale Datenbanken | vollständige HTML-Lesefassung |
| BPE 7 Algorithmen und Datenstrukturen | vollständig in drei HTML-Kapiteln ausgebaut |
| BPE 8 Gesellschaftliche Aspekte | vollständige HTML-Lesefassung |

BPE 8 enthält aktuell algorithmischen Einfluss, Informationsvorauswahl und
Filterblasen, Graphgrundlagen, ein soziales Netzwerk, gewichtete Wegsuche,
Chancen und Risiken, drei Quizfragen, acht Übungen mit Lösungen und 15
Ich-kann-Ziele.

Wichtige Seiten:

- `index.html`: Startseite und Gesamtübersicht
- `inhaltsverzeichnis.html`: Lernlandkarte
- `bpe-6-relationale-datenbanken.html`: BPE 6
- `bpe-8-gesellschaftliche-aspekte.html`: BPE 8
- `glossar.html`: Fachbegriffe und Befehle
- `referenz.html`: Spickzettel
- `checklisten.html`: interaktive Ich-kann-Checklisten

## 4. Quellen

Die privaten Originalquellen liegen außerhalb des öffentlichen Repositories:

- Bildungsplan:
  `D:\Google Drive\Codex\PythonLab\resources\29-TB02-Inhalt-Band 2a-AG-3 Informatik.pdf`
- BPE 5:
  `D:\Google Drive\Codex\PythonLab\resources\bpe-5-grundlagen-der-programmierung-version-mit-python\bpe-5-gdp_python`
- BPE 7:
  `D:\Google Drive\Codex\PythonLab\resources\bpe-7-algorithmen-datenstrukturen-python`
- BPE 8:
  `D:\Google Drive\Codex\PythonLab\resources\bpe-8-gesellschaftliche-aspekte`

Originalmaterialien, PDFs und Musterlösungen nicht ungeprüft veröffentlichen.
Die Schülerfassung muss eigenständig formuliert bleiben.

## 5. Technischer Rahmen

- reines HTML, CSS und Vanilla JavaScript
- keine Frameworks und keine CDN-Abhängigkeiten
- muss auch offline funktionieren
- zentrales Design: `assets/style.css`
- Interaktionen, Quiz und Checklisten: `assets/lehrbuch.js`
- aktueller Cache-Buster: `?v=2.4.1`
- responsive Prüfung mindestens bei 1440 × 900 und 390 × 844
- private Ordner wie `memory/`, `tmp/`, `resources/` und `ideas.txt` bleiben
  durch `.gitignore` unveröffentlicht

Lokaler Testserver aus `D:\Google Drive\Codex`:

```powershell
python -m http.server 8754
```

Danach öffnen:

`http://127.0.0.1:8754/Lehrbuch/`

## 6. Arbeitsregeln

1. Vor jeder Änderung `git status` und `DOKUMENTATION.md` prüfen.
2. Änderungen anderer Agenten nicht überschreiben oder zurücksetzen.
3. Neue Inhalte genau einer BPE und einer kanonischen Datei zuordnen;
   Doppelkapitel vermeiden.
4. Bei neuen HTML-Seiten Navigation, Startseite, Inhaltsverzeichnis,
   Glossar, Referenz und Checklisten mitprüfen.
5. `DOKUMENTATION.md` mit Datum, Uhrzeit, Autor und Änderung ergänzen.
6. Private Memory-Dateien aktualisieren, falls sie auf dem Laptop synchronisiert
   sind.
7. Vor dem Push Links, Anker, JavaScript und Desktop-/Mobilansicht testen.

Mindestens ausführen:

```powershell
node --check assets/lehrbuch.js
node --check assets/kara.js
git diff --check
```

## 7. Nächster sinnvoller Ausbau

Als nächster großer Schritt bietet sich **BPE 1 Tabellenkalkulation** als
vollständige HTML-Lesefassung an. Danach können BPE 2 bis BPE 4 folgen.
Alternativ kann zunächst ein gemischtes Abiturtraining für J1/J2 entstehen.

Vor einer größeren neuen Einheit zuerst den Bildungsplan und vorhandene lokale
Materialordner sichten. Die bestehende visuelle Sprache des Lehrbuchs soll
beibehalten werden: anschauliche Beispiele, ruhige Typografie, klare Grafiken,
Übungen, Lösungen und Selbstchecks.

## 8. Letzter veröffentlichter Inhaltsstand

- `3fc3b07` – BPE 6 und BPE 8 vervollständigt
- `50ce38c` – Veröffentlichung von BPE 8 dokumentiert
- GitHub Pages wurde nach beiden Commits erfolgreich geprüft.
