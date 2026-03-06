<div align="center">

 <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=header&text=Travaux%20Pratiques%20%7C%20ENSET%20Mohammedia&fontSize=40&fontAlignY=30" alt="Bannière Projet" width="100%" />

  <h1>Mini Projet 1 - Portfolio Web (HTML & CSS)</h1>

  <p>
    <a href="http://essoktani.tech/">
      <img src="https://img.shields.io/badge/Portfolio-essoktani.tech-05122A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" />
    </a>
    <a href="https://www.linkedin.com/in/yazid-essoktani-337549251/">
      <img src="https://img.shields.io/badge/LinkedIn-Yazid_ESSOKTANI-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
    </a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
    <img src="https://img.shields.io/badge/Layout-Flexbox%20%26%20Grid-8b5cf6?style=for-the-badge" alt="Layout" />
  </p>

</div>

<br />


<div align="center">

| Contexte Académique | Informations Projet |
| :--- | :--- |
| **Établissement :** ENSET Mohammedia | **Réalisé par :** [Yazid ESSOKTANI](https://www.linkedin.com/in/yazid-essoktani-337549251/) |
| **Filière :** Master Systèmes Distribués et Intelligence Artificielle | **Encadré par :** Prof. Oumayma AGHERAI |
| **Département :** Mathématiques et Informatique | **Année Universitaire :** 2025/2026 |
| **Module :** Technologies Web et Web Sémantique | **Sujet :** Création d’un portfolio web en HTML5/CSS3 |

</div>

<br />

## Sommaire

1. [Présentation](#-présentation)
2. [Fonctionnalités implémentées](#️-fonctionnalités-implémentées)
3. [Structure des fichiers](#-structure-des-fichiers)
4. [Installation et Visualisation](#-installation-et-visualisation)
5. [Explication du code (niveau débutant)](#-explication-du-code-niveau-débutant)
  - [1) Le squelette HTML](#1-le-squelette-html)
  - [2) La navigation (menu)](#2-la-navigation-menu)
  - [3) Une section de contenu](#3-une-section-de-contenu)
  - [4) Variables CSS (couleurs globales et système de design)](#4-variables-css-couleurs-globales-et-système-de-design)
  - [5) Header fixe avec backdrop blur](#5-header-fixe-avec-backdrop-blur)
  - [6) Gradients et texte dégradé](#6-gradients-et-texte-dégradé)
  - [7) Flexbox pour aligner le menu](#7-flexbox-pour-aligner-le-menu)
  - [8) Grid pour afficher les cartes en colonnes](#8-grid-pour-afficher-les-cartes-en-colonnes)
  - [9) Responsive design (mobile)](#9-responsive-design-mobile)
  - [10) Méthode simple pour progresser](#10-méthode-simple-pour-progresser)

---

## Présentation
Ce projet est un portfolio web personnel réalisé dans le cadre du **Mini Projet 1**. Il a été développé **exclusivement avec HTML5 et CSS3**, sans l'utilisation de bibliothèques externes ou de frameworks (comme Bootstrap ou Tailwind).

## Fonctionnalités implémentées
Conformément aux exigences du projet :
- **Structure Sémantique** : Utilisation de balises HTML5 appropriées (`<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`).
- **Mise en page (Layout)** : 
  - La navigation (`<nav>`) utilise **Flexbox** pour l'alignement horizontal avec positionnement fixe.
  - Les sections utilisent **CSS Grid** et **Flexbox** pour une disposition propre et réactive.
  - Header fixe avec effet de flou (backdrop-filter) pour un rendu moderne.
- **Système de Variables CSS** : Variables `:root` pour une gestion centralisée :
  - Couleurs Primaires : `--primary: #7c3aed` (Violet), `--secondary: #a855f7`, `--accent: #ec4899` (Rose)
  - Fond: `--bg-primary: #ffffff` (Blanc), `--bg-secondary: #f8f9fa` (Gris très clair)
  - Texte: `--text-primary: #1a1a1a` (Noir), `--text-secondary: #6b7280` (Gris)
  - Polices: `--font-sans: Inter`, `--font-mono: JetBrains Mono`
- **Effets Visuels Avancés** : 
  - Dégradés linéaires (gradient-text)
  - Animations fluides (transitions, keyframes)
  - Glows et shadows pour la profondeur
  - Badges, badges d'état et éléments interactifs
- **Responsive Design** : Adaptation automatique pour tous les tailles d'écran (mobile, tablette, desktop).

## Structure des fichiers
- `index.html` : Contient la structure sémantique et le contenu du portfolio.
- `style.css` : Contient l'ensemble des règles de style, la typographie, les grilles et les media queries.
- `README.md` : Ce présent rapport de projet.

## Installation et Visualisation
Aucune installation spécifique n'est requise. Il suffit de cloner ce dépôt et d'ouvrir le fichier `index.html` dans n'importe quel navigateur web moderne.

---

## Explication du code (niveau débutant)

Cette partie explique **comment lire et comprendre le code** si vous débutez en HTML/CSS.

### 1) Le squelette HTML

```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio | Yazid Essoktani</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <!-- contenu visible de la page -->
</body>
</html>
```

**Explication simple :**
- `<!DOCTYPE html>` : indique au navigateur qu'on utilise HTML5.
- `<html lang="fr">` : la page est en français.
- `<head>` : contient les informations techniques (pas le contenu principal visible).
- `<meta charset="UTF-8">` : permet d'afficher correctement les accents.
- `<meta name="viewport" ...>` : rend la page adaptée aux mobiles.
- `<link rel="stylesheet" ...>` : connecte le fichier CSS pour le style.

### 2) La navigation (menu)

```html
<nav class="navbar">
  <div class="logo">~/YE</div>
  <ul class="nav-links">
    <li><a href="#skills">Compétences</a></li>
    <li><a href="#projects">Projets</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

**Ce que ça fait :**
- `<nav>` : zone réservée au menu de navigation.
- `class="navbar"` : permet d'appliquer un style CSS spécifique.
- `<a href="#skills">` : lien interne qui descend vers la section ayant `id="skills"`.

### 3) Une section de contenu

```html
<section id="projects" class="projects-section">
  <div class="container">
    <h2 class="section-title">Projets Récents</h2>
    <article class="project-card">
      <h3>Store Smartly</h3>
      <p>Application SaaS complète de gestion de stock.</p>
    </article>
  </div>
</section>
```

**Ce que ça fait :**
- `<section>` : bloc logique de la page.
- `id="projects"` : identifiant unique pour y accéder via un lien.
- `<article>` : contenu autonome (ici, une carte de projet).

### 4) Variables CSS (couleurs globales et système de design)

```css
:root {
    --primary: #7c3aed;
    --secondary: #a855f7;
    --accent: #ec4899;
    
    --bg-primary: #ffffff;
    --bg-secondary: #f8f9fa;
    --text-primary: #1a1a1a;
    --text-secondary: #6b7280;
    --border-color: #e5e7eb;
    
    --font-sans: 'Inter', sans-serif;
    --font-mono: 'JetBrains Mono', monospace;
    
    --container-width: 1280px;
}

body {
    font-family: var(--font-sans);
    background-color: var(--bg-primary);
    color: var(--text-primary);
    line-height: 1.6;
}
```

**Pourquoi c'est utile :**
- `:root` contient des **variables CSS réutilisables** pour couleurs, polices et tailles.
- `var(--primary)` lit la valeur d'une variable, permettant une cohérence globale.
- Modifier une seule variable met à jour automatiquement toute la page.
- Système de design cohérent avec couleurs primaires, secondaires et accentuées.

### 5) Header fixe avec backdrop blur

```css
.header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    background: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border-color);
}
```

**Explication :**
- `position: fixed` : barre de navigation reste au sommet lors du défilement.
- `backdrop-filter: blur(12px)` : effet de flou moderne derrière l'en-tête.
- `z-index: 1000` : assure que le header reste au-dessus du contenu.

### 6) Gradients et texte dégradé

```css
.gradient-text {
    background: linear-gradient(135deg, var(--primary), var(--secondary), var(--accent));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
```

**Explication :**
- `linear-gradient()` : crée une dégradation de couleur.
- `background-clip: text` : fait que le dégradé s'applique au texte.
- Crée un effet visuel moderne et attrayant.

### 7) Flexbox pour aligner le menu

```css
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

**Explication :**
- `display: flex` : active Flexbox.
- `justify-content: space-between` : espace les éléments à gauche et à droite.
- `align-items: center` : aligne verticalement au centre.

### 8) Grid pour afficher les cartes en colonnes

```css
.projects-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}
```

**Explication :**
- `display: grid` : active CSS Grid.
- `repeat(3, 1fr)` : crée 3 colonnes de même largeur.
- `gap: 20px` : ajoute un espace entre les cartes.

### 9) Responsive design (mobile)

```css
@media screen and (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
}
```

**Explication :**
- `@media ...` : applique des styles seulement sur petits écrans.
- `1fr` : une seule colonne sur mobile, donc lecture plus confortable.

### 10) Méthode simple pour progresser

Si vous débutez, travaillez dans cet ordre :
1. Modifier un texte dans `index.html`.
2. Recharger la page dans le navigateur.
3. Changer une couleur dans `:root`.
4. Tester le responsive en réduisant la largeur de la fenêtre.

En répétant ce cycle, vous comprendrez rapidement le lien entre **structure HTML** et **style CSS**.