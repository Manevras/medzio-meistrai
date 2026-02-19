# 📖 INSTRUKCIJOS – MEDŽIO MEISTRAI SVETAINĖ

Ši instrukcija paprasta kaip A-B-C. Net 5-metis supras! 😊

---

## 📁 PROJEKTO STRUKTŪRA

```
medzio-meistrai/
│
├── index.html              ← PAGRINDINIS FAILAS (čia viskas!)
│
└── assets/
    ├── images/
    │   ├── hero-default.jpg     ← HERO nuotrauka (viršuje)
    │   ├── about-default.jpg    ← APIE MUS nuotrauka
    │   ├── project-1.jpg        ← Projektas 1
    │   ├── project-2.jpg        ← Projektas 2
    │   └── project-3.jpg        ← Projektas 3
    │
    └── videos/
        └── restoration-animation.gif   ← GIF animacija (jei naudoji)
```

---

## 🖼️ KAIP PAKEISTI NUOTRAUKAS

### Žingsnis 1 – Paruošk nuotrauką
- Optimizuok nuotrauką TinyPNG: **https://tinypng.com**
- Rekomenduojamas dydis: Hero – 1920×1080px, About – 800×1000px, Projektai – 800×800px

### Žingsnis 2 – Įkelk į tinkamą katalogą
- Nuotaukos → `assets/images/`
- GIF/Video → `assets/videos/`

### Žingsnis 3 – Pervadink failą TIKSLIAI
- Hero nuotrauka → `hero-default.jpg`
- About nuotrauka → `about-default.jpg`
- Projektai → `project-1.jpg`, `project-2.jpg`, `project-3.jpg`

### ⚠️ SVARBU: Jei naudoji savo pavadinimą:
Atidaryk `index.html` ir surask (Ctrl+F):
```
src="assets/images/hero-default.jpg"
```
Pakeisk į savo pavadinimą:
```
src="assets/images/mano-nuotrauka.jpg"
```

---

## ✏️ KAIP PAKEISTI TEKSTUS

### Atidaryk `index.html` teksto redaktoriuje (pvz. VS Code arba Notepad++)

### Pagrindinis heroaus tekstas (~eil. 155):
```html
<h2>Sugrąžiname medžiui<br>jo tikrąją vertę.</h2>
```
Pakeisk tekstą tarp `<h2>` ir `</h2>`

### Kontaktai (~eil. 230):
```html
<p class="contact-name">Nojus</p>
```
```html
<a href="tel:+37060534774" ...>+370 605 34774</a>
```
```html
<a href="mailto:medzio.meistrai.paslaugos@gmail.com" ...>
    medzio.meistrai.paslaugos@gmail.com
</a>
```

### Paslaugų kortelės (~eil. 195-220):
Kiekvienoje kortelėje rasi:
```html
<p class="service-name">Parketo restauravimas</p>
<p class="service-desc">Šlifavimas, lakavimas...</p>
```
Tiesiog pakeisk tekstą!

---

## 📱 KAIP PATIKRINTI MOBILE VERSIJĄ

1. Atidaryk `index.html` naršyklėje
2. Spausk **F12** (atsidarys Developer Tools)
3. Spausk **Ctrl+Shift+M** (Toggle Device Toolbar)
4. Viršuje pasirink „iPhone 14" arba „iPad"
5. Matai kaip atrodo telefone! ✅

---

## 🚀 KAIP DEPLOYINTI PER VERCEL

### Žingsnis 1 – Sukurk GitHub paskyrą
→ https://github.com (nemokama)

### Žingsnis 2 – Sukurk naują repozitoriją
1. Spausk žalią mygtuką „New"
2. Pavadinimas: `medzio-meistrai`
3. Spausk „Create repository"

### Žingsnis 3 – Įkelk failus į GitHub
**Per naršyklę (paprasčiausias būdas):**
1. Atidaryk savo repozitoriją GitHub
2. Spausk „uploading an existing file"
3. Vilk visus projekto failus į langą
4. Spausk „Commit changes"

**Arba per terminalą:**
```bash
git init
git add .
git commit -m "Pirmas įkėlimas"
git remote add origin https://github.com/TAVO_VARDAS/medzio-meistrai.git
git push -u origin main
```

### Žingsnis 4 – Sukurk Vercel paskyrą
→ https://vercel.com (nemokama, prisijunk per GitHub)

### Žingsnis 5 – Importuok projektą
1. Vercel → „Add New Project"
2. Pasirink `medzio-meistrai` iš GitHub
3. Spausk „Deploy"
4. ✅ Po 1 minutės svetainė veikia!

**Gautas adresas:** `https://medzio-meistrai.vercel.app`

---

## 🌐 KAIP SUSIETI SU DOMENAI.LT DOMENU

### Žingsnis 1 – Nusipirk domeną
→ https://domenai.lt
- Ieškoki `medzio-meistrai.lt`
- Kaina ~10-15€/metai

### Žingsnis 2 – Prijunk prie Vercel
1. Vercel → tavo projektas → „Settings" → „Domains"
2. Įrašyk: `medzio-meistrai.lt`
3. Vercel parodys Nameservers (pvz. `ns1.vercel-dns.com`)

### Žingsnis 3 – Pakeisk Nameservers Domenai.lt
1. Domenai.lt → prisijunk → „Mano domenai"
2. Spausk ant domeno → „DNS / Nameservers"
3. Pakeisk į Vercel Nameservers
4. Palaukit 1-6 valandas ⏳

### Žingsnis 4 – Gotova! ✅
`https://medzio-meistrai.lt` veikia su automatiniu SSL (HTTPS)

---

## ❓ DAŽNIAUSIOS PROBLEMOS

### „Nuotrauka nematoma"
✅ Patikrink failo pavadinimą – turi būti TIKSLIAI toks pat (pvz. `hero-default.jpg`)
✅ Patikrink ar failas yra `assets/images/` kataloge
✅ Spausk Ctrl+F5 (hard refresh naršyklėje)

### „Mygtukas neveikia"
✅ Atidaryk F12 → Console → ar yra raudonų klaidų?
✅ Patikrink ar `index.html` visiškai išsaugotas

### „Puslapis lėtai kraunasi"
✅ Optimizuok nuotraukas: https://tinypng.com
✅ GIF sumažink: https://ezgif.com/optimize

---

## 🎉 SĖKMĖS!

Klausimai? Patikrink F12 → Console ir ieškoki klaidų.

**© 2024 Medžio Meistrai**
