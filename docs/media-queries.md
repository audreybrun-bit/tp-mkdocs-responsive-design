# Média queries

## Pourquoi utiliser des media queries ?

Les media queries permettent d'appliquer des styles CSS selon les caractéristiques du contexte de lecture **(largeur de l'écran, orientation, résolution, préférences utilisateur, etc.)**. Elles constituent le mécanisme de base pour réaliser une mise en page responsive.

**Objectif** : éviter qu'une mise en page « casse » quand l'utilisateur change de support (mobile, tablette, ordinateur) ou modifie la taille de texte. En contexte d'ingénierie pédagogique, cela sert directement la lisibilité des consignes, la stabilité de la navigation et l'accessibilité, notamment pour des apprenants utilisant des zooms ou des tailles de police augmentées.

![image mediaqueries](img/dediaqueries.png)
*Image générée par IA*

## Syntaxe essentielle

```css
@media (min-width: 768px) {
  /* styles pour écrans >= 768px */
}
```

Une media query associe une **condition** (ici, une largeur minimale d'écran) à un **bloc de styles**, appliqué uniquement si la condition est vraie.

## Exemples concrets

### 1. Passage d'une colonne à deux colonnes

```css
.card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1rem;
}

@media (min-width: 768px) {
  .card-grid {
    grid-template-columns: 1fr 1fr;
  }
}
```

### 2. Ajuster la typographie

```css
h1 { font-size: 1.6rem; }

@media (min-width: 992px) {
  h1 { font-size: 2.3rem; }
}
```

## Breakpoints et logique responsive

Une media query s'appuie sur des conditions. Dans un scénario responsive classique, on raisonne par paliers :

- **Mobile-first** : on définit un style de base pour les petits écrans, puis on ajoute des améliorations via des conditions comme `min-width`.
- **Progressive enhancement** : si la condition n'est pas remplie (écran trop petit, orientation différente), l'interface reste utilisable et le contenu demeure accessible.

Ce raisonnement aide aussi à diagnostiquer des dysfonctionnements fréquents : chevauchements, débordements, typographies trop petites ou éléments interactifs difficiles à cliquer.

## Points d'attention (accessibilité et robustesse)

- Tester le rendu avec un zoom navigateur (ex. 125 % / 200 %).
- Vérifier la lisibilité : contrastes, taille minimale, hauteur de ligne (`line-height`).
- Éviter les largeurs fixes pour le texte.
- Préférer des layouts flexibles (`grid`/`flex`) associés à des media queries ciblées.

## Cas d'usage en ingénierie pédagogique

- **Supports de cours** : réorganiser en une seule colonne, sur mobile, les blocs « définition / exemple / exercice ».
- **Consignes** : augmenter la lisibilité en réduisant la densité (espacements, taille des titres) selon le viewport.
- **Parcours interactifs** : afficher des éléments secondaires (aides, liens, résumés) seulement à partir de certains seuils d'écran.

## Mini check-list responsive

- Le contenu reste lisible en portrait **et** en paysage.
- Les blocs ne se chevauchent pas.
- Les éléments interactifs restent cliquables.
- La navigation reste compréhensible.

