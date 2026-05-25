# pregnancy-malaysian

# 🌸 BungaTracker

**Aplikasi penjagaan kehamilan & pantang berpandukan KKM**  
*Pregnancy & postpartum tracker aligned with Malaysia's KKM guidelines*

BungaTracker is a progressive web app (PWA) that combines an **interactive pregnancy dashboard** with a **baby growth reference tool** – all in a single, offline-capable HTML file. It covers the entire journey from early pregnancy through the first 1000 days of life.

---

## ✨ Features

### 📊 Dashboard (Utama)
- **Countdown to EDD** – days remaining / post-delivery with trimester badge
- **Progress rings** – pregnancy days vs postpartum days
- **Date management** – LMP, EDD, and actual birth date
- **Kick counter** – tap to count fetal movements (KKM: from 28 weeks)
- **Contraction timer** – start/stop with session log
- **Breastfeeding tracker** – side suggestion, timer, and history
- **Appointment book** – add, view, and delete clinic visits

### 📈 Tumbesaran (Growth)
- **Fetal size slider** (Week 4–40) – CRL, estimated weight, fruit comparison
- **Maternal weight gain table** – recommended gain by pre‑pregnancy BMI (KKM)
- **Postnatal growth table** (0–12 months) – weight, length, head circumference (WHO standards)
- **Growth velocity** – expandable accordion for 0–3, 3–6, 6–12 months
- **Bar charts** – fetal weight progression & baby weight (boys/girls)  
  *(All data follows KKM/WHO references)*

### 👶 Bayi (Baby)
- **Vaccination schedule** – from birth to 18 months (BCG, Hepatitis B, 6‑in‑1, MMR, etc.)
- **Baby home checklist** – categorized by feeding, bathing, diapers, clothing, sleep, health, travel

### 🏥 KKM Content
- Quick‑view timelines for the Malaysian National Immunisation Programme (NIP) and key prenatal milestones (Buku Pink, anomaly scan, MGTT, Tdap, postnatal visits)

### 🍲 Menu Pantang
- 6 sets of postpartum meal plans with recipes and grocery lists (modal + copy to WhatsApp)

### 📋 Senarai (Lists)
- **Hospital bag checklist**
- **Personal shopping list** (add/edit)
- **Pantang recipes & tips**
- **Pantang habits tracker**
- **Post‑delivery rituals** (urutan, jamu, uri)

### 🔒 Privacy & Storage
- All data saved **locally** in `localStorage`
- Optional **Google Sheet cloud backup** – just plug in your Apps Script URL
- No external databases, no tracking

### 📱 PWA Ready
- Works **offline** after first load
- Installable on Android/iOS home screen
- Standalone display with pink KKM theme

---

## 🚀 Quick Start

1. **Download** the single HTML file (e.g., `index.html`).
2. **Open it** directly in any modern browser (Chrome, Edge, Safari, Firefox).
3. That’s it! No build tools, no server needed.

### Install as PWA (Mobile)
- **Android**: Open in Chrome, tap the menu (⋮) → "Add to Home screen".
- **iOS**: Open in Safari, tap the Share button → "Add to Home Screen".

---

## ⚙️ Customization

### Enable Google Sheets Backup
1. Create a Google Apps Script web app that accepts POST requests with JSON.
2. Copy the deployment URL.
3. In the code, replace `'YOUR_WEBAPP_URL'` with your URL:
   ```javascript
   const WEBAPP_URL = 'https://script.google.com/macros/s/.../exec';