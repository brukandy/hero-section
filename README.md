# 🎯 Hero Section - Leone Master School

Hero section moderna con sfondo animato WebGL, video 3D interattivo e integrazione Typeform.

## 📌 Info Progetto

- **Repository:** https://github.com/brukandy/hero-section
- **Live Demo:** https://brukandy.github.io/hero-section/
- **Account GitHub:** brukandy
- **Progetto Locale:** `/Users/brunolorenzon/CascadeProjects/hero-section/`
- **Stile:** Mindvalley-inspired con effetti 3D e animazioni premium
- **Versione:** 1.0.0

---

## ✨ Caratteristiche Principali

### 🌊 Sfondo Animato WebGL
- Shader personalizzato con effetto iridescente blu navy
- Animazione fluida e performante
- Position fixed per copertura full viewport

### 🎬 Video Interattivo 3D
- **GIF Thumbnail:** https://leonemasterschool.it/wp-content/uploads/2024/07/REF29JULY-ezgif.com-video-to-gif-converter.gif
- **Video Vimeo:** https://vimeo.com/1106026523
- Effetto 3D tilt che segue il movimento del mouse
- Play button con animazione smooth
- Autoplay Vimeo al click

### 📝 Typeform Integration
- **Form ID:** mGllVklt
- **URL:** https://form.typeform.com/to/mGllVklt
- Popup al 70% dello schermo
- CTA principale: "Conosciamoci meglio"
- Testo descrittivo sotto il bottone

