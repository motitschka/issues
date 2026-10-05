# Geoguesser Sprintplan

Timeline mit allen 45 Issues des HTL-Geoguesser-Projekts (4AHITM, HTL Villach): 6 Sprints vom 05.10. bis 21.12.2026, Abhängigkeiten, „Ohne zu warten“-Hinweise und Acceptance Criteria – zum Abhaken für alle drei Teammitglieder.

## Öffnen

- **Lokal:** `index.html` im Browser öffnen. Es wird nichts installiert.
- **Online:** unter *Settings → Pages* „Deploy from a branch“, Branch `main`, Ordner `/ (root)` wählen. GitHub Pages für private Repositories braucht GitHub Pro (für Schüler gratis über das GitHub Student Developer Pack).

## Häkchen

- Werden im Browser gespeichert (`localStorage`), also pro Person und Gerät.
- **Stand teilen** kopiert einen Link mit deinem Fortschritt. Wer ihn öffnet, kann ihn mit dem eigenen Stand **zusammenführen** oder ihn **ersetzen**.
- **Zurücksetzen** löscht alle Häkchen in diesem Browser.

## Inhalt ändern

Die Issues stehen als JSON direkt in `index.html` (`<script id="issues-data">`). Pro Issue: `id`, Person (`L`, `D`, `M`), Label, Weight (`w`), Sprint (`s`), Titel (`t`), Abhängigkeiten (`deps`, als IDs), Hinweis (`how`) und Acceptance Criteria (`ac`). Häkchen hängen an der `id` – beim Umbenennen eines Titels bleiben sie erhalten, beim Ändern der `id` nicht.
