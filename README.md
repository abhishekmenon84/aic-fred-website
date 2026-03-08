# 🍁 AIC Fredericton – Official Website

**Association of Indo-Canadians, Fredericton, New Brunswick**  
🌐 [aicfred.org](https://aicfred.org)

---

## About This Project

This is the official website for the **Association of Indo-Canadians (AIC) Fredericton** — a non-profit organization dedicated to fostering a vibrant, inclusive, and engaged Indo-Canadian community in New Brunswick.

Built with pure HTML5, Tailwind CSS, and vanilla JavaScript. Fully static — hosted on GitHub Pages with a custom domain.

---

## 📁 Project Structure

```
aic-fred-website/
├── index.html          ← Main website (single-page)
├── data/
│   └── events.json     ← ✏️ EDIT THIS to add/update events
├── assets/
│   └── logo.jpeg       ← AIC logo
├── CNAME               ← Custom domain config for GitHub Pages
└── README.md           ← This file
```

---

## 🚀 Deployment – GitHub Pages

### Step 1: Create the Repository

1. Go to [github.com](https://github.com) → **New Repository**
2. Name it exactly: `aic-fred-website`
3. Set visibility to **Public**
4. Click **Create Repository**

### Step 2: Upload Files

**Option A – GitHub Web UI (easiest):**
1. Open your new repo on GitHub
2. Click **Add file → Upload files**
3. Drag and drop all files (maintaining the folder structure)
4. Commit changes

**Option B – Git CLI:**
```bash
git init
git add .
git commit -m "Initial AIC Fredericton website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/aic-fred-website.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages** (left sidebar)
2. Under **Source**, select: `Deploy from a branch`
3. Branch: `main` | Folder: `/ (root)`
4. Click **Save**

Your site will be live at: `https://YOUR_USERNAME.github.io/aic-fred-website/`

---

## 🌐 Custom Domain Setup (aicfred.org)

### Step 4: Configure GitHub

1. In **Settings → Pages**, scroll to **Custom domain**
2. Enter: `aicfred.org`
3. Click **Save** (this creates/uses the `CNAME` file)
4. Check **Enforce HTTPS** ✅

### Step 5: Configure Your DNS Provider

Log into your domain registrar (where you bought `aicfred.org`) and add these DNS records:

| Type  | Name | Value                   |
|-------|------|-------------------------|
| A     | @    | 185.199.108.153         |
| A     | @    | 185.199.109.153         |
| A     | @    | 185.199.110.153         |
| A     | @    | 185.199.111.153         |
| CNAME | www  | YOUR_USERNAME.github.io |

> ⏳ DNS changes can take 24–48 hours to propagate globally.

---

## ✏️ How to Add/Update Events

Edit the file `data/events.json`. Each event follows this structure:

```json
{
  "id": 7,
  "title": "Event Name",
  "date": "2026-12-15",
  "time": "6:00 PM – 9:00 PM",
  "location": "Venue Name, Fredericton, NB",
  "description": "Short description of the event.",
  "category": "Cultural",
  "image": "🎉",
  "register": "https://your-google-form-link.com"
}
```

**Available categories:** `Cultural` | `Gala` | `Community` | `Arts` | `Education`

After editing, commit and push to GitHub — the site updates automatically.

---

## 🔗 Connect Google Form

1. Go to [forms.google.com](https://forms.google.com)
2. Create a form (Name, Email, Phone, Role, Message)
3. Click **Send → Link** and copy the URL
4. In `index.html`, replace `https://forms.google.com` with your form URL
5. Also update the same in `data/events.json` for each event's `register` link

---

## 🛠️ Recommended Free Tools

| Purpose | Tool | Link |
|---------|------|-------|
| Code Editor | VS Code | [code.visualstudio.com](https://code.visualstudio.com) |
| Version Control | GitHub Desktop | [desktop.github.com](https://desktop.github.com) |
| Image Optimization | Squoosh | [squoosh.app](https://squoosh.app) |
| Forms | Google Forms | [forms.google.com](https://forms.google.com) |
| Email Newsletter | Mailchimp (free tier) | [mailchimp.com](https://mailchimp.com) |
| Analytics | Google Analytics | [analytics.google.com](https://analytics.google.com) |
| SEO Check | Google Search Console | [search.google.com/search-console](https://search.google.com/search-console) |

---

## 📬 Contact

- Email: info@aicfred.org  
- Website: [aicfred.org](https://aicfred.org)

---

*Made with ❤️ for the Indo-Canadian community in Fredericton, NB*
