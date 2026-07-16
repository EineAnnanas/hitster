# Hitster Klassik – Handy-App (PWA)

Solo-Spiel mit automatischem Spotify-Playback. Einmaliges Setup, danach: App öffnen, Kopfhörer rein, spielen.

## 1. App hosten (einmalig, ~5 Min)

Das Spotify-Login braucht eine echte Web-Adresse (https), eine lokale Datei reicht nicht.
Kostenlos mit GitHub Pages:

1. Auf github.com einloggen (oder Account anlegen) → **New repository**, Name z.B. `hitster-klassik`, Public, anlegen.
2. **Add file → Upload files** → alle Dateien aus diesem Ordner hochladen (`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`) → Commit.
3. Repo → **Settings → Pages** → unter "Branch" `main` und `/ (root)` wählen → Save.
4. Nach ~1 Minute ist die App erreichbar unter:
   `https://DEINNAME.github.io/hitster-klassik/`

## 2. Spotify-Developer-App anlegen (einmalig, ~3 Min, Premium nötig)

1. Auf **developer.spotify.com/dashboard** mit deinem Spotify-Konto einloggen.
2. **Create app**: Name/Beschreibung egal, als **Redirect URI** exakt deine App-Adresse aus Schritt 1 eintragen
   (mit `/` am Ende, genau so, wie es die App unter "Spotify verbinden" anzeigt). API: "Web API" anhaken. Speichern.
3. In der App-Übersicht die **Client ID** kopieren.

## 3. In der App verbinden

1. App-Adresse am Handy öffnen → **Spotify verbinden** → Client ID einfügen → **Mit Spotify verbinden** → Login bestätigen.
2. Aufs Handy legen: In Safari **Teilen → Zum Home-Bildschirm**, in Chrome/Android **Installieren**. Läuft dann im Vollbild wie eine App.

## Spielen

- **Solo · Endlos**: 3 Leben, Highscore. / **Solo · Klassisch**: Zielzahl erreichen. / **Party**: 2–6 Teams.
- "Karte ziehen" startet den Song automatisch **blind** über deine Spotify-App (auch bei gesperrtem Bildschirm).
  Falls nichts spielt: Spotify-App einmal öffnen, irgendetwas kurz anspielen, zurückwechseln, erneut Play.
- Ohne Spotify-Verbindung funktioniert alles weiter per QR-Code/Link.

## Hinweise

- Playback-Steuerung erfordert **Spotify Premium** (Spotify-Beschränkung).
- Spielstand und Highscore werden im Browser gespeichert.
