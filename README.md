# 🛡️ Óbuda University SOC Command Web Portal — GitHub Pages Deployment Package

Ez a mappa (**`soc-portal-gh-pages`**) tartalmazza az Óbudai Egyetem (Bánki Kar) Kiberbiztonsági SOC Web Portál **előre lefordított, azonnal üzembe helyezhető (deploy-ready) statikus weboldalát**.

---

## 🚀 Hogyan tudod 1 perc alatt közzétenni GitHub Pages-en?

### 1. Opció: GitHub Webes felületen (Feltöltés / Drag & Drop)
1. Hozz létre egy új GitHub repót (pl. `soc-portal` vagy `oe-soc`).
2. Töltsd fel a **`soc-portal-gh-pages` mappa teljes tartalmát** a repó gyökerébe:
   - `index.html`
   - `404.html`
   - `.nojekyll`
   - `assets/` mappa (a JS és CSS fájlokkal)
3. A GitHub repóban kattints: **Settings** (Beállítások) ➔ **Pages** (bal oldali menü).
4. A **Build and deployment** résznél:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (vagy `master`), mappa: `/ (root)`
   - Kattints a **Save** gombra!
5. 1-2 percen belül a GitHub Pages linken elérhetővé válik a weboldalad:  
   👉 `https://<felhasznaloneved>.github.io/<repo-neve>/`

---

### 2. Opció: Git Parancssorból (CLI)
Nyiss egy terminált / PowerShell-t ebben a mappában (`soc-portal-gh-pages`), majd futtasd:

```bash
git init
git add .
git commit -m "Deploy: OE-UNI Retro Cyberpunk SOC Command Center"
git branch -M main
git remote add origin https://github.com/<felhasznaloneved>/<repo-neve>.git
git push -u origin main --force
```

Ezután a repó **Settings ➔ Pages** menüjében kapcsold be a GitHub Pages-t (`main` branch, `/ (root)` mappa).

---

## ✨ Mit tartalmaz ez a csomag?

- **Önálló (Standalone) Interaktív Demó Mód**: Ha a Python háttérrendszer nincs elindítva a háttérben, a weboldal automatikusan a beépített szimulációs adatokkal és interaktív funkciókkal működik.
- **Teljes Fúziós Műveleti Központ**:
  - 🖥️ **War Room Dashboard**: Valós idejű MITRE ATT&CK radar, fenyegetettségi szint mutató, LED KPI-k, telemetria ticker.
  - ⚡ **Cyber Range Támadás Szimulátor**: SSH Brute-force, SQLi Exfiltration, Cowrie Honeypot, LockBit 3.0 Ransomware tesztfuttatások.
  - 🔍 **Incidens Munkaállomás**: Részletes riasztás-elemzés, IoC-k, AI triázs javaslatok, SOAR beavatkozási napló.
  - 🛡️ **NIS2 Hatósági Megfelelőség**: Automatikus 24h korai figyelmeztetés & 72h CSIRT incidens-bejelentő dosszié generálás (2024. évi LXIX. tv.).
  - 🇭🇺 **Kétnyelvűség**: Váltás Magyar 🇭🇺 és Angol 🇬🇧 nyelvek között a felső menüsorban.
  - 👥 **Stáblista & Manifesztum**: Egyetemi projektcsapat névsor és Neptun-kódok keresővel és színes szerepkör-címkékkel.
