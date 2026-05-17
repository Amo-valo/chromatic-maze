# Chromatic Maze — PWA

Jeu de labyrinthe installable sur iOS et Android comme une vraie app.

## Fichiers
- `index.html` — le jeu complet
- `manifest.json` — rend l'app installable
- `sw.js` — cache le jeu pour jouer hors-ligne
- `icon-192.png` / `icon-512.png` — icônes (à créer, voir ci-dessous)

---

## Créer les icônes (obligatoire)

Tu as besoin de deux images PNG avec fond sombre et un labyrinthe/logo :
- `icon-192.png` → 192×192 px
- `icon-512.png` → 512×512 px

Option rapide : utilise https://favicon.io ou Canva pour créer une icône,
puis exporte en 192px et 512px dans le dossier du projet.

---

## Mettre en ligne gratuitement avec GitHub Pages

### Étape 1 — Créer un compte GitHub
→ https://github.com (gratuit)

### Étape 2 — Créer un nouveau dépôt
- Clique sur "New repository"
- Nom : `chromatic-maze`
- Coche "Public"
- Clique "Create repository"

### Étape 3 — Uploader les fichiers
- Clique "uploading an existing file"
- Glisse tous tes fichiers (index.html, manifest.json, sw.js, icons)
- Clique "Commit changes"

### Étape 4 — Activer GitHub Pages
- Va dans Settings → Pages
- Source : "Deploy from a branch"
- Branch : `main` / `root`
- Clique Save

### Étape 5 — Accéder à ton app
Ton jeu sera disponible à :
https://TON_PSEUDO.github.io/chromatic-maze/

---

## Installer sur iPhone (iOS)
1. Ouvre l'URL dans Safari
2. Appuie sur l'icône Partager (carré avec flèche)
3. "Sur l'écran d'accueil"
4. L'app apparaît comme une vraie app !

## Installer sur Android
1. Ouvre l'URL dans Chrome
2. Chrome affiche automatiquement "Ajouter à l'écran d'accueil"
3. Ou : menu ⋮ → "Installer l'application"

---

## Jouer en local (pour tester)
Tu ne peux pas ouvrir index.html directement (les Service Workers
nécessitent un serveur). Installe Node.js puis :

```bash
npx serve .
```
Puis ouvre http://localhost:3000
