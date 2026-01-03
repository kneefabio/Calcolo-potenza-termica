# 🔥 Calcolatore Potenza Termica - PWA

App Progressive Web per calcolare la potenza termica necessaria per riscaldare ambienti.

## 📦 File Inclusi

- `index.html` - File principale dell'applicazione
- `manifest.json` - Configurazione PWA
- `service-worker.js` - Per funzionamento offline
- `icon-192.png` - Icona piccola (192x192)
- `icon-512.png` - Icona grande (512x512)

## 📱 Installazione su Android

### Metodo 1: Hosting Online (Consigliato)

1. **Carica i file su un hosting gratuito:**
   - GitHub Pages (gratis, facile)
   - Netlify Drop (trascina la cartella)
   - Vercel
   - Firebase Hosting

2. **Installa l'app:**
   - Apri l'URL con Chrome su Android
   - Apparirà un banner "Aggiungi a Home"
   - Oppure: Menu (⋮) → "Installa app" o "Aggiungi a schermata Home"

### Metodo 2: Server Locale

1. **Avvia un server locale:**
   ```bash
   # Con Python 3
   python3 -m http.server 8000
   
   # Con Node.js
   npx http-server
   ```

2. **Trova l'IP locale del PC:**
   - Windows: `ipconfig`
   - Mac/Linux: `ifconfig` o `ip addr`

3. **Sul telefono:**
   - Connettiti alla stessa rete WiFi
   - Apri Chrome e vai a `http://[IP-PC]:8000`
   - Installa l'app dal menu

## 💻 Uso su PC

Basta aprire `index.html` con un browser moderno:
- Chrome
- Firefox
- Edge
- Safari

## 🚀 Hosting Gratuito Consigliato

### GitHub Pages (Il più semplice)

1. Crea un account su GitHub
2. Crea un nuovo repository
3. Carica tutti i file
4. Vai in Settings → Pages
5. Seleziona "main branch"
6. L'app sarà online su: `https://[tuo-username].github.io/[nome-repo]`

### Netlify Drop

1. Vai su https://app.netlify.com/drop
2. Trascina la cartella con tutti i file
3. Ottieni subito un URL pubblico

## ✨ Caratteristiche

- ✅ Funziona offline dopo la prima visita
- ✅ Installabile come app nativa
- ✅ Calcolo in tempo reale
- ✅ Parametri opzionali avanzati
- ✅ Responsive (PC, tablet, smartphone)
- ✅ Segue normative UNI EN 12831

## 🔧 Troubleshooting

**L'opzione "Installa app" non appare:**
- Usa Chrome (altri browser potrebbero non supportare PWA)
- L'app deve essere servita via HTTPS o localhost
- Ricarica la pagina

**Non funziona offline:**
- Aspetta qualche secondo dopo il primo caricamento
- Controlla che il service worker sia registrato (F12 → Application → Service Workers)

## 📝 Note

- Le icone sono generate automaticamente con un design a termometro
- Il manifest.json configura colori e comportamento dell'app
- Il service worker gestisce la cache per l'uso offline
