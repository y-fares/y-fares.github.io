# GitHub Portfolio Setup — y-fares.github.io

**Guide d'installation et déploiement du portfolio GitHub Pages.**

---

## 📋 Pré-requis

- Compte GitHub
- Git installé localement
- Ruby 2.7+ (pour Jekyll local)
- Bundler (pour dépendances Ruby)

---

## 🚀 Installation

### Step 1 : Créer le repo GitHub (5 min)

```bash
# Sur GitHub.com
1. New repository
2. Name: "y-fares.github.io" (EXACT)
3. Make it Public
4. Initialize with README
5. Clone locally
```

### Step 2 : Copier les fichiers (5 min)

```bash
cd y-fares.github.io

# Copier depuis ORIGIN/github-portfolio :
# - _config.yml
# - README.md
# - *.md (skills, about, contact, projects/)
# - assets/ (css, images)
# - Gemfile
# - .gitignore
```

### Step 3 : Installer dépendances (5 min)

```bash
bundle install
```

### Step 4 : Test local (10 min)

```bash
bundle exec jekyll serve

# Ouvrir browser: http://localhost:4000
# Tester: navigation, links, responsive (F12 > mobile view)
```

### Step 5 : Ajouter images (10 min)

Créer `assets/images/` et ajouter :

- `avatar.png` (100×100, professional photo)
- `banner.png` (1200×400, hero image optionnel)
- Product screenshots (1200×600 each):
  - `trending-engine.png`
  - `meeting-brain.png`
  - `interview-prep.png`

**Où trouver screenshots :**
- Si tu as les produits : screenshot directement
- Si pas de produit : créer simple diagram en Figma/Draw

### Step 6 : Commit et push (5 min)

```bash
git add .
git commit -m "initial portfolio commit"
git push origin main

# Attendre 2-3 minutes pour GitHub Pages build
```

### Step 7 : Vérifier déploiement (2 min)

```bash
# Ouvrir dans browser
https://y-fares.github.io

# Tester sur mobile (iPhone + Android emulator)
```

---

## ✅ Quality Checklist

Avant de considérer le portfolio prêt :

- [ ] Tous les liens marchent (0 404s)
- [ ] Pas de typos (Ctrl+F chaque page)
- [ ] Mobile responsive (test sur vrai phone)
- [ ] Dark mode (dev tools > dark mode simulation)
- [ ] Images chargent rapidement
- [ ] Contact info visible partout (footer, contact page)
- [ ] Social links corrects (LinkedIn, GitHub)
- [ ] Favicon affichée (y-fares.github.io browser tab)

---

## 🎨 Customization

### Changer couleurs

Éditer `assets/css/style.css` :

```css
:root {
  --primary-color: #0066cc;  /* Change ici */
  --text-primary: #1a1a1a;
  /* etc */
}
```

### Ajouter pages

1. Créer `new-page.md` à la racine
2. Ajouter lien dans nav (`_config.yml` ou manuelle)
3. Écrire contenu en Markdown

### Éditer _config.yml

```yaml
title: "Your Name"
description: "Your tagline"
author: "Your Name"
url: "https://y-fares.github.io"
```

---

## 📈 Analytics (Optionnel mais recommandé)

### Ajouter Google Analytics

1. Créer compte Google Analytics
2. Récupérer Measurement ID (format: G-XXXXXXXXXX)
3. Ajouter script à `_config.yml` ou footer

---

## 🐛 Troubleshooting

**Portfolio doesn't show up :**
- Attendre 3-5 min (GitHub Pages build peut être lent)
- Vérifier `Settings → Pages → Source` = main branch
- Check `gh-pages` branch (GitHub Pages peut créer une branche)

**Styles pas appliquées :**
- Hard refresh browser (Ctrl+Shift+R)
- Check `assets/css/style.css` existe
- Check `_config.yml` theme ligne

**Images not loading :**
- Check chemin (doit être `assets/images/filename.png`)
- Vérifier fichier existe en local
- Comparer avec README.md image reference

**Local server won't start :**
```bash
bundle install  # Réinstaller gems
bundle exec jekyll clean  # Nettoyer cache
bundle exec jekyll serve  # Relancer
```

---

## 🚀 Post-Launch

**Jour 1 :**
- [ ] Visiter https://y-fares.github.io
- [ ] Test tous les liens
- [ ] Screenshot pour trace

**Semaine 1 :**
- [ ] Ajouter lien dans LinkedIn bio
- [ ] Envoyer lien à 5 amis pour feedback
- [ ] Fixer bugs identifiés

**Semaine 2+ :**
- [ ] Share dans LinkedIn posts
- [ ] Envoyer link à recruteurs
- [ ] Monitor Google Analytics (si activé)
- [ ] Itérer basé sur feedback

---

## 📞 Support

Des questions?
- Jekyll docs : https://jekyllrb.com/
- GitHub Pages : https://pages.github.com/
- Markdown guide : https://www.markdownguide.org/

---

**Ready?** 🚀 Commence par Step 1!
