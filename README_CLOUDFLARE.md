# Cloudflare Pages - Konfiguraatio

## ⚠️ TÄRKEÄ: Pages on erillinen palvelu!

Cloudflare Pages EI ole DNS/CDN-näkymässä. Se on oma palvelunsa.

---

## Mistä löytyy?

### 1. Cloudflare Dashboard
```
https://dash.cloudflare.com
```

### 2. Vasemmalla navigaatiossa
**Scrollaa ALASPÄIN** ja etsi:
- **"Pages"** tai
- **"Workers & Pages"** → "Pages"

### 3. Valitse Projekti
- Etsi: **"asterpay-landing"** (tai mikä on projektin nimi)
- Klikkaa projektia

### 4. Settings → Build & deployments
Tarkista:
- **Root directory:** `landing/`
- **Build output directory:** `/` (tyhjä)
- **Build command:** (tyhjä)

---

## Ongelma: /api näyttää pääsivun

### Tarkista:

1. **Build Settings:**
   - Root directory: `landing/`
   - Build output directory: `/` (tyhjä)

2. **Deployments:**
   - Deployments → Viimeisin → Preview
   - Testaa `/api/` polku

3. **Build Logs:**
   - Deployments → Viimeisin → Build log
   - Etsi: `api/index.html`

---

## Korjaus

Jos Root directory on väärä:

1. Settings → Build & deployments
2. Muuta Root directory: `landing/`
3. Muuta Build output directory: `/` (tyhjä)
4. Save
5. Deploy uudelleen

---

*Cloudflare Pages setup päivitetty: Tammikuu 2026*
