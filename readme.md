# PAREK Framework Website

Welcome to the **PAREK Framework Website** — an multi‑page portal that presents the **P**ost‑quantum **A**sset & Algorithm Inventory, **R**isk Assessment, **E**xecution, and **K**ey‑governance (PAREK) methodology.

Live instance: **<https://www.pqc.lt>**  

---

## 📑 Table of Contents
1. [About the Project](#about-the-project)  
2. [Features](#features)  
3. [Repository Layout](#repository-layout)  
4. [Quick Start](#quick-start)  
5. [Local Development](#local-development)  
6. [Deployment](#deployment)  
7. [Contributing](#contributing)  
8. [License](#license)  
9. [Acknowledgements](#acknowledgements)

---

## About the Project
The PAREK Framework is an EU‑aligned methodology that guides organisations from discovery of quantum‑vulnerable cryptography to full post‑quantum deployment and continuous crypto‑agility. This website provides:

* **Framework overview** and the five lifecycle stages.
* **Objectives** mapping PAREK to EU milestones (2026 ▸ 2030 ▸ 2035).
* **Features** such as CBOM‑centric discovery and hybrid migration patterns.
* **Progress dashboard** tracking project status.

The site is fully static (HTML/CSS) and styled to mimic an Emacs buffer using bespoke CSS.

## Features
* **Emacs‑style UI** — Solarized‑dark palette, header/modeline, monospace fonts.
* **Multi‑page navigation** — `index.html`, `framework.html`, `objectives.html`, `features.html`, `progress.html`.
* **Org‑mode flavour** — Section bullets (`*`, `-`) to ease copy‑paste into Org documents.
* **No build toolchain required** — plain HTML & CSS; just host the files.

## Repository Layout
```
├── docs/                 # Source of the live site (served by GitHub Pages)
│   ├── index.html        # Main landing page
│   ├── framework.html    # PAREK framework details
│   ├── objectives.html   # Programme objectives
│   ├── features.html     # Key features
│   ├── progress.html     # Status dashboard
│   └── style.css         # Emacs‑inspired styling
├── .github/
│   └── workflows/        # CI for link checking & HTML validation
├── README.md             # This file
└── LICENSE               # MIT License
```

> **Tip 📝**  If you fork this repo, simply edit any HTML file under `docs/` and commit. GitHub Pages will publish the change within minutes.

## Quick Start
```bash
# Clone repository
$ git clone https://github.com/Grigaliunas/parek‑framework‑site.git
$ cd parek‑framework‑site

# Preview locally (Python 3.x)
$ python -m http.server -d docs 8080
# → open http://localhost:8080 in your browser
```

## Local Development
1. **Edit HTML** — the pages are plain HTML; any editor works.  
2. **Style tweaks** — modify `docs/style.css`.  
3. **Validate** — run `npm install -g html‑validator-cli` and `html-validator --file docs/index.html` for W3C compliance.

## Deployment
### GitHub Pages
1. Go to **Settings ▸ Pages**.  
2. Select **Branch** = `main`, **Folder** = `/docs`.  
3. Save — your site will be available at `https://<user>.github.io/<repo>/`.

### Custom Domain
1. Add `www.pqc.lt` to **Settings ▸ Pages ▸ Custom domain**.  
2. Create a CNAME record pointing to `your‑github‑username.github.io`.  
3. Enable “Enforce HTTPS”.

## Contributing
Pull requests are welcome! Please open an issue first to discuss major changes.  
Follow the [Contributor Covenant](https://www.contributor-covenant.org/) code of conduct.

## License
This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

## Acknowledgements
* Inspired by the Emacs Zenburn & Solarized themes.  
* Built with ♥ by the PAREK Framework community.

