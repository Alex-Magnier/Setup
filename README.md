# Mon Setup - Documentation

Site portfolio showcasing mon setup informatique avec composants et périphériques.

## 🎨 Fonctionnalités

- 📱 **Responsive design** - Optimisé pour desktop, tablet et mobile
- 🎯 **3 pages** - Accueil, Composants, Périphériques
- 📊 **Intégration Google Sheets** - Possibilité d'ajouter des tableaux
- 🎭 **Design moderne** - Thème noir/rouge avec animations

## 📂 Structure du projet

```
.
├── index.html          # Page d'accueil
├── compo.html          # Liste des composants PC
├── periph.html         # Liste des périphériques
├── README.md           # Cette documentation
├── styles.css          # Feuille de styles CSS
└── assets/
    └── setup.jpg       # Image du setup
```

## 🚀 Comment utiliser

### Ajouter un tableau Google Sheet

Insérez ce code HTML où vous voulez le tableau :

```html
<div class="google-sheet-container">
    <iframe src="https://docs.google.com/spreadsheets/d/VOTRE_ID_SHEET/edit?usp=sharing" class="google-sheet"></iframe>
</div>
```

Remplacez `VOTRE_ID_SHEET` par l'ID de votre Google Sheet (visible dans l'URL après `/d/`)

## 📖 Explication CSS détaillée

### Réinitialisation globale (*) - Lignes 1-5

### Réinitialisation globale (*) - Lignes 1-5
- `margin: 0;` → Enlève l'espace extérieur par défaut de tous les éléments
- `padding: 0;` → Enlève l'espace intérieur par défaut de tous les éléments  
- `box-sizing: border-box;` → Inclut la bordure dans la largeur/hauteur totale (facilite le calcul des dimensions)

### Body - Lignes 7-11
- `font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;` → Choisit une belle police avec des alternatives de secours
- `background-color: #0f0f0f;` → Fond très sombre (presque noir) pour un style moderne
- `padding: 20px;` → Espace autour du contenu pour éviter que tout soit collé aux bords

### Setup Image (.setup-image) - Lignes 13-20
- `display: block;` → Affiche l'image comme un bloc pour pouvoir la centrer
- `margin: 0 auto 30px;` → Centre l'image (0 gauche/droite auto) et ajoute 30px d'espace en bas
- `max-width: 50%;` → L'image ne peut pas dépasser 50% de la largeur de son conteneur
- `height: auto;` → Maintient les proportions de l'image automatiquement
- `border: #0f0f0f 3px solid;` → Bordure noire de 3px autour de l'image
- `border-radius: 15px;` → Arrondit légèrement les coins de l'image
- `box-shadow: 0 4px 15px rgba(255, 68, 68, 0.3);` → Ombre rouge subtile (décalée de 4px en bas) pour faire ressortir l'image

### Titre Principal (.setup-titre) - Lignes 22-38
- `display: flex;` → Utilise flexbox pour avoir un système de centrage perfectionné
- `align-items: center;` → Centre verticalement le contenu
- `justify-content: center;` → Centre horizontalement le contenu
- `background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);` → Dégradé gris vers plus foncé en diagonale
- `color: white;` → Texte blanc
- `height: 150px;` → Hauteur de la boîte du titre
- `padding: 10px;` → Espace intérieur de 10px
- `border: 3px solid #ff4444;` → Bordure rouge vif de 3px
- `border-radius: 30px;` → Coins très arrondis (30px)
- `margin: 0 auto 30px;` → Centre la boîte avec auto en gauche/droite et 30px d'espace en bas
- `max-width: 600px;` → Largeur maximale de 600px
- `font-size: 32px;` → Texte grand et lisible
- `box-shadow: 0 4px 15px rgba(255, 68, 68, 0.3);` → Ombre rouge subtile

### Conteneur des Composants (.composant-pc) - Lignes 40-49
- `color: #ff4444;` → Texte rouge vif
- `background-color: #1a1a1a;` → Fond sombre
- `border: 2px solid #ff4444;` → Bordure rouge de 2px
- `border-radius: 20px;` → Coins arrondis
- `padding: 25px 15px;` → Espace intérieur (25px en haut/bas, 15px à gauche/droite)
- `text-align: center;` → Centre le texte
- `max-width: 600px;` → Limite la largeur
- `margin: 0 auto;` → Centre la boîte sur la page

### Composant Individuel (.composant) - Lignes 51-55
- `margin-bottom: 25px;` → Espace de 25px entre chaque composant
- `padding-bottom: 20px;` → Espace intérieur en bas
- `border-bottom: 1px solid #333;` → Ligne grise (1px) sous chaque composant pour les séparer

### Dernier Composant (.composant:last-child) - Lignes 57-60
- `border-bottom: none;` → Enlève la ligne sous le dernier composant
- `margin-bottom: 0;` → Enlève l'espace en bas du dernier composant

### Titre des Composants (.composant h2) - Lignes 62-66
- `font-size: 20px;` → Taille du texte
- `margin-bottom: 8px;` → Espace en bas du titre
- `color: #ff4444;` → Texte rouge pour les titres

### Paragraphes (.composant p) - Lignes 68-71
- `color: #ccc;` → Texte gris clair (couleur claire sur fond sombre)
- `font-size: 15px;` → Taille du texte plus petite que les titres

### Listes (ul) - Lignes 73-78
- `list-style-position: inside;` → Place les puces À L'INTÉRIEUR du texte (collé au texte)
- `padding-left: 0;` → Enlève l'espace à gauche par défaut
- `margin-top: 10px;` → Espace en haut de la liste
- `text-align: left;` → Aligne le texte à gauche dans les listes

