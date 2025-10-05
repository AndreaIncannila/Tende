# MP TENDE — PWA (GitHub Pages)

Pacchetto pronto per pubblicazione su GitHub Pages e installazione come app.

## Come pubblicare
1. Crea un repo pubblico su GitHub e carica **tutti i file nella root**.
2. Vai su **Settings → Pages** e seleziona *Deploy from a branch*, branch **main**, folder **/** (root).
3. Apri l'URL del sito e dal browser fai **Installa app** / **Aggiungi a Home**.

## Come sostituire le icone con il tuo logo
- Sostituisci i file in `icons/` con PNG **192×192** e **512×512** (consigliata grafica su sfondo trasparente). 
- Sostituisci `logo-header.png` con l'immagine che vuoi appaia nella testata (altezza consigliata ~56–64px).
- Il nome dell'app è impostato su **MP TENDE** nel `manifest.webmanifest` e nel titolo della pagina.

## Note tecniche
- Cache offline con `service-worker.js` (cache-first). Se aggiorni i file, incrementa `mp-tende-pwa-v3` nel service worker.
- I modelli si salvano in `localStorage` (chiave `mp-tende-modelli-cm`).