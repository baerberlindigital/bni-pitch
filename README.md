# Berlin Bär Pitch

Pitch-Anzeige für das Wochenmeeting: Handy-Liste und Beamer-Ansicht mit Modus-Auswahl und Bär der Woche.

## Dateien
- `beamer.html`: Beamer-Ansicht (16:9) mit Auswahlseite, Timer, Presenter-Steuerung
- `pitch.html`: Handy-Liste
- `index.html`: Startseite mit Links zu beiden
- `apps-script/code.gs`: komplettes Skript für das Google Sheet (ersetzt den bisherigen Inhalt)

## Einrichten
1. `apps-script/code.gs` in das Apps-Script-Projekt kopieren, unter "Bereitstellungen verwalten" eine neue Version bereitstellen.
2. Die `/exec`-URL der Web-App ist in `beamer.html` und `pitch.html` bereits eingetragen (bei neuer Bereitstellung mit neuer URL dort anpassen).
3. GitHub Pages aktivieren (Settings, Pages, Branch `main`, Ordner `/ (root)`).

Alternativ lassen sich beide Seiten direkt über die Web-App aufrufen: `<exec-URL>?seite=beamer` und `<exec-URL>?seite=pitch`.

## Modi
- A: Jeder Bär stellt den vorher eingecheckten Bären vor
- B: Jeder Bär stellt den danach eingecheckten Bären vor
- C: Zufällige Reihenfolge der Bären und Vertretungen

Der Bär der Woche hat 60 statt 30 Sekunden.
