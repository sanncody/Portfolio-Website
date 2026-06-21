# Sandeep Wadhawan — Portfolio Website

A personal portfolio website built with plain HTML, CSS, and Bootstrap. Fully static, no build step required.

**Live:** [sanncody.github.io/Portfolio-Website](https://sanncody.github.io/Portfolio-Website/)

---

## Sections

| Section | Description |
|---|---|
| **Home** | Intro with a typed.js animation cycling through tech stack |
| **Experience** | Work history — FluxusForge, Revispy, Kirabiz Technologies |
| **Skills** | Tech stack cards — Node.js, Express, Fastify, MongoDB, React, TypeScript, etc. |
| **Education** | BVICAM (MCA) and Rajdhani College (B.Sc. Mathematics) |
| **Projects** | Sannsta, MERN Chat App, Post-Burst |
| **Certifications** | Sheryians Coding School, Scaler, HackerRank |
| **Contact** | Form with inline toast feedback, powered by Google Apps Script |

---

## Tech Stack

- **HTML5 / CSS3**
- **Bootstrap 5** — layout and responsive grid
- **AOS** (Animate On Scroll) — scroll-triggered fade-in animations
- **Typed.js** — typewriter effect on the home section
- **Remix Icons + Line Awesome** — icon sets
- **Google Apps Script** — serverless contact form backend

---

## Project Structure

```
Portfolio-Website/
├── index.html              # Main entry point
├── assets/
│   ├── css/
│   │   ├── style.css       # Custom styles and theme variables
│   │   ├── bootstrap.min.css
│   │   ├── aos.css
│   │   └── line-awesome.min.css
│   ├── js/
│   │   ├── main.js
│   │   ├── bootstrap.bundle.min.js
│   │   └── aos.js
│   ├── images/             # Profile photo and institution images
│   ├── fonts/              # Line Awesome font files
│   └── cv/
│       ├── Sandeep_Resume_2026.html   # Print-ready resume (open in Chrome → Ctrl+P → Save as PDF)
│       └── *.pdf                      # Exported resume PDFs
└── README.md
```

---

## Running Locally

No build tools needed. Just open `index.html` in a browser:

```bash
# Clone the repo
git clone https://github.com/sanncody/Portfolio-Website.git
cd Portfolio-Website

# Open directly
start index.html        # Windows
open index.html         # macOS
```

Or use the VS Code **Live Server** extension for hot reload.

---

## Contact Form

The contact form submits to a **Google Apps Script** endpoint using `fetch` with `mode: 'no-cors'`. On success, an inline green toast is shown; on failure, a red toast with a direct email fallback appears.

To swap in your own endpoint, update the `scriptURL` constant at the bottom of `index.html`:

```js
const scriptURL = 'https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec';
```

---

## Resume (CV)

The file `assets/cv/Sandeep_Resume_2026.html` is a print-ready single-page resume.

**To export as PDF:**
1. Open the file in **Chrome**
2. Press `Ctrl+P`
3. Destination → **Save as PDF**
4. Paper size → **A4**, Margins → **None**
5. Enable **Background graphics**
6. Save

---

## Connect

- **Email:** sandeepwadhawan2001@gmail.com
- **LinkedIn:** [linkedin.com/in/sandeep-wadhawan-1055a1195](https://www.linkedin.com/in/sandeep-wadhawan-1055a1195/)
- **GitHub:** [github.com/sanncody](https://github.com/sanncody)
