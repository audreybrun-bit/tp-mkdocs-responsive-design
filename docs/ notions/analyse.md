# Analyse réflexive (F2D57)

Cette analyse réflexive met en relation les choix techniques réalisés dans le mini-site (MkDocs Material, Bootstrap, media queries, organisation des contenus) avec les exigences du référentiel F2D57 : concevoir, structurer et diffuser des ressources pédagogiques numériques adaptées aux usages et aux contextes d'apprentissage.

La fiche F2D57 définit la mission de cet emploi-type ainsi :  
« étudier et assurer la maîtrise d'œuvre des projets numériques pour répondre aux besoins des acteurs et publics des établissements et favoriser l'évolution des pratiques pédagogiques ».

---

## 1. Objectif de l'analyse

Il s'agit de montrer en quoi les décisions techniques prises dans ce projet relèvent d'une véritable démarche d'ingénierie pédagogique, et contribuent à :

- améliorer l'expérience apprenant ;
- garantir l'accessibilité ;
- assurer la cohérence pédagogique ;
- soutenir la diffusion de contenus multimodaux.

---

## 2. Structuration des contenus

Le site repose sur une organisation claire :

- une page d'accueil contextualisée ;
- une section « Notions » regroupant les concepts clés ;
- une page d'analyse réflexive.

Cette structuration répond à l'activité F2D57 :  
« élaborer les cahiers des charges fonctionnels pour la réalisation de dispositifs et de ressources ».

---

## 3. Choix techniques et justification

### MkDocs Material
Documentation claire, hiérarchisée et responsive.

### Media queries
Adaptation du contenu aux différents supports.

### Bootstrap
Simplifie la mise en page responsive et propose des composants standardisés.

### CSS personnalisé
Corrige les débordements sur mobile.

---

## 4. Exemple de grille Bootstrap (affiché comme code)

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6">
      Bloc A
    </div>
    <div class="col-12 col-md-6">
      Bloc B
    </div>
  </div>
</div>
```

---

## 5. Breakpoints Bootstrap (affiché comme code)

```html
col-12  → sur mobile, chaque bloc prend toute la largeur  
col-md-6 → à partir de md, deux colonnes
```

---

## 6. Exemple d’alerte Bootstrap (affiché comme code)

```html
<div class="alert alert-info" role="alert">
  Rappel : testez toujours sur plusieurs tailles d'écran.
</div>
```

---

## 7. Conclusion

Le projet répond aux attentes du référentiel F2D57 en proposant un mini-site clair, responsive, structuré et cohérent.  
Les choix techniques sont justifiés, ancrés dans les missions officielles de l'emploi-type, et illustrent une démarche d'ingénierie pédagogique à part entière.

