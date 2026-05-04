# My Personal Academic Website Template

A clean, minimal researcher portfolio built with pure HTML/CSS/JS, not a lot of frameworks, no build tools, no dependencies. Just one file.

This was my personal attempt at building (vibe coded a whole lot) a research presence online. I wanted something that felt human, not templated, and something that could sit next to researcher websites that inspire me. If you're a PhD student, postdoc, or early-career researcher who wants a professional web presence, feel free to fork this, make it yours, and give back when you can.

---

## ✨ Features

- **Single `index.html`** — no npm, no build step, no dependencies to install
- **Responsive** — works on mobile, tablet, and desktop with a collapsing sidebar
- **Sticky sidebar** with photo, identity block, live news feed, and social links
- **Publications section** with expandable abstract and BibTeX per paper
- **Research area cards** with colored headers
- **Fellowships & Honors** section
- **Experience** grouped by institution with color-coded banners
- **Teaching & Service** in a two-column layout
- **Opportunities & Mentees** section
- **Filmstrip photo section** with drag-to-scroll and lightbox click-to-expand
- **Scrollytelling** — sticky section label that tracks your scroll position
- **Pulsing live dot** on Recent News
- **Google Analytics** ready — just drop in your measurement ID
- **OG image support** for rich link previews on WhatsApp, LinkedIn, Slack
- **Favicon** support
- **Font Awesome** icons for social links

---

## 🚀 How to Use

### 1. Fork the repo
Click **Fork** at the top right of this page.

### 2. Rename your repo
For GitHub Pages to work, rename your repo to:
```
yourusername.github.io
```

### 3. Enable GitHub Pages
Go to your repo **Settings → Pages → Source → Deploy from branch → main**.

Your site will be live at `https://yourusername.github.io` within a few minutes.

### 4. Customize the content
Open `index.html` and replace the placeholder content with your own:
- Your name, photo, and identity text
- Your bio tagline
- Research area descriptions
- Publications list
- Education, experience, teaching, service
- Filmstrip photos (add images to an `img/` folder)
- Social links (Google Scholar, LinkedIn, GitHub, CV)

---

## 🎨 Customization

The easiest customization knobs are the CSS variables at the top of the `<style>` block:

```css
:root {
  --warm: #f0efe9;          /* warm background color */
  --surface: #222233;       /* topbar dark color */
  --cyan: #5bbfbf;          /* accent color */
  --sidebar-width: 255px;   /* sidebar width */
  --max-width: 1200px;      /* max layout width */
  --topbar-h: 58px;         /* topbar height */
}
```

Change `--warm` to any background color, `--cyan` to your accent, and the layout will follow.

---

## 📊 Google Analytics

Add your measurement ID to the `<head>`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🖼️ OG Image (Link Previews)

An `og-image.html` file is included — open it in Chrome, screenshot it at 1200×630px, save as `og-image.jpg`, upload to your repo root, and add to your `<head>`:

```html
<meta property="og:image" content="https://yourusername.github.io/og-image.jpg">
```

---

## 📄 License

MIT License — free to use, modify, and distribute. Attribution appreciated but not required.

If you use this template, I'd love to see what you build. Feel free to open an issue, send a message, or just drop a ⭐ on the repo.

---

Built by [Jobin Varughese](https://jobin-varughese.github.io) · Texas A&M University
