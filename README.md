# Geoguesser Sprintplan

Timeline mit allen Issues des HTL-Geoguesser-Projekts (4AHITM, HTL Villach): 6 Sprints vom 05.10. bis 21.12.2026, Abhängigkeiten, „Ohne zu warten“-Hinweise und Acceptance Criteria – zum Abhaken für alle drei Teammitglieder.

## Öffnen

- **Online:** https://motitschka.github.io/issues/
- **Lokal:** `index.html` im Browser öffnen. Es wird nichts installiert.

## Issues erstellen

Issues werden erst kurz vor der Arbeit angelegt. **Issue erstellen** öffnet in GitLab ein neues Issue mit Titel, Beschreibung, Abhängigkeiten und Acceptance Criteria. Die Quick Actions am Ende der Beschreibung setzen beim Speichern Label, Sprint-Milestone und Weight und weisen das Issue dir zu (`/assign me`).

- **Schon erstellt? In GitLab suchen** prüft vorher, ob es das Issue bereits gibt.
- **Titel und Beschreibung kopieren** ist der Ausweg, falls GitLab die Felder nicht vorausfüllt.

## Häkchen

- Werden im Browser gespeichert (`localStorage`), also pro Person und Gerät.
- **Stand teilen** kopiert einen Link mit deinem Fortschritt. Wer ihn öffnet, kann ihn mit dem eigenen Stand **zusammenführen** oder ihn **ersetzen**.
- **Zurücksetzen** löscht alle Häkchen in diesem Browser.

## Inhalt ändern

Die Issues stehen als JSON direkt in `index.html` (`<script id="issues-data">`). Pro Issue: `id`, Person (`L`, `D`, `M`), Label, Weight (`w`), Sprint (`s`), Titel (`t`), Abhängigkeiten (`deps`, als IDs), Hinweis (`how`) und Acceptance Criteria (`ac`). Häkchen hängen an der `id` – beim Umbenennen eines Titels bleiben sie erhalten, beim Ändern der `id` nicht.
