# 📱 Agenda MIFASS — Guide d'installation iPhone

Ce guide vous explique comment mettre l'agenda sur l'écran d'accueil de votre iPhone, comme une vraie application.

---

## 🎯 Vue d'ensemble (3 étapes)

1. **Héberger** les fichiers en ligne (gratuit, 5 minutes — GitHub Pages)
2. **Ouvrir** le lien dans Safari sur votre iPhone
3. **Ajouter** à l'écran d'accueil

---

## 📂 ÉTAPE 1 — Héberger l'app sur GitHub Pages (gratuit)

### A. Créer un compte GitHub
1. Allez sur https://github.com et cliquez sur **Sign up**
2. Renseignez votre email et créez un mot de passe
3. Vérifiez votre email

### B. Créer un nouveau dépôt (repository)
1. En haut à droite, cliquez sur **+** → **New repository**
2. Nommez le dépôt : `agenda-mifass` (ou tout autre nom)
3. Cochez **Public** (obligatoire pour la version gratuite)
4. Cochez **Add a README file**
5. Cliquez sur **Create repository**

### C. Téléverser les fichiers
1. Sur la page du dépôt, cliquez sur **Add file** → **Upload files**
2. Faites glisser TOUS les fichiers du dossier `agenda-mifass-pwa` :
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-152.png`
   - `icon-167.png`
   - `icon-180.png`
   - `icon-192.png`
   - `icon-512.png`
3. En bas, cliquez sur **Commit changes**

### D. Activer GitHub Pages
1. Dans le dépôt, allez dans l'onglet **Settings** (en haut à droite)
2. Dans le menu de gauche, cliquez sur **Pages**
3. Sous "Source", choisissez **Deploy from a branch**
4. Sous "Branch", sélectionnez **main** et **/ (root)**, puis cliquez sur **Save**
5. Attendez 1 à 2 minutes
6. Rechargez la page : un message en haut affiche votre URL, par exemple :
   `https://votreusername.github.io/agenda-mifass/`

✅ **Votre app est maintenant en ligne !**

---

## 📲 ÉTAPE 2 — Installer sur l'écran d'accueil iPhone

> ⚠️ **IMPORTANT : il faut obligatoirement utiliser Safari** (pas Chrome ni un autre navigateur).

1. Ouvrez **Safari** sur votre iPhone
2. Tapez l'URL de votre app (ex. `https://votreusername.github.io/agenda-mifass/`)
3. Une fois la page chargée, touchez le bouton **Partager** en bas (l'icône carrée avec une flèche vers le haut ⬆︎)
4. Faites défiler vers le bas et touchez **« Sur l'écran d'accueil »**
5. Modifiez le nom si vous voulez (par défaut : « Agenda MIFASS ») puis touchez **Ajouter**

🎉 **L'icône MIFASS apparaît maintenant sur votre écran d'accueil !**

Quand vous touchez l'icône, l'app s'ouvre **en plein écran sans la barre Safari**, exactement comme une vraie application.

---

## 💾 À propos des données

- Vos événements sont **enregistrés localement sur votre iPhone** (technologie localStorage)
- Ils restent disponibles même hors-ligne ✈️
- ⚠️ Si vous supprimez l'app de l'écran d'accueil **OU** videz les données Safari, les événements seront perdus
- Pour sauvegarder, utilisez régulièrement le bouton **Word** ou **PDF** pour exporter votre agenda

---

## 🔄 Mettre à jour l'app plus tard

Si vous voulez améliorer l'app (ajouter des fonctionnalités, corriger un bug) :
1. Téléversez les nouveaux fichiers sur GitHub (Add file → Upload files)
2. La nouvelle version est en ligne dans la minute
3. Sur votre iPhone, fermez complètement l'app (double-clic Home / glisser vers le haut) et rouvrez-la

---

## 🆘 Problèmes courants

**L'icône n'apparaît pas correctement → fond blanc**
→ Vérifiez que les fichiers `icon-180.png` et `icon-192.png` sont bien téléversés.

**« Sur l'écran d'accueil » n'apparaît pas dans le menu Partager**
→ Vous n'êtes pas dans Safari. Ouvrez l'URL dans Safari obligatoirement.

**L'app ne se charge pas hors-ligne**
→ Ouvrez l'app au moins une fois en ligne. Le service worker met les fichiers en cache à la première visite.

**Mes données ont disparu**
→ Vérifiez que vous n'avez pas désactivé localStorage dans les Réglages Safari. Allez dans Réglages → Safari → Avancé → Données de sites web pour vérifier.

---

## 🔐 Sécurité et confidentialité

- **Les données restent sur votre iPhone** — rien n'est envoyé sur internet
- **GitHub Pages héberge uniquement le code** de l'app, pas vos événements
- Le dépôt étant public, **n'incluez jamais de données sensibles dans les fichiers source**
- Pour un usage très confidentiel, demandez plutôt un hébergement privé (Netlify ou Vercel offrent des dépôts privés gratuits)

---

## 📞 Si besoin d'aide

Cette app est 100% personnalisable. Vous pouvez demander :
- Des fonctionnalités supplémentaires (rappels, notes vocales, partage…)
- Un design différent
- Une version multi-utilisateurs (avec base de données)
- Une vraie app App Store (paiement Apple Developer requis)