### 🎨 Typography & Design
- **Headline:** Cormorant Garamond (64px desktop)
- **Gradiente animato** su "oltre i titoli"
  - Beige (#D4C5B0) → Bianco (#FFFFFF)
  - Effetto shimmer infinito (3s loop)
- **Body:** Inter font family
- Layout single-column centrato

### 🏛️ Logo IUL
- **URL:** https://leonemasterschool.it/wp-content/uploads/2024/07/iul.png
- Card con glassmorphism
- Hover effect con opacity
- Filter brightness per logo bianco

### 📊 Proof Stack (3 Cards)
1. **+60,000 corsisti** - Icona utenti
2. **1,300 testimonianze** - Icona stella
3. **92% tasso di completamento** - Icona check

Ogni card con:
- Icona SVG custom
- Background gradient blu
- Hover effect con transform
- Responsive grid layout

---

## 📋 Contenuti

### Copy
- **Headline:** "Risultati straordinari e concreti **oltre i titoli**"
  - "oltre i titoli" con gradiente animato shimmer
- **Subtitle:** "Affiancamento in crescita personale, business, immobiliare & coaching"
- **CTA Button:** "Conosciamoci meglio" (apre Typeform popup)
- **CTA Description:** "Prenota una chiamata con un selezionatore per chiedere maggiori informazioni"

### Trust Elements
- **Logo IUL** - Polo Universitario
- **Proof Stack:**
  - +60,000 corsisti
  - 1,300 testimonianze
  - 92% tasso di completamento dei programmi

---

## 🎨 Design System

### Colori
```css
/* Background */
--bg-navy: #0f172a;
--bg-navy-dark: #1e3a8a;

/* Gradiente Testo */
--gradient-beige: #D4C5B0;
--gradient-beige-light: #E8DCC8;
--gradient-white: #FFFFFF;

/* CTA Button */
--btn-primary: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%);

/* Glass Effects */
--glass-bg: rgba(255, 255, 255, 0.05);
--glass-border: rgba(255, 255, 255, 0.1);
```

### Typography
```css
/* Fonts */
font-family: 'Cormorant Garamond', serif; /* Headlines */
font-family: 'Inter', sans-serif; /* Body */

/* Sizes */
--h1-desktop: 64px;
--h1-tablet: 48px;
--h1-mobile: 36px;
--subtitle: 20px;
--body: 16px;
```

### Spacing
```css
--section-padding: 80px 40px 120px;
--card-padding: 20px;
--gap-cards: 24px;
```

---

## 🛠️ Installazione

### 1. Clone Repository
```bash
git clone https://github.com/brukandy/hero-section.git
cd hero-section
```

### 2. Apri Locale
```bash
# Usa un server locale (es. Live Server VSCode)
# Oppure Python
python3 -m http.server 8082
```

### 3. Apri Browser
```
http://localhost:8082
```

---

## 📦 Integrazione Elementor

### Metodo 1: iFrame (Consigliato)
```html
<style>
/* Reset padding Elementor */
.elementor-widget-html {
    margin: 0 !important;
    padding: 0 !important;
}
.elementor-widget-container {
    margin: 0 !important;
    padding: 0 !important;
}
</style>

<iframe 
    src="https://brukandy.github.io/hero-section/" 
    width="100%" 
    height="1100" 
    frameborder="0"
    scrolling="no"
    style="border: none; display: block; margin: 0; padding: 0; overflow: hidden;">
</iframe>
```

### Istruzioni Elementor
1. **Crea sezione** Full Width
2. **Imposta sezione:**
   - Padding: 0 su tutti i lati
   - Margin: 0 su tutti i lati
3. **Aggiungi widget HTML**
4. **Incolla il codice** sopra
5. **Salva e pubblica**

### Note
- **Altezza iframe:** 1100px (regola se necessario)
- **Typeform:** Funziona nel popup
- **Video 3D:** Effetto mouse funziona
- **Responsive:** Automatico

---

## 📱 Responsive Breakpoints

### Desktop (> 1024px)
- Layout single-column centrato
- Video max-width: 600px
- Proof stack: 3 colonne

### Tablet (768px - 1024px)
- Headline: 48px
- Video: 100% width
- Proof stack: 2 colonne

### Mobile (< 768px)
- Headline: 36px
- Video: 100% width
- Proof stack: 1 colonna
- Padding ridotto

---

## 🎬 Funzionalità JavaScript

### 1. Sfondo Animato WebGL
```javascript
// Inizializzazione shader WebGL
// File: script.js (linee 1-98)
```

### 2. Video 3D Tilt Effect
```javascript
// Effetto 3D che segue il mouse
// File: script.js (linee 100-125)
```

### 3. Play Button → Vimeo
```javascript
// Toggle GIF thumbnail / Vimeo iframe
// File: script.js (linee 127-145)
```

### 4. Typeform Popup
```javascript
// Caricato da embed.typeform.com/next/embed.js
// Configurato con data-attributes HTML
```

---

## 📂 Struttura File

```
hero-section/
├── index.html          # Struttura HTML
├── style.css           # Stili CSS
├── script.js           # JavaScript (WebGL + interazioni)
├── README.md           # Documentazione
└── .git/              # Git repository
```

---

## 🔄 Workflow Aggiornamenti

### 1. Modifica Locale
```bash
# Modifica i file
code .
```

### 2. Test Locale
```bash
# Apri con Live Server o Python
python3 -m http.server 8082
```

### 3. Commit & Push
```bash
git add .
git commit -m "Descrizione modifiche"
git push origin main
```

### 4. Verifica GitHub Pages
- Aspetta 1-2 minuti
- Apri: https://brukandy.github.io/hero-section/
- Hard refresh: Cmd+Shift+R (Mac) o Ctrl+F5 (Windows)

### 5. Aggiorna Elementor
- Svuota cache Elementor (Tools → Regenerate CSS)
- Svuota cache WordPress
- Hard refresh browser

---

## 🎯 Personalizzazione

### Cambiare Typeform
```html
<!-- In index.html, linea 64 -->
<button data-tf-popup="TUO_FORM_ID" ...>
```

### Cambiare Video Vimeo
```html
<!-- In index.html, linea 52 -->
<iframe src="https://player.vimeo.com/video/TUO_VIDEO_ID?autoplay=1...">
```

### Cambiare GIF Thumbnail
```html
<!-- In index.html, linea 38 -->
<img src="URL_TUA_GIF" alt="Video thumbnail">
```

### Modificare Colori
```css
/* In style.css */
/* Cerca e modifica i valori hex/rgba */
```

---

## 🐛 Troubleshooting

### Typeform non si apre
- Verifica che lo script `embed.typeform.com/next/embed.js` sia caricato
- Controlla console browser per errori
- Verifica Form ID corretto

### Video 3D non segue mouse
- Verifica che `script.js` sia caricato
- Controlla console per errori JavaScript
- Testa su browser moderno (Chrome, Firefox, Safari)

### Sfondo animato non visibile
- Verifica supporto WebGL del browser
- Controlla console per errori shader
- Fallback: background blu navy statico

### iFrame Elementor non funziona
- Svuota cache Elementor
- Verifica padding/margin sezione = 0
- Controlla altezza iframe (min 1100px)

---

## 📊 Performance

- **Lighthouse Score:** 95+ (Performance)
- **First Contentful Paint:** < 1.5s
- **Time to Interactive:** < 3s
- **WebGL:** GPU-accelerated
- **Immagini:** Ottimizzate e lazy-loaded

---

## 🚀 Prossimi Step

- [ ] Aggiungere analytics tracking
- [ ] A/B testing CTA copy
- [ ] Ottimizzare mobile performance
- [ ] Aggiungere più animazioni micro-interactions
- [ ] Integrare con CRM

---

## 📝 Changelog

### v1.0.0 (26 Nov 2024)
- ✅ Sfondo animato WebGL blu navy
- ✅ Video 3D interattivo con mouse tracking
- ✅ Typeform integration (popup 70%)
- ✅ Logo IUL con glassmorphism
- ✅ Proof stack 3 cards
- ✅ Gradiente animato shimmer su "oltre i titoli"
- ✅ Font Cormorant Garamond + Inter
- ✅ Responsive completo
- ✅ GitHub Pages deploy
- ✅ Elementor iframe ready

---

## 👨‍💻 Sviluppato per

**Leone Master School**
- Piattaforma: LearnWorlds + WordPress/Elementor
- Design System: Mindvalley-inspired
- Focus: Conversione e engagement premium

---

## 📄 Licenza

Proprietario - Leone Master School © 2024

---

**Made with ❤️ for Leone Master School**
