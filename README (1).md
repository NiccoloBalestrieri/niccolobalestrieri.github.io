# Niccolò Balestrieri — Portfolio 👨‍💻✨

Benvenuto nel repository del mio **sito personale/portfolio**: un'unica pagina veloce, accessibile e mobile‑first per raccontare chi sono, cosa faccio e i miei progetti di AI & Software Engineering.

[**🌐 Live demo**](https://niccolobalestrieri.github.io/) · [📷 Anteprima](preview.png)

---

## 🚀 Caratteristiche principali

- **UI dark/light** con toggle (`☀️/🌙`), animazioni fluide e layout responsive.
- **Routing “single page”**: sezioni *Home*, *My Projects* e *Now* senza ricaricare la pagina.
- **Meta tag social completi** (Open Graph + Twitter Card) per condivisioni ottimizzate.
- **Progetti dinamici**: card pulite con tech‑tags e link diretti ai repo GitHub.
- **Mobile‑first**: menu hamburger, griglia elastica e tipografia leggibile su ogni schermo.
- **Facile da clonare e pubblicare su GitHub Pages** (nessun build step richiesto).

---

## 🧱 Tech stack

- **HTML5 + CSS3** (no framework, stile custom)
- **Vanilla JavaScript** per routing, menu e theme toggle
- **Open Graph/Twitter meta** per anteprime social
- Hosting consigliato: **GitHub Pages**

---

## 📁 Struttura (suggerita)

```
.
├── index.html               # Sito principale (questo repo)
├── README.md                # Questo file
├── preview.png              # Immagine di anteprima per social
├── siteicon.png             # Favicon / Touch icon
├── icon.jpg                 # Avatar (fallback gestito in <img onerror>)
├── favicon/
│   ├── githubicon.png
│   ├── instagramicon.png
│   └── linkedinicon.png
└── assets/                  # (opzionale) immagini aggiuntive
```

> Suggerimento: mantieni i nomi dei file come in `index.html` per evitare 404.


---

## 🛠️ Avvio rapido in locale

1. **Clona** il repo:
   ```bash
   git clone https://github.com/<tuo-utente>/<tuo-repo>.git
   cd <tuo-repo>
   ```

2. **Apri** `index.html` con il browser **oppure** avvia un server statico:
   ```bash
   # con Python 3
   python -m http.server 8000
   # poi visita: http://localhost:8000
   ```

---

## ☁️ Deploy su GitHub Pages (metodo semplice)

1. Fai **push** su `main` (o `master`).
2. Vai su **Settings → Pages**.
3. Seleziona **Source: Deploy from a branch**.
4. Scegli **Branch: main** e **/ (root)** → **Save**.
5. L’URL sarà: `https://<tuo-utente>.github.io/<tuo-repo>/`  
   *Se il repo si chiama `<tuo-utente>.github.io`, la pagina sarà su `https://<tuo-utente>.github.io/`.*

> Ricorda di impostare `preview.png` e `siteicon.png` nella root per anteprime e icone corrette.


---

## ⚙️ Personalizzazione rapida

- **Titolo, descrizione e anteprime social**: modifica i meta tag in `<head>`
  ```html
  <meta property="og:title" content="Niccolò Balestrieri - AI Specialist & Engineer">
  <meta property="og:description" content="I'm just a nerd who loves manga and AI. Turning ideas into code.">
  <meta property="og:image" content="https://niccolobalestrieri.github.io/preview.png">
  ```

- **Link social**: aggiorna gli `href` dentro `.social-links`.
- **Progetti**: aggiungi card nella sezione **My Projects** seguendo lo schema esistente.
- **Palette e stile**: modifica le CSS variables in `:root`:
  ```css
  :root {
    --bg-dark: #000000;
    --text-light: #ffffff;
    --text-muted: #999999;
    --accent: #3b82f6;
    --card-bg: #0a0a0a;
    --card-hover: #1a1a1a;
  }
  ```

---

## ♿ Accessibilità & UX

- Contrasto elevato in dark mode, tipografia leggibile.
- Navigazione via tastiera sui link principali.
- Riduzione *motion* moderata (transizioni brevi e non bloccanti).
- *Alt text* presente sull’avatar con **fallback** automatico a GitHub se l’immagine locale manca.

> Miglioramenti possibili: skip‑link per saltare all’area contenuti, `aria-current` per il tab attivo, focus‑ring più evidente.


---

## 🔍 SEO & Social

- **Open Graph** e **Twitter Card** già attivi.
- Titoli, sottotitoli e copy pensati per una *one‑pager* con parole chiave: *AI*, *Engineer*, *GenAI*, *Portfolio*.
- Suggerito: aggiungi una breve bio testuale (<200 caratteri) nella *Home* per rafforzare i risultati su motori di ricerca.


---

## 📈 Manutenzione & Performance

- Nessuna dipendenza esterna: caricamento rapido e semplice da *cache*.
- Consigli:
  - comprimi le immagini (`.png/.jpg` → `.webp` se possibile),
  - usa dimensioni coerenti (`avatar` 200×200/150×150),
  - evita immagini > 300–400 kB nella home,
  - abilita GitHub Pages con `Enforce HTTPS` (Settings → Pages).


---

## 🗺️ Roadmap (idee)

- [ ] Aggiungere sezione **Blog/Notes** con post in Markdown
- [ ] Modal/overlay per dettagli progetto con screenshot e stack
- [ ] Animazioni su scroll (GSAP o IntersectionObserver)
- [ ] i18n (IT/EN) con switch della lingua
- [ ] Test Lighthouse (A11y/Best Practices/SEO/Performance) e fix continui


---

## 🤝 Contribuire

È un portfolio personale, ma **issue** e **PR** con fix/migliorie sono benvenuti (accessibilità, performance, refactor CSS).


---

## 📜 Licenza

Rilasciato sotto **MIT License**. Vedi `LICENSE` (puoi crearla con:  
```bash
curl -o LICENSE https://raw.githubusercontent.com/github/gitignore/main/MIT.md
```

---

## 📫 Contatti

- **LinkedIn**: https://www.linkedin.com/in/niccolò-balestrieri-91a386252
- **GitHub**: https://github.com/NiccoloBalestrieri
- **Email**: niccolobalestrieri2@gmail.com

Se vuoi collaborare su progetti di **Generative AI**, **Computer Vision** o **MLOps**, scrivimi! 🚀
