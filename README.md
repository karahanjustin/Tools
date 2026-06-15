# Tools Hub

Internes Werkzeug-Dach von Potsdam Media. Eine vernetzte Oberflaeche, die zu allen
Tools fuehrt und den geteilten Demo-Terminplaner enthaelt.

Live: https://potsdam-media.de/Tools/

## Tools

- **Call Tracker** (live) -> https://potsdam-media.de/leads/
- **Terminplaner** (live) -> Cal.com-Einbettung im Hub
- Lead Finder, Pipeline, Demo Studio -> geplant

## Kalender verbinden

Der Terminplaner bettet Cal.com ein (geteilt, Zeitzonen + Erinnerungen automatisch).
Zum Aktivieren in `index.html` die Konstante setzen:

```js
const CAL_LINK = "homeservicereply/demo";  // dein cal.com user/event
```

Solange `CAL_LINK` leer ist, zeigt der Hub eine Anleitung statt des Kalenders.

## Neues Tool hinzufuegen

In `index.html` im `.grid` eine weitere `.card live` mit Link ergaenzen, oder eine
`.card soon` als Platzhalter. Single-file, kein Build, kein Backend.

## Deployment

GitHub Pages aus `main`, Root. Custom Domain (potsdam-media.de) wird vom User-Pages-Setup
geerbt, daher liegt der Hub unter `/Tools/`.
