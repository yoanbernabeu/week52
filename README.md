# 📋 Gestionnaire de Résolutions - RESOLUTIONS.EXE

![Windows 3.11](https://img.shields.io/badge/Style-Windows%203.11-008080?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222222?style=flat-square&logo=github)

> 🏆 Projet réalisé pour le défi [DevChallenges Week-52 - Liste de Résolutions](https://devchallenges.yoandev.co/challenge/week-52/)

## 🎯 Le Défi

Créer une application de gestion de liste avec :
- ✅ Ajouter/Supprimer des items dans une liste
- ✅ Utiliser `localStorage` pour la persistance des données

## 🖥️ Aperçu

Une application nostalgique au style **Windows 3.11** pour gérer vos bonnes résolutions de la nouvelle année ! Retrouvez l'ambiance rétro des années 90 avec une interface fidèle aux fenêtres classiques de Microsoft.

## ✨ Fonctionnalités

### Gestion des Résolutions
- **Ajouter** une résolution avec titre, date butoir et description
- **Changer le statut** : En cours → Terminé → Abandonné
- **Persistance locale** : vos données sont sauvegardées automatiquement dans le `localStorage`

### Interface Windows 3.11
- 🪟 Fenêtre déplaçable (drag & drop)
- 📁 Menu "Fichier" avec raccourcis clavier
- 🎨 Palette de couleurs authentique (Teal, Gris, Bleu marine)
- 📜 Barre de défilement rétro
- 🔘 Boutons avec effet 3D biseauté

### Import/Export
- **Enregistrer sous...** : Exporter vos résolutions en fichier `.RES` (JSON)
- **Ouvrir...** : Importer un fichier de sauvegarde

### 🥚 Easter Egg
Cliquez sur **Aide > A propos...** pour une surprise nostalgique ! 💙

## 🚀 Installation

Aucune installation requise ! C'est une application **100% front-end**.

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/votre-username/week52.git
   ```

2. Ouvrez `index.html` dans votre navigateur préféré

## 📁 Structure du Projet

```
week52/
├── .github/
│   └── workflows/
│       └── deploy.yml   # CI/CD GitHub Actions
├── index.html           # Application complète (HTML + CSS + JS)
└── README.md            # Documentation
```

## 🚀 Déploiement (CI/CD)

L'application est automatiquement déployée sur **GitHub Pages** à chaque push sur la branche `main`.

### Configuration requise

1. Allez dans les **Settings** de votre dépôt GitHub
2. Dans **Pages** (menu de gauche)
3. Sous **Build and deployment** :
   - **Source** : sélectionnez `GitHub Actions`

### Workflow

Le fichier `.github/workflows/deploy.yml` configure le déploiement automatique :
- ✅ Se déclenche à chaque push sur `main`
- ✅ Peut être lancé manuellement depuis l'onglet **Actions**
- ✅ Déploie le contenu sur GitHub Pages

Votre application sera accessible à :
```
https://votre-username.github.io/week52/
```

## 🛠️ Technologies Utilisées

| Technologie | Utilisation |
|-------------|-------------|
| **HTML5** | Structure de l'application |
| **CSS3** | Style rétro Windows 3.11 |
| **JavaScript (Vanilla)** | Logique CRUD et localStorage |
| **Google Fonts** | Police VT323 (style terminal) |

## 💾 Stockage des Données

Les résolutions sont stockées dans le `localStorage` du navigateur sous la clé `win31_data` au format JSON :

```json
[
  {
    "id": 1704067200000,
    "title": "Apprendre Rust",
    "date": "31/12/2025",
    "desc": "Enfin comprendre le borrow checker",
    "status": "todo"
  }
]
```

### Statuts disponibles
| Statut | Description |
|--------|-------------|
| `todo` | En cours |
| `done` | Terminé |
| `abandoned` | Abandonné |

## 🎨 Palette de Couleurs

| Couleur | Hex | Utilisation |
|---------|-----|-------------|
| Teal | `#008080` | Fond d'écran |
| Gris | `#c0c0c0` | Fenêtre |
| Bleu Marine | `#000080` | Barre de titre |
| BSOD Blue | `#0000AA` | Easter egg 💀 |

## 📝 Licence

Ce projet est open source. Créé avec ❤️ et nostalgie.
