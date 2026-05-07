# 📈 Trading Journal

Application desktop **moderne et hors ligne** pour suivre tes trades, analyser tes performances et progresser comme un pro.
Construite avec **Electron + React**, conçue pour Windows.

![GitHub release](https://img.shields.io/github/v/release/djubg/trading-journal?style=flat-square&color=5b8cff)
![Downloads](https://img.shields.io/github/downloads/djubg/trading-journal/total?style=flat-square&color=22c55e&label=Téléchargements)
![License](https://img.shields.io/github/license/djubg/trading-journal?style=flat-square)

---

## ⬇️ Téléchargement

👉 **[Télécharger la dernière version](https://github.com/djubg/trading-journal/releases/latest)**

Choisis le fichier `Trading Journal Setup X.X.X.exe`, lance-le, et c'est parti.
L'app se met à jour **automatiquement** quand une nouvelle version est publiée.

---

## ✨ Fonctionnalités

### 📒 Journal complet
- Ajouter / modifier / supprimer / **dupliquer** tes trades
- Tous les champs essentiels : date, heure, marché, timeframe, BUY/SELL, entrée, SL, TP, lot, valeur/point
- Tags personnalisés (ex: `breakout`, `FVG`, `news`...) avec auto-complétion
- Capture d'écran avant + après le trade
- Notes : pourquoi tu es entré, erreur commise, leçon apprise

### 🧮 Calculs automatiques
- **Risk Reward (RR)** auto
- **PnL automatique** depuis entrée/SL/TP/lot
- **Taille de position suggérée** selon ton capital et ton % de risque
- **Winrate, expectancy, drawdown max, séries** de gains/pertes

### 📊 Dashboard puissant
- Courbe d'équité (PnL cumulé)
- **Heatmap calendrier** (style GitHub) — vert = jour gagnant, rouge = jour perdant
- Stats par marché, par jour de semaine, par heure
- Distribution des RR (histogramme)
- Stats par tag (winrate + PnL par setup)
- Top 8 des erreurs récurrentes
- Filtre période : 7j / 30j / 90j / Tout

### 🎯 Plan de trading
- Onglet dédié au **plan en markdown** (règles, setups, checklist)
- **Objectifs** : max trades/jour, RR minimum, objectif PnL hebdo
- **Alertes rouges** automatiques si tu dépasses tes limites

### 🛡️ Robustesse
- Sauvegarde locale automatique
- **Backups quotidiens** (10 derniers jours conservés)
- Export **CSV** (Excel) et **JSON** (sauvegarde complète)
- Import JSON pour restaurer
- 100 % **hors ligne** — tes données ne quittent jamais ton PC

### ⚡ UX
- Style **moderne sombre**, simple comme un cahier
- Tableau type Google Sheets avec **tri par colonne**
- Filtres rapides : recherche, marché, tag, dates
- **Raccourcis clavier** : `N` nouveau trade · `1/2/3` onglets · `Ctrl+F` recherche · `Shift+F` plein écran · `Esc` annuler · `Ctrl+S` enregistrer
- Mode plein écran tableau

### 🔄 Mises à jour automatiques
Quand une nouvelle version est publiée, l'app affiche un **bandeau bleu** avec un bouton **"Mettre à jour"**. Téléchargement en arrière-plan, redémarrage en un clic, données conservées.

---

## 🖼️ Aperçu

> Ajoute des screenshots ici une fois l'app lancée
> (`assets/journal.png`, `assets/dashboard.png`, etc.)

---

## 🛠️ Pour les développeurs

### Prérequis
- Node.js 18+
- npm

### Lancer en développement
```bash
git clone https://github.com/djubg/trading-journal.git
cd trading-journal
npm install
npm run dev
```

### Build de l'exécutable Windows
```bash
npm run package
```
Le `.exe` est généré dans `release/`.

### Publier une nouvelle version
1. Bump la version dans `package.json` (ex: `1.0.0` → `1.0.1`)
2. Définis `GH_TOKEN` (Personal Access Token GitHub avec scope `repo`)
3. Lance :
```bash
npm run release
```
4. Va sur GitHub Releases et publie la draft

---

## 📂 Où sont stockées mes données ?

| Type | Chemin |
|------|--------|
| Trades & paramètres | `%APPDATA%\trading-journal\trades.json` |
| Screenshots | `%APPDATA%\trading-journal\screenshots\` |
| Backups quotidiens | `%APPDATA%\trading-journal\backups\` |

> Astuce : tu peux copier ce dossier sur une clé USB pour transférer ton journal sur un autre PC, ou utiliser **Export JSON** depuis l'app.

---

## 🧰 Stack technique

- [Electron](https://www.electronjs.org/) — runtime desktop
- [React 18](https://react.dev/) — UI
- [Vite](https://vitejs.dev/) — bundler
- [Recharts](https://recharts.org/) — graphiques
- [electron-builder](https://www.electron.build/) — packaging
- [electron-updater](https://www.electron.build/auto-update) — mises à jour auto

---

## 📜 Licence

Usage personnel libre. Pas de garantie.

---

⭐ **Si l'app t'aide à mieux trader, mets une étoile sur le repo !**