### Éléments de liste (li) - Lignes 80-85
- `text-align: center;` → Centre le texte des éléments de liste
- `line-height: 1.8;` → Espace entre les lignes (plus lisible)
- `color: #ccc;` → Texte gris clair
- `padding-left: 5px;` → Petit espace à gauche

### Conteneur des boutons (.button-container) - Lignes 87-93
- `display: flex;` → Utilise flexbox pour aligner les boutons
- `gap: 20px;` → Espace entre les boutons
- `justify-content: center;` → Centre les boutons horizontalement
- `margin: 20px auto 30px;` → Espace autour du conteneur
- `max-width: 600px;` → Limite la largeur

### Boutons (.btn) - Lignes 95-108
- `padding: 12px 25px;` → Espace intérieur du bouton
- `border: 2px solid #ff4444;` → Bordure rouge
- `background-color: transparent;` → Fond transparent par défaut
- `color: #ff4444;` → Texte rouge
- `border-radius: 10px;` → Coins arrondis
- `text-decoration: none;` → Enlève le soulignement des liens
- `font-weight: bold;` → Texte en gras
- `cursor: pointer;` → Curseur de main au survol
- `transition: all 0.3s ease;` → Animation lisse lors du survol

### Boutons au survol (.btn:hover) - Lignes 110-113
- `background-color: #ff4444;` → Fond rouge au survol
- `color: #1a1a1a;` → Texte noir au survol (effet inverse)

### Conteneur Google Sheet (.google-sheet-container) - Lignes 115-122
- `max-width: 95%;` → Prend presque la largeur entière de la page
- `margin: 30px auto;` → Centre et ajoute de l'espace
- `border: 2px solid #ff4444;` → Bordure rouge cohérente avec le design
- `border-radius: 20px;` → Coins arrondis
- `overflow: hidden;` → Cache tout ce qui dépasse
- `box-shadow: 0 4px 15px rgba(255, 68, 68, 0.3);` → Ombre rouge subtile

### Iframe Google Sheet (.google-sheet) - Lignes 124-128
- `width: 100%;` → Prend 100% de la largeur de son conteneur
- `height: 600px;` → Hauteur de 600px sur desktop
- `border: none;` → Pas de bordure (on utilise le conteneur)
- `border-radius: 18px;` → Coins arrondis

### Responsive Tablet (@media max-width: 768px) - Lignes 130-172
**Adaptations pour tablettes et petits écrans :**
- `body { padding: 10px; }` → Réduit le padding à 10px
- `.setup-titre { height: 100px; font-size: 24px; }` → Titre plus compact
- `.setup-image { max-width: 100%; }` → Image prend toute la largeur
- `.button-container { flex-direction: column; max-width: 100%; }` → Boutons en colonne, fullwidth
- `.btn { width: 100%; padding: 15px; }` → Boutons au-dessus les uns des autres
- `.composant-pc { max-width: 100%; }` → Container fullwidth
- `.google-sheet { height: 500px; }` → Hauteur réduite pour le sheet
- Texte et espacements réduits pour lisibilité

### Responsive Mobile (@media max-width: 480px) - Lignes 174-195
**Adaptations pour téléphones :**
- `body { padding: 8px; }` → Padding minimal
- `.setup-titre { height: 80px; font-size: 20px; }` → Titre encore plus compact
- `.google-sheet { height: 400px; }` → Hauteur encore réduite
- `.composant-pc { padding: 15px 8px; }` → Padding réduit
- Tous les textes sont plus petits mais restent lisibles
- `margin-top: 10px;` → Espace au-dessus de la liste
- `text-align: left;` → Aligne la liste à gauche

### Éléments de Liste (li) - Lignes 80-85
- `text-align: center;` → Centre le texte des éléments
- `line-height: 1.8;` → Espace entre les lignes pour plus de lisibilité
- `color: #ccc;` → Texte gris clair
- `padding-left: 5px;` → Petit espace (5px) après la puce

### Conteneur des Boutons (.button-container) - Lignes 87-93
- `display: flex;` → Utilise flexbox pour aligner les boutons
- `gap: 20px;` → Espace de 20px entre les deux boutons
- `justify-content: center;` → Centre les boutons horizontalement
- `margin: 20px auto 30px;` → Espace au-dessus (20px), centre la boîte (auto) et 30px en bas
- `max-width: 600px;` → Largeur maximale pour rester alignée avec les autres éléments

### Boutons (.btn) - Lignes 95-105
- `padding: 12px 25px;` → Espace intérieur (12px haut/bas, 25px gauche/droite)
- `border: 2px solid #ff4444;` → Bordure rouge de 2px
- `background-color: transparent;` → Fond transparent par défaut
- `color: #ff4444;` → Texte rouge
- `border-radius: 10px;` → Coins arrondis du bouton
- `text-decoration: none;` → Enlève le soulignement des liens
- `font-weight: bold;` → Texte en gras pour plus de visibilité
- `cursor: pointer;` → Change le curseur en pointeur au survol
- `transition: all 0.3s ease;` → Transition lisse de 0.3 secondes pour tous les changements
- `font-size: 15px;` → Taille du texte du bouton

### Boutons au Survol (.btn:hover) - Lignes 107-109
- `background-color: #ff4444;` → Fond devient rouge au survol
- `color: #1a1a1a;` → Texte devient sombre au survol (inverse des couleurs)

## Résumé des couleurs utilisées
- **Fond principal** : #0f0f0f (noir très sombre)
- **Fond secondaire** : #1a1a1a (noir moins sombre)
- **Texte principal** : #ff4444 (rouge vif)
- **Texte secondaire** : #ccc (gris clair)
- **Bordure grise** : #333 (gris foncé)

