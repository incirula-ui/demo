# 🚀 Vercel Deployment Guide — PTI International Website

Complete step-by-step instructions to deploy the PTI International website to Vercel.

## ✅ Prerequisites

- GitHub account (with repository: https://github.com/incirula-ui/demo)
- Vercel account (free at https://vercel.com)

## 📋 Option 1: Deploy via Vercel Dashboard (Recommended)

### Step 1: Connect GitHub Repository
1. Go to https://vercel.com/new
2. Click **"Import Project"**
3. Paste repository URL: `https://github.com/incirula-ui/demo`
4. Click **"Import"**

### Step 2: Configure Project
- **Framework Preset:** Select "Other" (it's a static site)
- **Build Command:** Leave empty or set to `echo 'Static site'`
- **Output Directory:** Leave empty (uses root)
- **Environment Variables:** None needed

### Step 3: Deploy
1. Click **"Deploy"**
2. Wait for deployment to complete (usually 1-2 minutes)
3. Get your live URL: `https://demo-[unique-id].vercel.app`

✨ Your site is now live!

---

## 📋 Option 2: Deploy via Vercel CLI

### Step 1: Install Vercel CLI
```bash
npm install -g vercel
# or
yarn global add vercel
```

### Step 2: Authenticate
```bash
vercel login
# Follow prompts to authenticate with GitHub
```

### Step 3: Deploy
```bash
cd /workspaces/demo
vercel
```

### Step 4: Follow Prompts
```
? Set up and deploy "~/workspaces/demo"? [Y/n] y
? Which scope do you want to deploy to? [your-account]
? Link to existing project? [y/N] n
? What's your project's name? demo
? In which directory is your code located? ./
? Want to modify these settings? [y/N] n
```

✨ Deployment complete!

---

## 🔧 Project Configuration Details

### vercel.json Configuration
```json
{
  "version": 2,
  "buildCommand": "echo 'Static site - no build needed'",
  "outputDirectory": ".",
  "routes": [{
    "src": "/(.*)",
    "dest": "/index.html"
  }],
  "headers": [{
    "source": "/(.*)",
    "headers": [
      { "key": "Cache-Control", "value": "public, max-age=3600" },
      { "key": "X-Content-Type-Options", "value": "nosniff" },
      { "key": "X-Frame-Options", "value": "SAMEORIGIN" }
    ]
  }]
}
```

### Static Files
- ✅ `index.html` — Main website file (1066 lines, all-in-one)
- ✅ `vercel.json` — Deployment configuration
- ✅ `.gitignore` — Git exclusion rules
- ✅ `README.md` — Project documentation

---

## 🌍 Live URL

After deployment, access your site at:
- **Production:** `https://[project-name].vercel.app`
- **Preview:** Available for each Git push

Example: `https://pti-international.vercel.app`

---

## 📊 What's Included

### Features Deployed
- ✅ Interactive 3D dental implant viewer (model-viewer library)
- ✅ 7-language support (EN, TR, DE, FR, ES, RU, AR)
- ✅ RTL support for Arabic
- ✅ GSAP animations & scroll triggers
- ✅ Responsive Tailwind CSS design
- ✅ Technical specifications table
- ✅ Product catalog
- ✅ Certifications showcase
- ✅ Expandable FAQ
- ✅ Contact CTAs
- ✅ Professional footer

### External Resources (CDN)
- Tailwind CSS 3
- GSAP 3.12.2
- ScrollTrigger plugin
- Google Fonts (Space Grotesk, Inter, IBM Plex Mono)
- Model Viewer 3.4.0
- 3D Model: GitHub raw content

---

## 🔍 Testing After Deployment

### Checklist
- [ ] Homepage loads correctly
- [ ] Language switcher works (all 7 languages)
- [ ] 3D model rotates on scroll
- [ ] HUD readout updates with rotation angle
- [ ] Smooth animations on scroll
- [ ] FAQ items expand/collapse
- [ ] Navigation links work
- [ ] Mobile responsive (test on phone)
- [ ] No console errors (check DevTools)
- [ ] Page loads in < 3 seconds

---

## 🔗 Useful Links

- **Vercel Dashboard:** https://vercel.com/dashboard
- **GitHub Repository:** https://github.com/incirula-ui/demo
- **Project Analytics:** https://vercel.com/dashboard/project/[project-id]
- **Domain Management:** https://vercel.com/dashboard/domains
- **Environment Variables:** https://vercel.com/dashboard/project/[project-id]/settings/environment-variables

---

## 🚨 Troubleshooting

### Issue: 3D model not loading
**Solution:** Model URL requires external access. Check CDN availability.

### Issue: Styles not loading
**Solution:** Tailwind CSS loads from CDN. Check internet connection.

### Issue: Languages not switching
**Solution:** Check browser console for JavaScript errors. Reload page.

### Issue: Animations not smooth
**Solution:** This is expected on slow devices. Animations are GPU-accelerated.

---

## 📝 Custom Domain (Optional)

To add a custom domain:
1. Go to Vercel Dashboard → Project Settings → Domains
2. Add your domain (e.g., `pti-international.com`)
3. Configure DNS records as instructed
4. Wait for SSL certificate (automatic)

---

## 🔄 Continuous Deployment

**Auto-Deploy on Push:**
Every time you push to `main` branch, Vercel automatically:
1. Detects changes
2. Builds project (if needed)
3. Runs tests (if configured)
4. Deploys to production
5. Creates preview deployment for PRs

---

## 📞 Support

For deployment issues:
- Check Vercel documentation: https://vercel.com/docs
- Review build logs in Vercel Dashboard
- Check GitHub Issues: https://github.com/incirula-ui/demo/issues

---

**Last Updated:** August 2026
**Status:** ✅ Ready for Production
