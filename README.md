# Prisme Digital

**Studio web — sites vitrines, espaces membres et outils de gestion.**
Los Santos, San Andreas.

---

## À propos du projet

Ce dépôt contient l'intégralité du code source du site vitrine de Prisme Digital, entreprise de développement web opérant sur le serveur FlashbackFA. Il est public et le restera : l'accès complet au code, sans obfuscation, fait partie des engagements pris auprès de FlashbackFA.

Aucune adresse de mise en ligne n'est indiquée ici. Les pages sont déployées par l'administration de FlashbackFA sur le domaine `fbfa.fr`, seul domaine autorisé.

---

## Contenu du dépôt

```
Paulygone-FlashbackFA/
├── index.html    ← le site vitrine, complet et autonome
├── images/       ← les visuels d'origine, non nécessaires au déploiement
└── README.md
```

### index.html — le site vitrine

| Section | Rôle |
|---|---|
| Héro | Promesse principale et deux appels à l'action |
| Indicateurs | Plateformes en production, heures d'expérience, disponibilité |
| À propos | Trois engagements, l'histoire du studio, notre position |
| Direction | Les deux patrons, leurs rôles et leurs créneaux |
| Services | Six domaines d'intervention — tarif sur demande |
| Méthode | Les quatre étapes d'un projet, du brief au suivi |
| Nous trouver | Adresse, horaires, conditions d'accueil |
| Communauté | Le serveur Discord, point d'entrée de tous les échanges |
| Pied de page | Navigation, mentions légales, cadre du projet |

---

## Choix techniques

Le site est un **document HTML unique et autonome**, sans framework ni étape de compilation.

| Élément | Choix | Raison |
|---|---|---|
| Structure | HTML5 sémantique | Accessibilité et référencement |
| Style | CSS3 natif, variables CSS | Aucune dépendance, chargement instantané |
| Interactivité | JavaScript vanilla (ES5) | Compatible avec tous les navigateurs, aucun build |
| Typographie | Space Grotesk + Inter | Repli automatique sur les polices système |
| Animations | Canvas 2D + IntersectionObserver | Désactivées si `prefers-reduced-motion` |
| Images | Encodées en base64 dans le document | Un seul fichier à déployer, aucun lien à casser |

**Pourquoi un fichier unique ?** Le site est hébergé sur une infrastructure tierce, sans accès administrateur du développeur, et mis en ligne par l'administration. Un livrable sans dépendance, sans runtime et sans build garantit un déploiement par simple copie de fichier, et une maintenance possible par n'importe qui.

### Appels réseau

Le site ne charge que les polices de caractères, depuis `fonts.googleapis.com` et `fonts.gstatic.com`. En cas d'indisponibilité, les polices système prennent le relais sans dégrader la mise en page.

Aucun autre appel réseau n'est effectué.

### Points d'attention

- Aucune donnée personnelle n'est collectée ni stockée
- Aucun cookie, aucun traceur
- Navigation clavier complète et attributs ARIA sur les composants interactifs
- Interface responsive testée de 320 px à 2560 px de large

---

## Déploiement

Aucune installation, aucune compilation.

**`index.html` se suffit à lui-même** : le fichier contient le code, les styles, les scripts et les images. Le déposer à la racine du serveur suffit.

Le dossier `images/` contient les visuels d'origine à leur taille réelle. Il n'est **pas nécessaire au déploiement**, les images étant déjà intégrées dans `index.html`. Il est conservé pour permettre de modifier ou remplacer un visuel par la suite.

---

## Identité

| Élément | Valeur |
|---|---|
| Nom | Prisme Digital |
| Signature | Studio web |
| Direction | Javier Silva, patron · Javier Silva, co-patron |
| Couleur principale | `#F23BA0` (magenta) |
| Couleur secondaire | `#25D5EC` (cyan) |
| Fond | `#07080C` |

Le prisme décompose la lumière en spectre : c'est l'origine du dégradé magenta → cyan utilisé sur l'ensemble de l'identité.

---

## Licence et propriété

Ce projet est développé dans le cadre du serveur de jeu de rôle FlashbackFA. Les sites réalisés pour le serveur et son administration deviennent la propriété de FlashbackFA, code source inclus, conformément aux conditions convenues avec l'équipe de gestion.

Le code est fourni dans son intégralité, sans obfuscation. La mise en production relève exclusivement de l'administration de FlashbackFA.

---

*Projet fictif réalisé dans un cadre de jeu de rôle. Les entreprises, montants et lieux mentionnés n'ont aucune existence réelle.*
