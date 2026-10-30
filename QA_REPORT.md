# Spukwerkstatt Landingpage – Qualitätsbericht

Stand: 30.10.2026

## Automatisch erfolgreich geprüft

- 3 HTML-Seiten erstellt: `index.html`, `datenschutz.html`, `impressum.html`.
- HTML geprüft: jede Seite hat ein Dokument-`title` und genau ein `h1`.
- Alle lokalen Bild-, CSS-, Script- und internen Seitenlinks verweisen auf existierende Dateien.
- Übersetzungsschlüssel aller `data-i18n`-Elemente in der JavaScript-Sprachdatei vorhanden.
- JavaScript-Syntaxprüfung (`node --check`) ohne Fehler.
- CSS über `tinycss2` geparst; keine Parserfehler.
- 5 Modus-Karten und 6 Konzept-Galeriegrafiken vorhanden.
- Alle Assets lokal eingebunden; keine externen Schrift-/Analyse-/Tracking-Skripte.
- Google Play und Apple App Store als **in Vorbereitung**, keine erfundenen Downloadlinks.
- Asset-Bilder für das Web als WebP komprimiert.

## Offen / noch nicht bestätigt

- **Visuelle Browserprüfung:** Chromium/Playwright ließ in dieser Ausführungsumgebung keine Navigationen zu (`ERR_BLOCKED_BY_ADMINISTRATOR`). Deshalb keine echten Desktop-/Mobil-Screenshots oder Browser-Interaktionstests. CSS-Responsivität ist implementiert, aber nicht browser-visuell verifiziert.
- Realgerätetest / Accessibility-Prüfung mit Screenreader, Tastatur und mobilen Browsern ausstehend.
- Juristische Prüfung der Datenschutz- und Impressumstexte ausstehend.
- Vollständige ladungsfähige Anschrift und weitere schnelle Kontaktmöglichkeit fehlen und sind als Platzhalter markiert.
- Echte Store-URLs sowie reale Gameplay-Screenshots fehlen, da Spiel noch nicht veröffentlicht bzw. auf Geräten getestet ist.

## Empfehlung

Vor der Veröffentlichung im lokalen Browser sowie auf Android/iPhone testen, Pflichtangaben ersetzen, Datenschutztext an tatsächliches Hosting anpassen, später reale Gameplay-Bilder ergänzen. Nach jeder SDK- oder Tracking-Integration die Datenschutzerklärung erneut prüfen.
