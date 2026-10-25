# Scudo QR

Controlla un QR code prima di aprirlo: mostra il dominio reale, segnala siti sosia, link accorciati, download di app e altri trucchi, e (facoltativo) confronta il link con Google Safe Browsing.

## Pubblicazione su GitHub Pages
1. Crea il repository `scudo-qr` e carica tutti i file di questa cartella.
2. Settings > Pages > Source: branch `main`, cartella `/ (root)`.
3. Apri `https://andreabossardi-png.github.io/scudo-qr/` dal telefono e scegli "Aggiungi a schermata Home".

## Google Safe Browsing (facoltativo)
1. Su console.cloud.google.com crea un progetto e abilita **Safe Browsing API**.
2. Crea una chiave API e limitala ai referrer `https://andreabossardi-png.github.io/*` e alla sola Safe Browsing API.
3. Nell'app apri "Controllo con Google Safe Browsing" e incolla la chiave. Resta salvata solo sul telefono.

L'API Lookup di Safe Browsing è gratuita per uso non commerciale.

## File
- `index.html` app completa (analisi, fotocamera live, foto, storico)
- `jsQR.js` lettore QR (jsQR 1.4.0, licenza Apache 2.0), usato quando il browser non ha BarcodeDetector
- `sw.js`, `manifest.json`, icone: installazione e uso offline
