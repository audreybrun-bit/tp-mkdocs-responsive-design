# Analyse réflexive ([F2D57](https://data.enseignementsup-recherche.gouv.fr/pages/fiche_emploi_type_referens_iii_itrf/?refine.referens_id=F2D57#top))

Cette analyse réflexive met en relation les choix techniques réalisés dans le mini-site (MkDocs Material, Bootstrap, media queries, organisation des contenus) avec les exigences du référentiel F2D57 : concevoir, structurer et diffuser des ressources pédagogiques numériques adaptées aux usages et aux contextes d'apprentissage. Ce travail relève ainsi directement du champ de l'**ingénierie pédagogique**, au cœur de la formation dans laquelle s'inscrit ce projet.

La fiche F2D57 définit la mission de cet emploi-type ainsi : *« étudier et assurer la maîtrise d'œuvre des projets numériques pour répondre aux besoins des acteurs et publics des établissements et favoriser l'évolution des pratiques pédagogiques »*. C'est cette mission qui sert de fil conducteur à l'analyse qui suit.

![image conclusion](img/conclusion.png)
*Image générée par IA*

## 1. Objectif de l'analyse

Il s'agit de montrer en quoi les décisions techniques prises dans ce projet relèvent d'une véritable démarche d'**ingénierie pédagogique**, et contribuent à :

- **Améliorer l'expérience apprenant** : guider la lecture, réduire la charge cognitive et stabiliser la navigation.
- **Garantir l'accessibilité** : assurer une présentation lisible sur mobiles et tablettes, compatible avec différents usages (zoom, tailles de police).
- **Assurer la cohérence pédagogique** : structurer les contenus et soutenir une progression, du principe au fonctionnement, puis à l'appropriation.
- **Soutenir la diffusion de contenus multimodaux** : faciliter la réutilisation et la maintenance des supports (mise à jour facile, homogénéité visuelle).

## 2. Structuration des contenus

Le site repose sur une organisation claire :

- une page d'accueil contextualisée ;
- une section « Notions » regroupant les concepts clés (Bootstrap, media queries, MkDocs Material) 
- une page d'analyse réflexive.

Cette structuration répond à l'activité F2D57 *« élaborer les cahiers des charges fonctionnels pour la réalisation de dispositifs et de ressources »* : 
l'arborescence et la navigation (`mkdocs.yml`) ont été pensées avant la production du contenu, comme le ferait un cahier des charges fonctionnel, une démarche typique **d'ingénierie pédagogique.**

## 3. Choix techniques et justification

### MkDocs Material

Permet une documentation claire, hiérarchisée et responsive. Offre une cohérence visuelle immédiate et facilite la diffusion de ressources pédagogiques.

### Media queries

Assurent l'adaptation du contenu aux différents supports (mobile, tablette, desktop), et répondent aux exigences d'accessibilité et d'inclusion.

### Bootstrap

Simplifie la mise en page responsive et propose des composants standardisés, utiles pour des ressources pédagogiques structurées.

### CSS personnalisé (extra.css)

Permet de corriger les débordements de tableaux sur mobile, et montre une capacité à adapter l'outil aux contraintes réelles d'usage.

## 4. Ancrage dans le référentiel F2D57

Au-delà des choix techniques, plusieurs activités identifiées par la fiche F2D57 trouvent un écho direct dans ce projet d'ingénierie pédagogique :

- *« Assurer la mise en place et la gestion des infrastructures, outils et services d'appui à la pédagogie numérique »* : MkDocs Material et GitLab Pages constituent ici une infrastructure complète de publication de ressources.
- *« Mettre en œuvre la chaîne de production-médiatisation des contenus dans le respect des chartes ergonomique, graphique et qualité »* : le thème Material assure une cohérence visuelle et une charte graphique homogène sur l'ensemble du site.
- *« Soutenir la démarche réflexive des enseignants sur leurs pratiques d'enseignement »* : cette page même illustre cette démarche, en questionnant l'usage des outils au regard d'une activité professionnelle réelle.

La fiche souligne enfin, dans ses tendances d'évolution, *« le développement de la mutualisation de la production inter-établissements »* à travers des outils comme **Git**. Ce projet illustre concrètement cette évolution du métier : l'usage de GitLab (dépôt personnel, commits réguliers, issues) permet de structurer, versionner et partager le travail au sein du groupe, dans une logique proche de celle attendue d'un ingénieur pédagogique amené à mutualiser des ressources avec d'autres établissements. L'**ingénierie pédagogique** ne se limite donc plus à la seule conception de contenus : elle intègre aujourd'hui pleinement des compétences techniques de gestion de projet numérique.

## 5. Exemples concrets d'activités

- **Concevoir et adapter des supports** : produire une ressource de cours structurée (cartes Bootstrap et titres hiérarchisés) qui reste lisible sur mobile grâce aux media queries et à la grille responsive.
- **Documenter un dispositif de formation** : utiliser MkDocs pour centraliser des contenus (principe et fonctionnement) et maintenir une version à jour facilement, un changement dans le Markdown se répercutant directement sur le site.
- **Accompagner l'apprentissage** : intégrer des « points d'attention » via des composants (alerts) et organiser les explications pour réduire la charge cognitive, en stabilisant la navigation et la lecture à différents niveaux de zoom.

## 6. Limites et pistes d'amélioration

- Ajouter des exemples interactifs pour renforcer l'apprentissage.
- Intégrer davantage de schémas ou de visuels explicatifs.
- Envisager une version téléchargeable des contenus.

## 7. Conclusion

Le projet répond aux attentes du référentiel F2D57 en proposant un mini-site clair, responsive, structuré et cohérent. Les choix techniques sont justifiés, ancrés dans les missions officielles de l'emploi-type, et illustrent une démarche d'**ingénierie pédagogique** à part entière, à la fois réflexive et opérationnelle.
