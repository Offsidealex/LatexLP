# LaTeX Studio

> Éditeur LaTeX en ligne, façon Overleaf, 100 % dans le navigateur — pensé pour préparer cours, TP, évaluations et CCF au lycée.

**👉 Application en ligne : [offsidealex.github.io/LatexLP](https://offsidealex.github.io/LatexLP/)**

---

## ✨ Fonctionnalités

- 📝 **Éditeur LaTeX** avec coloration syntaxique (CodeMirror)
- 👀 **Aperçu PDF en split-view** — éditeur à gauche, PDF à droite (comme Overleaf), avec séparateur déplaçable
- ⚡ **Compilation en ligne** via [texlive.net](https://texlive.net) (avec [latexonline.cc](https://latexonline.cc) en serveur de secours pour les documents simples)
- 📦 **Projets multi-fichiers** — import d'archives `.zip` Overleaf avec images, sous-dossiers, bibliographies, etc.
- 📁 **Arborescence avec sous-dossiers** illimités (BTS MATHS / CCF / Session 1 / …)
- ☁️ **Synchronisation GitHub** — push/pull automatique de tous vos documents dans un dépôt
- 💾 **Sauvegarde automatique** dans le navigateur (localStorage)
- 🎨 **Thèmes clair / foncé** + 10 palettes de coloration syntaxique
- 🖱️ **Glisser-déposer** de fichiers `.tex` ou `.zip` directement sur la fenêtre
- 📐 **Modèles intégrés** : TP, évaluation, corrigé, CCF, Beamer

---

## 🚀 Utilisation

Il suffit d'ouvrir l'application dans un navigateur — aucune installation. Tout fonctionne en local : les documents sont stockés dans le `localStorage` du navigateur, et la synchronisation GitHub (optionnelle) permet de retrouver son travail sur n'importe quel poste.

### Modèles préconfigurés

| Modèle | Usage |
|--------|-------|
| **Article vide** | Démarrage rapide |
| **Beamer** | Diaporama de cours |
| **TP / Activité** | Énoncé avec cadres réponses |
| **Évaluation** | Contrôle barémé |
| **Corrigé** | Document corrigé avec mise en forme |
| **CCF / BTS** | Épreuve d'examen multi-parties |

### Raccourcis

| Raccourci | Action |
|-----------|--------|
| `Ctrl + Entrée` | Compiler |
| `Ctrl + S` | Sauvegarder (renommer le document) |
| Double-clic sur le séparateur | Réinitialiser la largeur |

---

## ☁️ Synchroniser avec GitHub

1. Créer un [Fine-grained Personal Access Token](https://github.com/settings/personal-access-tokens/new) avec la permission **Contents: Read &amp; write** sur le dépôt cible
2. Dans l'app, cliquer sur **GitHub** dans la barre d'outils
3. Renseigner token + propriétaire + dépôt + branche + dossier
4. **Tester la connexion** puis **Tout pousser** ou **Tout récupérer**

Le token reste dans le navigateur — il n'est envoyé qu'à `api.github.com`.

---

## 🔧 Pile technique

- HTML / CSS / JavaScript pur, sans build
- [CodeMirror 5](https://codemirror.net/5/) pour l'éditeur
- [JSZip](https://stuk.github.io/jszip/) pour l'import d'archives Overleaf
- [texlive.net](https://texlive.net) (Norbert Preining) comme compilateur pdflatex distant
- API REST GitHub pour la synchronisation

---

## 📄 Licence

Projet personnel pédagogique — usage libre pour les collègues enseignants.

**Auteur :** Alexis RUIZ — Lycée Denis Diderot (Bavilliers)
