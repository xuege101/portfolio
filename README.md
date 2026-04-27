# Francis Tan - DevOps Engineer Portfolio

A highly performant, fully static, and visually stunning personal portfolio built for DevOps Engineers. It features a sleek glassmorphic UI, a dynamic particles background, and smooth page transitions.

Built with **Astro**, **Tailwind CSS v4**, and **GSAP**.

## 🚀 Features

- **Blazing Fast**: Static Site Generation (SSG) via Astro for instant load times.
- **Glassmorphic UI**: Beautiful translucent styling that adapts seamlessly to both Light and Dark modes.
- **Dynamic Background**: Custom canvas-based ambient pipeline/particles background that reacts to theme changes.
- **GSAP Animations**: Smooth scroll-triggered reveal animations and page transitions.
- **GitHub Pages Ready**: Pre-configured with a GitHub Actions workflow for zero-hassle automated deployments.

## 🛠️ Tech Stack

- [Astro](https://astro.build/) - Web framework
- [Tailwind CSS v4](https://tailwindcss.com/) - Utility-first styling engine
- [GSAP](https://gsap.com/) - Professional-grade JavaScript animations
- [tsParticles](https://particles.js.org/) & HTML5 Canvas - Ambient backgrounds

## 📂 Project Structure

All customizable content lives inside the Astro components. You do not need to know Astro deeply to edit your information — simply open the files in `src/components/` and edit the marked variables!

```text
/
├── public/
│   ├── js/                 # Canvas animation logic (pipeline.js)
│   └── Resume_2026.pdf     # Your downloadable CV
├── src/
│   ├── components/         # Your content lives here!
│   │   ├── AboutMe.astro   # Contact info & quick summary
│   │   ├── Experience.astro# Work history & timeline
│   │   ├── Hero.astro      # Main landing page banner
│   │   ├── Projects.astro  # Project grid & details
│   │   └── TechStack.astro # Skills & certifications
│   ├── layouts/
│   │   └── Layout.astro    # Global HTML wrapper & theme logic
│   ├── pages/              # The actual route files (e.g. /about)
│   └── styles/
│       └── global.css      # Core theme variables & Tailwind setup
├── astro.config.mjs        # Astro configuration (base path, site URL)
└── .github/workflows/      # Automated deployment script for GH Pages
```

## 💻 Local Development

All commands are run from the root of the project in your terminal:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs all required dependencies |
| `npm run dev` | Starts the local dev server at `localhost:4321` |
| `npm run build` | Builds your production site into `./dist/` |

## 🌐 Deploying to GitHub Pages

1. Push this repository to your GitHub account (e.g., `xuege101/portfolio`).
2. Go to your repository **Settings** -> **Pages**.
3. Under **Build and deployment**, set the Source to **GitHub Actions**.
4. The included `.github/workflows/deploy.yml` will automatically build and deploy your site every time you push to the `main` branch!

> **Note:** If you change your repository name or GitHub username, remember to update the `site` and `base` properties inside `astro.config.mjs`!
