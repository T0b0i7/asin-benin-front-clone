# 🇧🇯 ASIN Bénin — Clone Front-End

Reproduction fidèle de l'interface utilisateur du site officiel de l'**Agence des Systèmes d'Information et du Numérique (ASIN)** du Bénin — [asin.bj](https://asin.bj/).

Ce projet est un clone statique HTML/CSS/JS réalisé à partir des fichiers scrapés du site officiel, en respectant la charte graphique, la structure des pages, et les contenus originaux.

---

## 📸 Aperçu

| Page | Aperçu |
|------|--------|
| **Accueil** | Hero avec dégradé bleu + titre *"Transformer le quotidien des béninois par le numérique"* |
| **Présentation** | Page institutionnelle "Qui sommes-nous" |
| **Organigramme** | Organigramme visuel de l'agence |
| **Projets** | Liste des projets numériques |
| **Emplois** | Offres d'emploi et recrutements en cours |

---

## 🗺️ Plan du site — 15 pages

| Menu | Sous-menu | Fichier |
|------|-----------|---------|
| **ASIN** | Présentation | `qui-sommes-nous.html` |
| | Mission et Attributions | `mission-et-attributions.html` |
| | Mot du directeur général | `mot-directeur.html` |
| | Gouvernance et Organisation | `gouvernance.html` |
| | Organigramme | `organigramme.html` |
| **Projets** | — | `projets.html` |
| **Publications** | Actualités | `actualites.html` |
| | Documents | `documents.html` |
| | Vidéos | `videos.html` |
| **Opportunités** | Emplois | `emplois.html` |
| | Marchés publics | `appels-offres.html` |
| **Évènements** | — | `evenements.html` |
| **Contact** | — | `contact.html` |

Toutes les pages partagent le même header (navigation avec dropdowns au survol) et le même footer (liens utiles, newsletter, copyright, drapeau du Bénin).

---

## 🛠️ Stack technique

| Technologie | Usage |
|-------------|-------|
| **HTML5** sémantique | Structure de toutes les pages |
| **Bootstrap 5.3** | Grille responsive, navbar, composants UI |
| **CSS3** custom | Dégradés, animations, mise en page pixel-perfect |
| **JavaScript** vanilla | Menus dropdown hover, interactions |
| **Font Awesome 6** | Icônes sociales et UI |
| **Fonts** Aquawax + Montserrat | Typographie conforme au site original |

---

## 🎨 Charte graphique

| Élément | Couleur / Valeur |
|---------|------------------|
| Bleu institutionnel (textes, titres) | `#1E3A8A` |
| Bleu vif (bouton recherche) | `#1D4ED8` |
| Bleu foncé succès | `#1F4878` |
| Bleu-cyan clair (warning) | `#81B0B1` |
| Dégradé hero | `linear-gradient(279.18deg, #1F4878 18.73%, #81B0B1 105.17%)` |

---

## 📁 Architecture du projet

```
/
├── index.html                    # Page d'accueil
├── *.html                        # 14 pages internes (voir plan du site)
│
├── public/
│   └── assets/
│       ├── images/               # Images, logos, icônes (format web)
│       ├── fonts/                # Polices Aquawax + Montserrat (TTF)
│       └── ...
│
├── src/
│   └── assets/
│       ├── vendor/               # Bootstrap 5.3 minified
│       ├── css/                  # Styles originaux OS + custom
│       ├── js/                   # Scripts JS
│       └── fonts/                # Polices locales
│
├── data/                         # Pages scrapées (référence uniquement)
│   └── <timestamp>/
│       ├── index.html
│       ├── *.css, *.png, *.ttf, ...
│
├── package.json                  # Dépendances (Bootstrap)
├── README.md                     # Ce fichier
└── .gitignore
```

---

## 🚀 Installation et utilisation

### En local (serveur statique)

```bash
# Cloner le dépôt
git clone https://github.com/T0b0i7/asin-benin-front-clone.git

# Ouvrir dans le navigateur
cd asin-benin-front-clone
start index.html
```

### Via un serveur de développement (recommandé)

```bash
# Avec Python
python -m http.server 8000

# Avec Node.js (live-server)
npx live-server

# Avec PHP
php -S localhost:8000
```

Puis ouvrir [http://localhost:8000](http://localhost:8000).

---

## ✅ Fonctionnalités implémentées

- [x] Navigation fixe avec dropdowns au survol (hover)
- [x] Hero section avec dégradé et titre principal
- [x] Cartes des 3 pôles (Infrastructures, Sécurité, Système d'Information)
- [x] Section Actualités (DevLab, communiqués)
- [x] Footer complet : liens utiles (gouv.bj, numérique, ARCEP, finances, APDP)
- [x] Bloc newsletter avec formulaire d'abonnement
- [x] Pages institutionnelles (Présentation, Mission, Mot DG, Gouvernance, Organigramme)
- [x] Pages de contenu (Projets, Actualités, Documents, Vidéos)
- [x] Pages Opportunités (Emplois, Marchés publics)
- [x] Page Évènements et page Contact
- [x] Drapeau du Bénin en bas de page (vert-jaune-rouge)
- [x] Responsive design (tablette et mobile)
- [x] Polices Aquawax + Montserrat
- [x] Icônes sociales (Twitter, YouTube, Flickr)

---

## 📦 Dépendances

- [Bootstrap 5.3](https://getbootstrap.com/) — Framework CSS
- [Font Awesome 6](https://fontawesome.com/) — Bibliothèque d'icônes
- Polices : Aquawax (Light, Medium, Black) + Montserrat (Light, Regular, Medium, SemiBold, Bold, ExtraBold)

---

## 📄 Licence

Projet éducatif — reproduction de l'interface publique de l'ASIN Bénin à but d'apprentissage.  
Tous droits sur le design et les contenus appartiennent à l'**Agence des Systèmes d'Information et du Numérique (ASIN)** — [asin.bj](https://asin.bj/).
