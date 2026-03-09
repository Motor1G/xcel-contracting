# Xcel Contracting Website — Next Steps for Gary

## ✅ What's Done
- Complete 5-page static website built in `/Users/Rex/.openclaw/workspace/xcel-site/`
- All images copied and named correctly
- Git initialized and first commit made
- Ready to push to GitHub

---

## 1. Create the GitHub Repo (2 min)
1. Go to: https://github.com/new
2. Login as Motor1G
3. Repository name: **xcel-contracting**
4. Set to **Public**
5. Do NOT initialize with README, .gitignore, or license
6. Click **Create Repository**

---

## 2. Push the Code
Tell Rex: "The repo is created, push the code" and Rex will handle it.

---

## 3. Deploy on Netlify (5 min — free!)
1. Go to: https://app.netlify.com
2. Sign up / login with your GitHub account
3. Click **"Add new site" → "Import an existing project"**
4. Choose **GitHub** → authorize Netlify
5. Select the **Motor1G/xcel-contracting** repo
6. Build settings:
   - Build command: (leave blank)
   - Publish directory: `.` (just a dot)
7. Click **Deploy Site**
8. Your site will be live at something like `https://xcel-contracting-abc123.netlify.app`

---

## 4. Connect Your Custom Domain (xcelcontracting.com)
Once deployed on Netlify:
1. In Netlify → Site Settings → Domain Management
2. Click **Add custom domain** → enter `xcelcontracting.com`
3. Update your domain registrar's nameservers to point to Netlify (they'll give you the NS records)
4. Netlify provides free SSL automatically

---

## 5. Set Up Formspree (for the contact form)
1. Go to: https://formspree.io
2. Create a free account
3. Create a new form → get your form ID (looks like `xabcdefg`)
4. Find and replace `REPLACE_ME` in `contact.html` and `ai-solutions.html`:
   - Change `https://formspree.io/f/REPLACE_ME`
   - To `https://formspree.io/f/YOUR_FORM_ID`
5. Push the change: `git add -A && git commit -m "Add Formspree form ID" && git push`

---

## Site Structure
```
xcel-site/
  index.html          ← Home page
  entertainment.html  ← Xcel Entertainment services
  contracting.html    ← Contracting/Remodeling services  
  ai-solutions.html   ← AI Solutions (coming soon)
  contact.html        ← Get a Quote / contact form
  assets/
    css/style.css     ← All styles
    js/main.js        ← Nav + lightbox JS
    images/           ← All project photos + logo
```

## Notes
- The contact form will go to govitt1@live.com via Formspree (after you set it up)
- The site is 100% mobile-responsive with a hamburger menu
- Gallery has a click-to-zoom lightbox on desktop and mobile
- Google Maps is embedded on the contact page (shows Meridian area)
- All pages have the same header/footer navigation
