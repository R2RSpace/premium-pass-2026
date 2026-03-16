# 🎁 Google AI Pro — Exclusive Referral Invite Page

A polished, single-file HTML invitation page for sharing a **Google AI Pro** referral link. Built with pure HTML, CSS, and vanilla JS — no frameworks, no build tools, no dependencies.

---

## ✨ Preview

> Light mode and dark mode are supported automatically via `prefers-color-scheme`.

| Light | Dark |
|---|---|
| Clean white card on soft blue-grey dot grid | Deep surface card on near-black background |

---

## 🚀 Features

- **Zero dependencies** — one `.html` file, works offline (except Google Fonts)
- **Dark mode** — full `prefers-color-scheme: dark` token system
- **Reduced motion** — respects `prefers-reduced-motion`
- **Accessible** — semantic HTML, `role`, `aria-label`, `:focus-visible` outlines
- **Responsive** — fluid down to 320px, `max-width: 408px` card
- **Material Design 3 inspired** — 8px spacing grid, elevation system, ripple effect
- **Animated** — staggered entrance, Gemini star pulse, gradient text shift, coupon progress bar
- **Coupon UX** — visual discount block showing `Rp 1.236.000 → Rp 0` to communicate 4-month free value without ambiguous "free trial" wording

---

## 📁 Structure

```
.
└── index.html   # Everything — styles, markup, and script in one file
```

---

## 🛠️ Usage

### 1. Clone or download

```bash
git clone https://github.com/your-username/google-ai-pro-invite.git
cd google-ai-pro-invite
```

### 2. Edit your referral link

Open `index.html` and find the CTA anchor, then replace the `href` with your own referral URL:

```html
<a href="https://g.co/g1referral/YOURCODE" class="cta" ...>
```

### 3. Edit your name

Replace the two occurrences of `Ridho Eka Putra` with your own name:

```html
<!-- Badge -->
Exclusive Gifts from Ridho Eka Putra

<!-- og:description meta tag -->
<meta property="og:description" content="Ridho Eka Putra mengundang ...">
```

### 4. Deploy

Drop `index.html` anywhere that serves static files:

- **GitHub Pages** — push to `main`, enable Pages in repo settings, set source to `/ (root)`
- **Vercel / Netlify** — drag and drop the file
- **Any static host** — upload as `index.html`

---

## 🎨 Customisation

All visual tokens live in `:root` at the top of the `<style>` block. Common overrides:

| Token | Default (light) | Purpose |
|---|---|---|
| `--pri` | `#1a6cf5` | Button & accent color |
| `--pri-tint` | `#e8f0fe` | Badge & icon backgrounds |
| `--sur-card` | `#ffffff` | Card surface |
| `--r-card` | `24px` | Card corner radius |

To change the referral price displayed, update the `.hero-price` text and the `.coupon-original` value:

```html
<p class="hero-price">Rp&nbsp;309.000<span class="unit">/bln</span></p>
...
<span class="coupon-original">Rp&nbsp;1.236.000</span>  <!-- 4 × monthly price -->
```

---

## 📐 Design System

| Layer | Spec |
|---|---|
| Spacing | 8px base grid (`--sp-2` → `--sp-48`) |
| Type scale | 11 / 12 / 13 / 14 / 15 / 34px |
| Fonts | Google Sans Display (hero), Google Sans (UI), Roboto (fallback) |
| Radius | `--r-pill` 999px · `--r-card` 24px · `--r-inner` 12px |
| Shadows | `--shadow-xs / sm / md` — layered two-stop rgba |
| Motion | `--ease-out` `.05,.7,.1,1` · `--ease-std` `.2,0,0,1` |

---

## 📄 License

MIT — do whatever you want, attribution appreciated but not required.
