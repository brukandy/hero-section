# 🎯 Hero Section - Leone Master School

Hero section con sfondo animato blu navy e video 3D interattivo che segue il mouse.

## 📌 Info Progetto

- **Progetto Locale:** `/Users/brunolorenzon/CascadeProjects/hero-section/`
- **Account GitHub:** brukandy
- **Stile:** Mindvalley-inspired con effetti 3D

## ✨ Caratteristiche

- 🌊 **Sfondo animato** WebGL blu navy
- 🎬 **Video 3D interattivo** che segue il movimento del mouse
- 📱 **Responsive** layout a 2 colonne (desktop) → 1 colonna (mobile)
- 🎨 **Design moderno** con gradienti e glassmorphism
- ⭐ **Trust elements** con numeri e badge

## 📋 Contenuti

### Copy
- **Headline:** "Risultati straordinari e concreti oltre i titoli"
- **Subtitle:** Affiancamento in crescita personale, business, immobiliare & coaching
- **CTA 1:** Conosciamoci meglio
- **CTA 2:** Prenota una chiamata

### Trust Elements
- **Badge:** Università IUL · Trustpilot ⭐⭐⭐⭐⭐
- **Proof Stack:**
  - +60.000 corsisti affiancati
  - 1.300 testimonianze reali (367 a 5 stelle)
  - 92% tasso completamento programmi

### Video
- Layout 16:9
- Inclinazione iniziale: -5° Y, 2° X
- Effetto 3D: max ±15° rotazione seguendo mouse
- Smooth animation con interpolazione

## 🎨 Design System

### Colori
- **Background:** Blu navy animato (#17233B base)
- **Testo primario:** #ffffff
- **Testo secondario:** rgba(255, 255, 255, 0.8)
- **Gradient accent:** #60a5fa → #a78bfa
- **CTA primary:** #3b82f6 → #2563eb

### Tipografia
- **Font:** Inter (Google Fonts)
- **Title:** 56px / 900 weight
- **Subtitle:** 20px / 400 weight
- **Trust numbers:** 36px / 800 weight
- **Trust labels:** 13px / 400 weight

### Spacing
- **Section padding:** 80px verticale, 40px orizzontale
- **Grid gap:** 80px tra colonne
- **Button gap:** 16px
- **Trust bar gap:** 32px

## 🎬 Effetto Video 3D

### Parametri
```javascript
maxRotation: 15      // Gradi massimi rotazione
smoothness: 0.1      // Velocità seguimento mouse (0-1)
```

### Come Funziona
1. Mouse entra nell'area video
2. Posizione normalizzata (-1 a 1)
3. Calcolo rotazione X e Y
4. Interpolazione smooth con requestAnimationFrame
5. Mouse esce → reset a posizione iniziale

## 🔧 Installazione WordPress Elementor

### Metodo: HTML Widget

1. **Crea sezione** Full Width in Elementor
2. **Imposta sezione:**
   - Padding: 0 su tutti i lati
   - Margin: 0 su tutti i lati
   - Min Height: 100vh

3. **Aggiungi widget HTML**
4. **Copia tutto il contenuto** di `index.html`
5. **Modifica URL video** con il tuo video YouTube/Vimeo

### Personalizzazione URL Video

Nell'HTML, cerca:
```html
<iframe src="https://www.youtube.com/embed/VIDEO_ID"
```

Sostituisci `VIDEO_ID` con l'ID del tuo video.

## 📱 Responsive Breakpoints

- **Desktop (> 1024px):** 2 colonne, video 3D attivo
- **Tablet (768px - 1024px):** 1 colonna, video 3D ridotto
- **Mobile (< 768px):** 1 colonna, video statico

## 🚀 Server Locale

```bash
cd /Users/brunolorenzon/CascadeProjects/hero-section
python3 -m http.server 8082
# Apri: http://localhost:8082
```

## 🎯 Prossimi Step

1. ✅ Struttura HTML creata
2. ✅ CSS con effetti 3D
3. ✅ JavaScript sfondo + mouse tracking
4. ⏳ Sostituire URL video placeholder
5. ⏳ Deploy su GitHub Pages
6. ⏳ Test su WordPress Elementor

## 📝 Note Tecniche

- **WebGL:** Sfondo animato con shader personalizzati
- **3D Transform:** CSS transform con perspective
- **Mouse Tracking:** Event listener con normalizzazione coordinate
- **Smooth Animation:** requestAnimationFrame con interpolazione
- **Performance:** GPU-accelerated transforms

## 🔄 Modifiche Future

- [ ] Aggiungere video reale
- [ ] Link CTA funzionanti
- [ ] Ottimizzare performance mobile
- [ ] A/B test varianti copy
- [ ] Analytics tracking

---

**Made with ❤️ for Leone Master School**
