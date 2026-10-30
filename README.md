# Spukwerkstatt – Premium Landingpage

**Status:** Website technisch vorbereitet; rechtliche Pflichtangaben sind noch nicht vollständig und die App ist nicht veröffentlicht.

## Inhalt

- `index.html` – responsive Startseite mit Spielmodi, FAQ, Konzeptbilder-Galerie, Entwicklungsstatus und DE/EN-Umschalter.
- `datenschutz.html` – eigenständige, deutsch/englische **Datenschutzerklärung als Entwurf** für die statische Website.
- `impressum.html` – eigenständiges, deutsch/englisches **Impressum als Entwurf**.
- `styles.css` – Design, responsive Layouts, Animationen, Zugänglichkeit.
- `app.js` – Übersetzungen, mobile Navigation, Galerie, Scroll-Effekte. Keine Tracker/externen Libraries.
- `assets/images` – optimierte WebP-Dateien aus dem bereitgestellten Konzept-Art-Paket.
- `assets/icons` – Favicon und Apple Touch Icon.

## Vor Veröffentlichung erledigen – wichtig

1. In `datenschutz.html` und `impressum.html`: `[Straße und Hausnummer]` durch **vollständige ladungsfähige Anbieteranschrift** ersetzen, nicht durch ein reines Postfach. Dasselbe gilt für die englischen Felder.
2. In `impressum.html`: geeignete weitere schnelle Kontaktmöglichkeit sowie gegebenenfalls weitere erforderliche Angaben ergänzen.
3. Name `Marcel Single`, Projektbezeichnung `Flondy`, Ort `88605 Meßkirch` und E-Mail `flondy.dev@gmail.com` auf Richtigkeit prüfen.
4. Datenschutzerklärung mit dem **tatsächlich eingesetzten Hosting** abgleichen. Der Entwurf ist auf GitHub Pages ausgerichtet; GitHub Pages protokolliert laut eigenen Angaben Besucher-IP-Adressen für Sicherheitszwecke.
5. Falls Analyse/Marketing-Cookies, Kontaktformulare, Videos mit Drittanbieter-Einbettungen, App-SDKs, Newsletter-Dienste oder zusätzliche Hosting-Dienste eingebaut werden: Datenschutzerklärung vor Live-Schaltung aktualisieren und etwaige Einwilligungen korrekt implementieren.
6. Web-Privacy und App-Privacy sind getrennt: Nach SDK- und Datenflussanalyse des späteren Spiels die App-Datenschutzhinweise erstellen/ergänzen.
7. Die sechs Screenshots sind **KI-generierte Konzeptgrafiken, keine echten Gameplay-Aufnahmen**. Vor dem finalen Store-Listing gegen echte Screenshots aus dem getesteten Spiel austauschen.
8. Google Play und App Store sind als **in Vorbereitung** gekennzeichnet und nicht anklickbar. Nach Release die offiziellen URLs integrieren.
9. Optional: echte Domain und absolute `og:image`-URL ergänzen, Search-Console/Sitemap erst nach Veröffentlichung.

Die bereitgestellte statische Seite selbst lädt keine externen Schriften, Tracker, Analytics oder Cookies und verwendet keine Browser-Speicherung. Sprachumschaltung per `?lang=en` / `?lang` (DE). Externe Links auf Rechtsquellen werden erst beim bewussten Klicken geöffnet.

## Lokal ansehen

`index.html` direkt im Browser öffnen oder (empfohlen) im Ordner einen lokalen Webserver starten:

```bash
python -m http.server 8080
```

Im Browser `http://localhost:8080` aufrufen. Für Englisch `http://localhost:8080/?lang=en`.

## GitHub Pages

Repository erstellen oder öffnen, die **Dateien aus diesem Ordner direkt ins Repository-Hauptverzeichnis** kopieren (oder bei Branch-Deployment ins konfigurierte Pages-Verzeichnis), committen und in **Settings → Pages** den Branch/Ordner für die Veröffentlichung konfigurieren. Relative Pfade funktionieren auch als Projektseite unter `/repository-name/`.

Veröffentlichung der Website erst nach Ergänzung der rechtlichen Pflichtangaben empfohlen.

## Technische Details

- Frameworkfrei, reine statische HTML/CSS/JS-Dateien
- Responsive für Smartphone, Tablet, Desktop
- Galerie mit Dialog-Lightbox und Tastatursteuerung
- Sprachumschaltung für komplette Website einschließlich Rechtsseiten
- `prefers-reduced-motion` berücksichtigt
- Bilder als komprimierte WebP-Dateien; keine remote CDN-Anfragen
- Kein Tracking, keine Anmeldeformulare und keine angeblichen Live-Store-Buttons
- Browser- und Gerätetests in `QA_REPORT.md`

## Rechtliche Quellen (Stand Oktober 2026)

- § 5 DDG: https://www.gesetze-im-internet.de/ddg/__5.html
- LFK Baden-Württemberg, Impressumspflicht: https://www.lfk.de/service/dokumente-rechtsgrundlagen/leitfaden-zur-impressumspflicht-im-internet
- GitHub Pages Datenverarbeitung: https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

Die bereitgestellten Rechtstexte sind ein ausfüllbarer Entwurf, keine verbindliche Rechtsberatung.
