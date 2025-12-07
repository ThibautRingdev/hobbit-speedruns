# 🏃‍♂️ Hobbit Speedruns

> Community website for speedrunners of *The Hobbit* (2003) developed by Sierra Entertainment

[![Built with Astro](https://astro.badg.es/v2/built-with-astro/tiny.svg)](https://astro.build)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Live Site:** [hobbitspeedruns.com](https://hobbitspeedruns.com) *(coming soon)*

---

## 🎮 About

This is a modern rebuild of the Hobbit Speedruns community website, serving as a hub for speedrunners of the 2003 game *The Hobbit*. The site features comprehensive guides, resources, and serves as an accessible entry point for newcomers to the speedrunning community.

This project is a companion to the official [speedrun.com leaderboards](https://www.speedrun.com/hobbit), not a replacement.

---

## ✨ Features

- 📚 **Comprehensive Guides** - Detailed tutorials for all skill levels
- 🔗 **Curated Resources** - Links to tools, timers, and community spaces
- ⚡ **Lightning Fast** - Built with Astro for optimal performance
- 📱 **Fully Responsive** - Works beautifully on all devices
- 🎨 **Modern Design** - Clean, accessible interface with Tailwind CSS
- 🎱 **Adding Bingo Board Features** - A new Gamemode for all Runner
- 🌐 **Adding New Wiki Page** - To know how to route and practice bingo.

---

## 🚀 Quick Start

### Prerequisites

- Node.js 18.20.8+ or 20.3.0+ or 22.0.0+
- npm 9.6.5+ or pnpm 7.1.0+

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/hobbit-speedruns.git
cd hobbit-speedruns

# Install dependencies
npm install

# Start development server
npm run dev
```

Visit `http://localhost:4321` to see your site!

---

## 🛠️ Tech Stack

- **[Astro](https://astro.build)** - Static site generator for content-focused websites
- **[Tailwind CSS](https://tailwindcss.com)** - Utility-first CSS framework
- **[TypeScript](https://www.typescriptlang.org/)** - Type-safe JavaScript
- **[MDX](https://mdxjs.com/)** - Markdown with JSX for dynamic content

---

## 📂 Project Structure

```
hobbit-speedruns/
├── src/
│   ├── layouts/
│   │   └── Layout.astro          # Main layout with nav & footer
│   ├── pages/
│   │   ├── index.astro           # Homepage
│   │   ├── guides.astro          # Guides listing
│   │   ├── guides/
│   │   │   └── [slug].astro      # Individual guide pages
│   │   └── resources.astro       # Resources page
│   └── content/
│       └── guides/               # MDX guide files
├── public/
│   └── favicon.svg
├── astro.config.mjs
├── tailwind.config.mjs
├── tsconfig.json
└── package.json
```

---

## 📝 Adding Content

### Adding a New Guide

1. Create a new `.mdx` file in `src/content/guides/`:

```mdx
---
title: "Your Guide Title"
description: "Brief description of the guide"
icon: "🎮"
order: 1
---

# Your Guide Content

Write your guide using Markdown...
```

2. The guide will automatically appear on the guides page!

### Adding a Resource

Edit `src/pages/resources.astro` and add to the `resources` array:

```javascript
{
  name: "Resource Name",
  description: "What this resource does",
  url: "https://example.com"
}
```

---

## 🚢 Deployment

### Deploy to Vercel (Recommended)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

Or connect your GitHub repo to [Vercel](https://vercel.com) for automatic deployments.

### Deploy to Netlify

```bash
# Build the site
npm run build

# Deploy the dist/ folder to Netlify
```

### Other Platforms

The site can be deployed to any static hosting service. Just run `npm run build` and upload the `dist/` folder.

---

## 🧞 Commands

| Command                | Action                                           |
| :--------------------- | :----------------------------------------------- |
| `npm install`          | Install dependencies                             |
| `npm run dev`          | Start dev server at `localhost:4321`             |
| `npm run build`        | Build production site to `./dist/`               |
| `npm run preview`      | Preview built site locally                       |
| `npm run astro ...`    | Run Astro CLI commands                           |

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-guide`)
3. **Commit your changes** (`git commit -m 'Add amazing guide'`)
4. **Push to the branch** (`git push origin feature/amazing-guide`)
5. **Open a Pull Request**

### Contribution Ideas

- 📝 Write new guides or improve existing ones
- 🐛 Report bugs or suggest features via [Issues](https://github.com/ThibautRingdev/hobbit-speedruns/issues)
- 🎨 Improve the design or user experience
- 🔗 Add helpful resources for the community

---

## 🙏 Acknowledgments

- Original website by [milankarman](https://github.com/milankarman)
- The Hobbit speedrunning community
- [Sierra Entertainment](https://en.wikipedia.org/wiki/Sierra_Entertainment) for the original game

---

## 📞 Contact & Community

- **Discord:** [Join our community](https://discord.gg/uHRANWgUYZ)
- **Leaderboards:** [speedrun.com/hobbit](https://www.speedrun.com/hobbit)
- **Issues:** [GitHub Issues](https://github.com/ThibautRingdev/hobbit-speedruns/issues)

---

<p align="center">Made with ❤️ by the Hobbit Speedrunning Community</p>
