# Écrire à l'Université

Projet pour accompagner l'écriture académique à l'université. Ce dépôt contient un environnement Quarto complet pour créer des pages web, des documents PDF et des présentations sur le thème de l'écriture universitaire.

## 📚 Contenu

Ce projet propose :

- **Pages web** : Guides interactifs sur l'écriture académique
- **Documents PDF** : Ressources téléchargeables et imprimables
- **Présentations** : Slides RevealJS pour formations et ateliers
- **Ressources** : Bibliographie et outils pour l'écriture

## 🚀 Installation

### Prérequis

- [Quarto CLI](https://quarto.org/docs/get-started/) (version 1.4+)
- Un éditeur de texte (VS Code, RStudio, etc.)

### Installation de Quarto

**Linux (Ubuntu/Debian) :**
```bash
wget https://github.com/quarto-dev/quarto-cli/releases/download/v1.4.554/quarto-1.4.554-linux-amd64.deb
sudo dpkg -i quarto-1.4.554-linux-amd64.deb
```

**macOS :**
```bash
brew install quarto
```

**Windows :**
Téléchargez l'installateur depuis [quarto.org](https://quarto.org/docs/get-started/)

## 💻 Utilisation

### Prévisualiser le site web

```bash
quarto preview
```

Ouvre un serveur local avec rechargement automatique.

### Générer le site web

```bash
quarto render
```

Le site est généré dans le dossier `_site/`.

### Générer un document PDF spécifique

```bash
quarto render ecriture-academique.qmd --to pdf
```

### Générer la présentation

```bash
quarto render presentation.qmd --to revealjs
```

## 📖 Structure du projet

```
EcrireALUniv/
├── _quarto.yml              # Configuration principale
├── index.qmd                # Page d'accueil
├── ecriture-academique.qmd  # Guide de l'écriture académique
├── methodologie.qmd         # Méthodologie et techniques
├── ressources.qmd           # Outils et ressources
├── bibliographie.qmd        # Références bibliographiques
├── presentation.qmd         # Présentation RevealJS
├── styles.css               # Styles personnalisés
└── _site/                   # Site généré (ignoré par git)
```

## 🎨 Formats disponibles

### HTML (Site Web)
- Navigation interactive
- Recherche intégrée
- Responsive design
- Thèmes clair/sombre

### PDF
- Format A4
- Table des matières
- Numérotation des sections
- Liens hypertextes

### RevealJS (Présentation)
- Slides interactives
- Transitions animées
- Tableau blanc intégré
- Mode présentateur

## 🛠️ Personnalisation

### Modifier le thème

Éditez `_quarto.yml` pour changer les thèmes :

```yaml
format:
  html:
    theme: cosmo  # Changez pour flatly, minty, etc.
```

### Ajouter du contenu

1. Créez un fichier `.qmd` (par exemple `nouveau-chapitre.qmd`)
2. Ajoutez-le dans `_quarto.yml` sous `website.sidebar.contents`
3. Exécutez `quarto render`

### Styles personnalisés

Modifiez `styles.css` pour personnaliser l'apparence.

## 📝 Contribuer

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créez une branche (`git checkout -b feature/amelioration`)
3. Committez vos changements (`git commit -m 'Ajout d'une nouvelle section'`)
4. Poussez vers la branche (`git push origin feature/amelioration`)
5. Ouvrez une Pull Request

## 📄 Licence

Ce projet est libre d'utilisation pour l'enseignement et la recherche.

## 🔗 Liens utiles

- [Documentation Quarto](https://quarto.org/docs/guide/)
- [Guide Markdown](https://quarto.org/docs/authoring/markdown-basics.html)
- [Galerie d'exemples Quarto](https://quarto.org/docs/gallery/)

## 📧 Contact

Pour toute question ou suggestion, ouvrez une issue sur GitHub.

---

*Créé avec [Quarto](https://quarto.org) - Un système de publication scientifique et technique open-source*
