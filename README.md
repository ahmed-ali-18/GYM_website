# ⚡ IRONFORGE GYM — Website

A modern, dark-themed gym website built with pure HTML & CSS. Features animated icons, smooth scroll effects, a stat counter, and a live lead capture form powered by Formspree.

---

## 📁 Project Structure

```
ironforge-gym/
├── index.html       # Main website file
├── styles.css       # All styling and animations
└── README.md        # Project documentation
```

---

## 🖥️ Sections

| Section | Description |
|---|---|
| **Navbar** | Fixed, blur-on-scroll, mobile hamburger menu |
| **Hero** | Full-viewport with animated CTA and fire glow |
| **Ticker** | Auto-scrolling services banner |
| **Services** | 6 facility cards with unique icon animations |
| **Programs** | 3 training plans with featured highlight |
| **Stats** | Animated counters triggered on scroll |
| **Team** | 4 coach cards with hover effects |
| **Pricing** | 3 membership tiers in INR (₹) |
| **Contact Form** | Live form connected to Formspree |
| **Footer** | Brand info, links, and social handles |

---

## 🎨 Tech Stack

- **HTML5** — Semantic, clean markup
- **CSS3** — Custom properties, animations, grid, flexbox
- **Google Fonts** — Bebas Neue + Barlow + Barlow Condensed
- **Formspree** — Form backend (no server needed)
- **Vanilla JS** — Counter animation, navbar scroll, mobile menu

---

## 🔥 Animated Icons

Each service card has a unique CSS animation:

| Icon | Animation |
|---|---|
| 🏋️ Free Weights | Pulse (scale up/down) |
| ⚡ HIIT Arena | Spin (continuous rotate) |
| 🥊 Combat Studio | Bounce (vertical jump) |
| 🧘 Yoga & Recovery | Float (gentle up/down) |
| 🚴 Cycling Studio | Rotate (side to side) |
| 🏆 Elite Coaching | Shake (horizontal jitter) |

---

## 📬 Formspree Integration

This project uses **Formspree** to collect free trial form submissions and deliver them to your email inbox.

### How It Works

```
User fills the form → Clicks Submit
        ↓
Formspree receives the data
        ↓
Email sent to your inbox instantly
        ↓
Thank you message shown to user ✅
```

### Fields Captured

- First Name
- Last Name
- Email Address
- Phone Number
- Program of Interest

### Setup Steps

1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form → name it `IronForge Free Trial`
3. Copy your unique endpoint URL:
   ```
   https://formspree.io/f/YOUR_FORM_ID
   ```
4. In `index.html`, locate the `<form>` tag and update the `action` attribute:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
5. Save and deploy — submissions will arrive in your email ✅

### Spam Protection

The form includes a hidden honeypot field to block bots:
```html
<input type="text" name="_gotcha" style="display:none" />
```

### Free Plan Limit

> ⚠️ Formspree free plan allows **50 submissions/month**.
> Upgrade to the Basic plan (≈ ₹830/mo) for 1,000 submissions/month.

---

## 🚀 Getting Started

### Run Locally

No build tools or installation needed.

```bash
# 1. Clone or download the project
git clone https://github.com/yourusername/ironforge-gym.git

# 2. Open the folder
cd ironforge-gym

# 3. Open in browser
open index.html
```

Or simply double-click `index.html` — it opens directly in any browser.

### Deploy Online (Free)

| Platform | Steps |
|---|---|
| **GitHub Pages** | Push to GitHub → Settings → Pages → Deploy from main |
| **Netlify** | Drag & drop the project folder at netlify.com |
| **Vercel** | Import GitHub repo at vercel.com → auto deploys |

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout |
|---|---|
| `> 1024px` | Full desktop layout |
| `≤ 1024px` | 2-column grids, stacked programs |
| `≤ 768px` | Single column, hamburger menu |
| `≤ 480px` | Compact hero, stacked buttons |

---

## 🎨 Color Palette

| Variable | Value | Usage |
|---|---|---|
| `--bg` | `#0a0a0a` | Main background |
| `--surface` | `#1a1a1a` | Cards & surfaces |
| `--fire` | `#ff4500` | Primary accent (orange-red) |
| `--fire-lite` | `#ff6a35` | Hover state |
| `--gold` | `#f5c518` | Highlights |
| `--white` | `#ffffff` | Headings |
| `--grey-2` | `#888888` | Body text |

---

## ✏️ Customization Guide

| What to change | Where |
|---|---|
| Gym name & logo | `index.html` → `.nav-logo` and footer |
| Colors | `styles.css` → `:root` CSS variables |
| Pricing (₹) | `index.html` → `.pricing` section |
| Location & phone | `index.html` → `.contact-info` |
| Coach names & bios | `index.html` → `.team` section |
| Formspree endpoint | `index.html` → `<form action="...">` |

---

## 🔮 Future Improvements

- [ ] Add Google Sheets integration for unlimited lead storage
- [ ] Add WhatsApp notifications via CallMeBot
- [ ] Add a photo gallery section
- [ ] Add class schedule / timetable
- [ ] Add Google Maps embed
- [ ] Add testimonials / reviews section

---

