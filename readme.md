# 🎨 Coloring Book Generator

A free, lightweight web app that generates optimized AI prompts for creating printable coloring book pages. Built for [RLB Designs](https://rlbdesigns.com).

**[Live Demo →](https://coloring.rlbdesigns.com)**

---

## What It Does

1. You describe a scene (e.g. *"dolphin jumping out of the ocean near a butterfly"*)
2. Pick a coloring style — Classic, Detailed, Mandala, or Cartoon
3. The app builds an optimized prompt tuned for black-and-white line art
4. Open any free image generator, paste the prompt, and download your coloring page

---

## Free Image Generators Supported

| Generator | Free Tier | Notes |
|---|---|---|
| [Bing Image Creator](https://www.bing.com/images/create) | ✅ No account needed | Powered by DALL-E 3 — easiest to use |
| [Adobe Firefly](https://firefly.adobe.com) | ✅ Free tier | High quality results |
| [Ideogram](https://ideogram.ai) | ✅ Free tier | Excellent for line art |
| [Google AI Studio (Imagen)](https://aistudio.google.com/generate-image) | ✅ Free | Imagen 3 model |

> Need help using these tools? Visit [rlbdesigns.com](https://rlbdesigns.com) for step-by-step instructions.

---

## Tech Stack

- Pure HTML, CSS, and vanilla JavaScript
- Zero dependencies — no React, no Node, no build step
- Single file: `index.html`

---

## Deployment

This project is hosted on **Cloudflare Pages** connected to this GitHub repo.

### Deploy Your Own Copy

1. **Fork this repo**

2. **Connect to Cloudflare Pages**
   - Go to [dash.cloudflare.com](https://dash.cloudflare.com) → Workers & Pages → Create → Pages
   - Connect your forked GitHub repo
   - Leave all build settings blank (static HTML, no build needed)
   - Click Deploy

3. **Add a custom domain** *(optional)*
   - In Cloudflare Pages → your project → Custom domains
   - Add your domain (e.g. `coloring.yourdomain.com`)
   - DNS is configured automatically if your domain is on Cloudflare

### Run Locally

No install or server needed — just open the file directly in your browser:

```bash
git clone https://github.com/YOUR_USERNAME/coloring-book-generator.git
cd coloring-book-generator
open index.html
```

---

## Project Structure

```
coloring-book-generator/
└── index.html      # Entire app — HTML, CSS, and JS in one file
└── README.md       # This file
```

---

## Customization

All configuration is at the top of the `<script>` block in `index.html`:

- **`EXAMPLES`** — the example scene chips shown under the input
- **`STYLES`** — coloring styles and their prompt modifiers
- **`STYLE_MAP`** — the prompt text appended for each style
- **`LAUNCHERS`** — image generator links (add/remove as needed)

---

## License

MIT — free to use, modify, and distribute.

---

*Made with ❤️ by [RLB Designs](https://rlbdesigns.com)*
