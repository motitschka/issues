# Geoguesser Sprintplan

Timeline mit allen Issues des HTL-Geoguesser-Projekts (4AHITM, HTL Villach): 3 Sprints vom 28.09. bis 21.12.2026 (Abgaben 09.11., 30.11. und 21.12.), Abhängigkeiten, „Ohne zu warten“-Hinweise und Acceptance Criteria – zum Abhaken für alle drei Teammitglieder.

## Öffnen

- **Online:** https://motitschka.github.io/issues/
- **Lokal:** `index.html` im Browser öffnen. Es wird nichts installiert.

## Issues erstellen

Issues werden erst kurz vor der Arbeit angelegt. **Issue erstellen** öffnet in GitLab ein neues Issue mit Titel, Beschreibung, Abhängigkeiten und Acceptance Criteria. Die Quick Actions am Ende der Beschreibung setzen beim Speichern Label, Sprint-Milestone und Weight und weisen das Issue dir zu (`/assign me`).

- **Schon erstellt? In GitLab suchen** prüft vorher, ob es das Issue bereits gibt.
- **Titel und Beschreibung kopieren** ist der Ausweg, falls GitLab die Felder nicht vorausfüllt.

## Häkchen = GitLab-Issues

Die Häkchen werden nicht im Browser gespeichert, sondern direkt in GitLab:

- **Abhaken** schließt das passende GitLab-Issue (Zuordnung über den Titel), **Entfernen** öffnet es wieder. Ist niemand zugewiesen, wirst du beim Abhaken zugewiesen.
- Die Seite zeigt, **wer was erledigt hat** (Assignee, sonst wer geschlossen hat), und zählt das pro Person auf den Team-Karten.
- **Acceptance Criteria** kommen aus der Checkliste im Issue; Abhaken ändert die Beschreibung in GitLab.
- Wird ein Issue über einen Merge Request mit `Closes #…` geschlossen, erscheint es hier automatisch als erledigt. Die Seite aktualisiert sich jede Minute.
- Gibt es mehrere Issues mit demselben Titel, zählt das neueste.

**Verbinden:** Jede Person erstellt einmal einen eigenen [Personal Access Token](https://gitlab.com/-/user_settings/personal_access_tokens?name=Geoguesser%20Sprintplan&scopes=api) mit Scope `api` und Ablaufdatum spätestens 21.12.2026 und fügt ihn auf der Seite ein. Der Token bleibt im Browser und geht nur an gitlab.com; „Trennen“ löscht ihn. Ohne Token zeigt die Seite nur den Plan.

## Inhalt ändern

Die Issues stehen als JSON direkt in `index.html` (`<script id="issues-data">`). Pro Issue: `id`, Person (`L`, `D`, `M`), Label, Weight (`w`), Sprint (`s`), Titel (`t`), Abhängigkeiten (`deps`, als IDs), Hinweis (`how`) und Acceptance Criteria (`ac`). Häkchen hängen an der `id` – beim Umbenennen eines Titels bleiben sie erhalten, beim Ändern der `id` nicht.
