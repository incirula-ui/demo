# PTI International — Precision Dental Implant Systems

A modern, responsive website for PTI International, showcasing premium titanium dental implant systems with advanced 3D visualization, smooth animations, and comprehensive multi-language support.

## 🌟 Features

- **Interactive 3D Model Viewer** — Real-time 3D dental implant visualization with scroll-driven rotation and HUD readout
- **Multi-Language Support** — 7 languages: English, Turkish, German, French, Spanish, Russian, Arabic (with RTL support)
- **Smooth Animations** — GSAP-powered scroll animations, hover effects, and transitions
- **Responsive Design** — Mobile-first approach with Tailwind CSS
- **Professional UI Components**
  - Interactive specifications table
  - Expandable FAQ section
  - Certification showcase
  - Product catalog with feature cards
  - Contact and CTA sections
  - Footer with social links

- **SEO Optimized** — Semantic HTML, proper meta tags, structured content
- **Performance Optimized** — CDN-based resources, efficient CSS/JS, proper caching headers

## 📋 Tech Stack

- **HTML5** — Semantic markup
- **Tailwind CSS 3** — Utility-first styling
- **GSAP 3** — Advanced animations & scroll triggers
- **Model Viewer 3.4** — 3D model visualization
- **Google Fonts** — Professional typography (Space Grotesk, Inter, IBM Plex Mono)

## 🎨 Color Palette

```
Ink:     #0B1526 (Primary dark)
Paper:   #F5F6F3 (Background)
Steel:   #5B6672 (Secondary text)
Line:    #D7DCDA (Borders)
Cyan:    #0E9FC4 (Accent primary)
Bronze:  #B78A3F (Accent secondary)
Sage:    #6B8E7F (Accent tertiary)
```

## 📦 Project Structure

```
/workspaces/demo/
├── index.html          # Main website file (all-in-one)
├── vercel.json         # Vercel deployment config
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## 🚀 Getting Started

### Local Development

1. Clone the repository
```bash
git clone https://github.com/incirula-ui/demo.git
cd demo
```

2. Open in browser
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js http-server
npx http-server

# Or simply open index.html in your browser
```

3. Access at `http://localhost:8000`

### Deployment to Vercel

#### Option 1: Using Vercel CLI
```bash
npm i -g vercel
vercel
```

#### Option 2: Using GitHub
1. Push to GitHub repository
2. Connect repository to Vercel at https://vercel.com/new
3. Vercel will auto-deploy on push

## 📱 Responsive Breakpoints

- Mobile: < 640px
- Tablet: 640px - 1024px
- Desktop: > 1024px

## 🌐 Multi-Language Keys

All translatable content uses `data-i18n` attributes. Supported languages:
- `en` — English
- `tr` — Turkish (Türkçe)
- `de` — German (Deutsch)
- `fr` — French (Français)
- `es` — Spanish (Español)
- `ru` — Russian (Русский)
- `ar` — Arabic (العربية)

## 🔧 Key Features Breakdown

### 3D Model Viewer
- Interactive implant visualization
- Scroll-driven rotation (0-1440°)
- Live HUD readout showing rotation angle
- Specifications display panel
- Loading state handling

### Animation System
- GSAP ScrollTrigger integration
- Staggered reveal animations on scroll
- Smooth card transitions
- Hover state animations
- Floating and glow effects

### Interactive Elements
- Language switcher (desktop & mobile)
- Expandable FAQ with details element
- Smooth anchor navigation
- Hover effects on all interactive components
- Responsive navigation bar

## 📊 Content Sections

1. **Hero Section** — Brand positioning with 3D model and key stats
2. **Product Phases** — 3-phase implantation process visualization
3. **Statistics Strip** — Key metrics and achievements
4. **Product Catalog** — 3 main product categories
5. **Technical Specifications** — Detailed specs with comparison table
6. **Why PTI** — 4 key differentiators
7. **Certifications** — Global quality certifications
8. **FAQ** — 5 common questions
9. **Contact/CTA** — Call-to-action section
10. **Footer** — Company info, links, social media

## ♿ Accessibility

- Semantic HTML structure
- ARIA labels on form elements
- Proper heading hierarchy
- Color contrast compliance
- Keyboard navigation support
- Mobile-friendly touch targets

## 📈 Performance Metrics

- **First Contentful Paint (FCP)** — < 1s
- **Largest Contentful Paint (LCP)** — < 2.5s
- **Cumulative Layout Shift (CLS)** — < 0.1
- **Time to Interactive (TTI)** — < 3.5s

## 🔒 Security Headers

```
X-Content-Type-Options: nosniff
X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
Cache-Control: public, max-age=3600
```

## 📝 License

© 2026 PTI International. All rights reserved.

## 👨‍💼 Support

For inquiries, contact: info@pti-international.com

---

**Last Updated:** August 2026