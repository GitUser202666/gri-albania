# GRI-albania.net — Udhëzime për GitHub Pages

## HAPI 1 — Krijo repository në GitHub

1. Hap **github.com** dhe hyr me llogarinë `GitUser202666`
2. Trokit butonin **"+"** (lart djathtas) → **"New repository"**
3. **Repository name:** shkruaj saktësisht: `gri-albania`
4. Zgjidh **"Public"**
5. **MOS** checkbox-in "Add a README file"
6. Trokit **"Create repository"**

---

## HAPI 2 — Ngarko skedaret

Pas krijimit, GitHub të tregon një faqe bosh. Trokit **"uploading an existing file"**.

Zgjidh të gjithë skedaret që janë brenda dosjes `gri-albania/`:
- `_config.yml`
- `Gemfile`
- `index.html`
- `rreth.md`
- Dosjet: `_layouts/`, `_posts/`, `assets/`

Trokit **"Commit changes"** (buton jeshil poshtë).

---

## HAPI 3 — Aktivizo GitHub Pages

1. Shko tek **Settings** (lart në repository)
2. Klik **"Pages"** nga menuja e majtë
3. Te **"Source"** → zgjidh **"Deploy from a branch"**
4. Branch: **main** → Folder: **/ (root)**
5. Trokit **"Save"**

Pas 2-3 minutash faqja del live tek:
**https://GitUser202666.github.io/gri-albania**

---

## SI TË PUBLIKOSH SHKRIM TË RI NGA TELEFONI

### Metoda 1 — GitHub App (rekomandoj)

1. Hap **GitHub app** në telefon
2. Shko tek repository `gri-albania`
3. Hap dosjen **`_posts/`**
4. Trokit **"+"** → **"Create new file"**
5. Emri i skedarit duhet të jetë në këtë format:
   ```
   2025-05-21-titulli-shkrimit.md
   ```
6. Kopjo këtë template dhe plotëso:

```markdown
---
layout: post
title: "Titulli i plotë i shkrimit"
date: 2025-05-21
category: "Analizë Politike"
published: true
excerpt: "Një fjali e shkurtër që përshkruan shkrimin."
---

Teksti i shkrimit shkon këtu.

Paragrafi i dytë...

## Nëntitulli (opsional)

Vazhdo me tekstin...
```

7. Trokit **"Commit changes"**
8. Faqja përditësohet automatikisht brenda **2 minutash** ✓

### Kategorite e disponueshme:
- `"Analizë Politike"`
- `"Letërsi"`

---

## SI TË FSHEHËSH NJË SHKRIM (Draft)

Ndrysho në krye të skedarit:
```
published: false
```

---

## SI TË SHTOSH FOTO

1. Ngarko foton në dosjen `assets/img/` në GitHub
2. Në shkrim shto:
```
cover: /assets/img/emri-fotos.jpg
```

---

## DOMAIN PERSONAL (opsional)

Nëse dëshiron `gri-albania.net` si adresë:
1. Blej domain tek Namecheap / GoDaddy
2. Settings → Pages → "Custom domain" → shkruaj `gri-albania.net`
3. Te domain provider shto CNAME record që tregon tek `GitUser202666.github.io`
