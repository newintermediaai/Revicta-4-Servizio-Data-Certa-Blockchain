# Revicta 4 - Servizio Data Certa su Blockchain

**by NIAI (New Intermedia AI)**

link app https://spontaneous-palmier-a45222.netlify.app/

Servizio di notarizzazione documenti con hash SHA-256 e marca temporale su blockchain Bitcoin. Valido ai sensi delle vigenti leggi italiane.

---

## Funzionalita

- Calcolo hash SHA-256 del documento caricato
- Generazione certificato PDF con QR Code verificabile
- Creazione ZIP contenente: certificato, documento originale, ricevuta JSON
- Verifica transazione su Mempool.space (Mainnet / Testnet)
- Validazione TxID (64 caratteri esadecimali)
- Interfaccia responsive e ottimizzata per mobile

## Tecnologie

- HTML5 / CSS3 / JavaScript vanilla
- [jsPDF](https://github.com/parallax/jsjsPDF) - generazione PDF
- [JSZip](https://github.com/Stuk/jszip) - creazione archivi ZIP
- [QRCode.js](https://github.com/davidshimjs/qrcodejs) - generazione QR Code
- [Inter](https://fonts.google.com/specimen/Inter) - tipografia Google Fonts

## Deploy Netlify

### Opzione 1 - Drag & Drop

1. Accedi al tuo account Netlify
2. Trascina la cartella del progetto nell'area di deploy
3. Netlify serve automaticamente `index.html`

### Opzione 2 - CLI

```bash
# Installa Netlify CLI (una volta)
npm install -g netlify-cli

# Login (una volta)
netlify login

# Deploy
cd "Revicta 4 - Servizio Data Certa Blockchain"
netlify deploy --prod --dir=.
```

### Opzione 3 - app.bat

```
Doppio click su app.bat -> opzione [2] Deploy su Netlify
```

## Struttura file

```
Revicta 4 - Servizio Data Certa Blockchain/
├── index.html              # App principale (ottimizzata per Netlify)
├── netlify.toml            # Config Netlify (headers, cache, redirects)
├── app.bat                 # Script batch Windows
├── _headers                # Reference (config in netlify.toml)
├── _redirects              # Reference (config in netlify.toml)
├── README.md               # Questo file
├── codice iniziale*.txt    # Codice sorgente originale
├── Revicta 4*.html         # Versione abbellita (pre-ottimizzazione)
└── *.zip                   # Archivio distribuzione
```

## Utilizzo

1. Apri `index.html` nel browser
2. Seleziona il documento PDF
3. Clicca **Calcola Hash SHA-256**
4. Inserisci: nominativo, TxID, rete, data/ora
5. Clicca **Genera ZIP Completo**
6. Scarica il ZIP con certificato, documento e ricevuta

## Sicurezza

- Content Security Policy (CSP)
- X-Frame-Options: DENY
- X-Content-Type-Options: nosniff
- Strict-Transport-Security (HSTS)
- Referrer-Policy: strict-origin-when-cross-origin
- Permissions-Policy (camera/microfono/geolocalizzazione disabilitati)

## Licienza

Copyright 2026 NIAI - New Intermedia AI. Tutti i diritti riservati.
