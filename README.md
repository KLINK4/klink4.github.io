# KLINK4 — Landing Page

Site vitrine statique de **KLINK4**, DevSecOps Factory spécialisée en identité numérique, Wallet, BLE, RFID et cryptographie.

## Stack

- HTML5
- CSS3 (custom properties, flexbox, grid, animations)
- Vanilla JS (scroll effect de la navbar uniquement)
- Police [Syne](https://fonts.google.com/specimen/Syne) + [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts

Aucune dépendance, aucun build nécessaire.

## Structure

```
klink4-landing-html/
├── index.html      # Page principale
├── style.css       # Feuille de styles
└── public/
    ├── favicon.svg
    └── icons.svg
```

## Lancer en local

### Option 1 — Ouvrir directement

Double-cliquez sur `index.html` pour l'ouvrir dans le navigateur.

> Note : certaines fonctionnalités (ex. polices Google Fonts) nécessitent une connexion internet.

### Option 2 — Serveur local (recommandé)

Avec **Python** (inclus sur macOS/Linux) :

```bash
python3 -m http.server 8080
```

Puis ouvrir [http://localhost:8080](http://localhost:8080).

Avec **Node.js** (`npx` suffit, pas d'installation) :

```bash
npx serve .
```

Avec l'extension VS Code **Live Server** :

Clic droit sur `index.html` → _Open with Live Server_

## Déploiement

Le site étant 100 % statique, il peut être hébergé sur n'importe quelle plateforme :

| Plateforme       | Commande / méthode                          |
| ---------------- | ------------------------------------------- |
| **Netlify**      | Drag & drop du dossier sur netlify.com/drop |
| **GitHub Pages** | Activer Pages sur la branche `main`         |
| **Vercel**       | `vercel --prod`                             |
| **Tout serveur** | Copier les fichiers dans le dossier web     |

Aucune variable d'environnement ni étape de build n'est requise.
