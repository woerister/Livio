# Livio – Website (Support, Datenschutz, Impressum)

Statische Website der App **Livio** (ENKL-NET GmbH). Sie wird für die App-Store-Einreichung benötigt:

| Datei | Zweck | App Store Connect |
|---|---|---|
| `index.html` | Startseite | Marketing-URL (optional) |
| `support.html` | Support und FAQ | Support-URL |
| `privacy.html` | Datenschutzerklärung | Privacy-Policy-URL |
| `impressum.html` | Impressum (§ 5 DDG) | – |
| `style.css` | gemeinsames Styling (inkl. Dark Mode) | – |
| `favicon.svg`, `404.html` | Icon, Fehlerseite | – |

Es gibt keinen Build-Schritt: Dateien bearbeiten, committen, pushen. Header und Footer stehen in jeder HTML-Datei; bei Änderungen an der Navigation alle Seiten anpassen.

## Hosting

GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / `(root)`**.
Die resultierende URL (`https://<user>.github.io/Livio/`) bzw. eine eigene Domain trägst du in App Store Connect ein. Die Datenschutzerklärung nennt GitHub Pages als Hoster; wird anders gehostet, muss der Abschnitt „Hosting dieser Website“ angepasst werden.

## Qualitätssicherung

`.github/workflows/check.yml` prüft bei jedem Push/PR: keine Platzhalter wie `[… einfügen]`, keine kaputten internen Links, valides HTML/CSS.

## Checkliste bei jedem App-Release

- [ ] Stimmen Berechtigungen und Datenkategorien noch mit `privacy.html` überein (und mit Privacy Manifest und App-Store-Datenschutzangaben)?
- [ ] Stimmen Menünamen und Schritte in den FAQ auf `support.html` noch mit der App überein?
- [ ] „Stand“-Datum in `privacy.html` aktualisiert, falls der Text geändert wurde?
- [ ] URLs in App Store Connect erreichbar?
