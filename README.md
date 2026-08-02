# Ziel-Countdown

Eine Seite für ein Vertriebsziel: Zahl eintragen, Link verschicken, das Team sieht den Stand live.

## Nutzung

1. Seite öffnen (siehe „GitHub Pages aktivieren" unten für die URL).
2. Titel, Zielbetrag und aktuellen Stand eintragen, auf **„Board erstellen & Link holen"** klicken.
3. Der Browser springt automatisch auf einen Link mit `?g=...` – das ist der Link fürs Team.
4. Diesen Link ans Vertriebsteam schicken.
5. Über das Zahnrad unten rechts kann der Stand jederzeit aktualisiert werden. Alle, die den Link offen haben, sehen die neue Zahl automatisch innerhalb weniger Sekunden (kein neuer Link nötig).

Der Stand wird in einer Firebase Realtime Database gespeichert (Projekt `test-3cf18`, Regeln aktuell öffentlich lesbar/schreibbar). Die Board-ID im Link ist der einzige Schlüssel dazu – Link also nur an die gewünschten Personen schicken.

## GitHub Pages aktivieren (einmalig)

1. Im Repo zu **Settings → Pages**.
2. Bei **Source** „Deploy from a branch" auswählen.
3. Branch **main**, Ordner **/(root)** wählen, speichern.
4. Nach ein bis zwei Minuten ist die Seite unter `https://<dein-github-name>.github.io/Ziel-Countdowm/` erreichbar.

Kein Build-Schritt nötig – es ist eine einzelne statische `index.html`.
