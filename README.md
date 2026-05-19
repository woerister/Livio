# Livio – Legal / Support Pages

Dieser Ordner enthält die statischen HTML-Seiten für **Privacy Policy** und **Support**, die für die App-Store-Einreichung von Livio gehostet werden müssen.

## Dateien

- `privacy.html` – Datenschutzerklärung (URL muss in ASC unter „Privacy Policy URL" eingetragen werden)
- `support.html` – Support-Seite (URL muss in ASC unter „Support URL" eingetragen werden)
- `index.html` – einfache Übersichtsseite, die auf beide verlinkt

## Vor dem Hosten ausfüllen

In allen drei HTML-Dateien gibt es Platzhalter in `[eckigen Klammern]`. Such und ersetz:

- `[Anschrift einfügen]` / `[Adresse einfügen]` → Postanschrift der ENKL-NET GmbH
- `[Support-Adresse einfügen]` → Support-E-Mail (z. B. `support@enkl-net.de`)
- `[E-Mail einfügen]` → Kontakt-E-Mail (kann die gleiche sein)

Datum unten in `privacy.html` ggf. anpassen, falls du was am Wortlaut änderst.

## Hosting via GitHub Pages (kostenlos, ~5 Minuten)

1. Auf GitHub einen neuen öffentlichen Repo anlegen, z. B. `livio-legal`.
2. Die drei HTML-Dateien aus diesem Ordner committen und pushen.
3. Im Repo unter **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)`
   - Save
4. Nach 1–2 Minuten erreichbar unter `https://<dein-user>.github.io/livio-legal/`.
5. URLs für App Store Connect:
   - Privacy: `https://<dein-user>.github.io/livio-legal/privacy.html`
   - Support: `https://<dein-user>.github.io/livio-legal/support.html`

## Hosting via Notion (Alternative, noch schneller)

1. Notion → neue Seite „Livio Datenschutz" → Inhalt einfügen → **Share → Publish to web**.
2. Gleiches Vorgehen für eine Support-Seite.
3. Die beiden public URLs in ASC eintragen.

(Notion macht aus dem HTML kein 1:1, du kannst aber den Text aus den HTML-Dateien als Markdown aufbereiten.)

## Hosting auf eigener Domain

Wenn ENKL-NET eine Website mit eigenem Webspace hat, einfach die drei HTML-Dateien per FTP/SFTP hochladen, z. B. nach `https://enkl-net.de/livio/`.

## Wartung

- Bei jedem App-Update prüfen, ob die Datenschutzerklärung noch stimmt (z. B. neue Berechtigungen, neue Datenkategorien).
- Datum in `privacy.html` aktualisieren, wenn der Inhalt sich ändert.
- Die App-Store-Connect-Pflicht zur Privacy Policy URL bleibt für jedes Release bestehen.
