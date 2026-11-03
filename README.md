# Tropen im Einkaufswagen – Das große Abschluss-Quiz

Browser-Quiz für Gesellschaftslehre, Klasse 7 (Gesamtschule NRW), zum Abschluss der Unterrichtsreihe
„Lecker, aber auch gut und fair? – Landwirtschaft in den Tropen“. Jede Runde greift einen Abschnitt des
Arbeitsblatts auf, damit die Schülerinnen und Schüler die Inhalte wiedererkennen.

## Aufbau

- 5 Runden, 18 Fragen (17 mit Punkten, 1 Meinungsfrage ohne Punkte), maximal 34 Punkte
  1. Tropen im Einkaufswagen 🛒
  2. Plantage oder Kleinbauern? 🌴👨‍👩‍👧
  3. Die Ölpalme und der Zutaten-Detektiv 🔍
  4. Ist das fair? Kwames Geschichte 🍫
  5. Fairtrade und meine faire Schokoverpackung 🏷️
- Formate: Multiple Choice, Mehrfachauswahl, Wahr/Falsch, Zuordnen per Antippen, Lückentext, Zutaten-Detektiv, Meinungsfrage
- 2 Punkte im ersten Versuch, 1 Punkt im zweiten Versuch, danach wird die Lösung mit Erklärung gezeigt
- Vorlese-Button (Web Speech API, deutsche Stimme des Geräts) und Tipp-Button an jeder Frage
- Ergebnis mit 1–3 Sternen und Abzeichen: ab 28 Punkten 3 Sterne „Tropen-Profi“, ab 18 Punkten 2 Sterne „Fair-Detektiv“, sonst 1 Stern „Tropen-Entdecker“
- „Nochmal spielen“ mischt Fragen (innerhalb der Runden) und Antworten neu, „Nur meine Fehler wiederholen“ zeigt alle Fragen, die nicht im ersten Versuch richtig waren

## Technik und Datenschutz

- Eine einzige Datei `index.html` (HTML, CSS, JavaScript), keine Frameworks, keine externen Skripte, Schriften oder Bilder
- Keine Anmeldung, keine Namen, keine Speicherung (auch kein localStorage), kein Tracking
- Grafiken: Emojis und eigene SVG-Zeichnungen
- Getestet für iPad (Safari) im Hoch- und Querformat (768 px und 1024 px Breite)
- Vorlesen: Ist auf dem iPad keine deutsche Stimme installiert, unter Einstellungen → Bedienungshilfen → Gesprochene Inhalte → Stimmen → Deutsch eine Stimme laden.

## Veröffentlichen mit GitHub Pages

Repository → Settings → Pages → „Deploy from a branch“ → Branch `main`, Ordner `/ (root)`.
Die Adresse lautet danach `https://<benutzername>.github.io/quiz-tropen/`.

## Inhalte anpassen

Alle Fragen stehen oben im Skriptteil von `index.html` im Array `ROUNDS`. Jede Frage hat einen Hinweis (`hint`)
und eine Erklärung (`explain`). Richtige Antworten sind mit `ok: true` markiert.
