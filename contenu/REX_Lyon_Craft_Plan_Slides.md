# Plan slide-by-slide — REX Lyon Craft

> Livrable de l'étape 2.
> Talk de 45 minutes (30-32 min de présentation + 10-15 min de Q&R) — 16 slides.
> Répartition duo Didier/Laure : à définir à l'étape suivante.
> Formulation clé acte 1 : `[À TRANCHER]` (discussion en cours sur PR #2).

---

## Ouverture (slides 1-2) — ~3 min

### Slide 1 — L'atelier de menuiserie
- **Affichage** : Titre du talk + noms des intervenants, sur une image/métaphore visuelle de l'atelier — des chaises fabriquées, testées en fin de chaîne
- **Idée** : "Chaque chaise est construite, puis testée à la fin. Quand ça craque, on retourne à l'établi. Ce n'est pas de la négligence. C'est simplement la façon dont l'atelier a toujours fonctionné."
- **Intention** : Le public se reconnaît. Pas de jugement, juste un constat.

### Slide 2 — La question
- **Affichage** : "Et si le vrai problème n'était pas la vitesse — mais la façon dont on fabrique ?"
- **Idée** : Tension posée. Le coût invisible : allers-retours, incertitude, charge mentale. Difficulté croissante à fabriquer plus vite sans perdre en qualité.
- **Intention** : Ouvrir la curiosité, annoncer qu'on va raconter une histoire vraie.

---

## Acte 1 — L'héritage : travailler sans filet (slides 3-4) — ~5 min

### Slide 3 — Le contexte Alptis
- **Affichage** : Chiffres clés — 6-7 mois / produit, équipe de 4-5 personnes (PO, SA, 3 dev), 3 produits livrés (Select, Protect, Select Pro)
- **Idée** : Poser le décor. C'est la norme. Ça fonctionne.
- **Donnée** : 6-7 mois par produit, confirmé sur 3 produits

### Slide 4 — La douleur et le déclic
- **Affichage** : Visuel d'allers-retours dev ↔ recette (boucle) + `[À TRANCHER]` — phrase percutante sur le paradoxe vitesse/filet
- **Idée** : La migration Java 11 → 21 s'étire. Bugs et régressions détectés tardivement. Cycles qui auraient pu être raccourcis avec un filet de tests. C'est cette douleur qui motive la proposition craft. L'envie d'aller plus vite existe (design system, composants business). Mais sans filet, chaque accélération reste un pari. L'ambition est là — il manque un levier.
- **Anecdote** : Arrivée de Didier en pleine migration, l'incertitude permanente du "qu'est-ce que j'ai cassé ?"
- **Intention** : Fermer l'acte 1 avec une tension qui appelle l'acte 2.

---

## Acte 2 — L'expérimentation : repartir de zéro (slides 5-9) — ~10 min

### Slide 5 — Le pari : un nouveau produit from scratch
- **Affichage** : "SFR — Santé Frontaliers Suisses" + contexte (équipe nouvelle, zéro expérience Alptis)
- **Idée** : L'occasion de repartir sur des bases saines. Mais double courbe d'apprentissage : craft + contexte métier.
- **Intention** : Montrer que ce n'est pas un laboratoire confortable — c'est un vrai produit, avec de vraies contraintes.

### Slide 6 — Ce qu'on met en place
- **Affichage** : 5 piliers visuels — TDD / Mob programming / Kanban / Livraison continue en prod / Allègement du périmètre
- **Idée** :
  - TDD : conception émergente, code qui exprime l'intention métier
  - Mob : transfert de compétences craft ↔ contexte Alptis, review et recette allégées
  - Kanban : design sprint 2-3 jours, pas de cahier des charges complet, demandes métier en cours de route
  - Livraison continue en prod : déployer tout au long du projet, pas uniquement à la mise en marché — réduit la charge mentale de la mise en prod finale
  - Allègement du périmètre : fonctionnalités de confort retirées, focus sur le cœur métier — ajoutées après coup
- **Intention** : Concret, pas théorique. Le public craft connaît ces pratiques — ce qui l'intéresse c'est le contexte réel. Les deux derniers piliers montrent que le craft ne se limite pas aux pratiques de code.

### Slide 7 — Ce qui se passe vraiment
- **Affichage** : Frise des 4 phases back — Mob (~1,5 mois) → Pair (~1,5 mois) → Hybride (~1 mois) → Sans Didier (~2 mois). Note : côté front, 1 dev formé en pair par Didier, adopte le TDD en autonomie.
- **Idée** : L'accompagnement craft se réduit progressivement. ~3 semaines de friction orga. Congés successifs. Phase hybride avec absences alternées. Puis dev senior seul, pression de deadline, TDD lâché sur certaines zones.
- **Intention** : Honnêteté brute. Le public craft sait que la réalité ne ressemble jamais au plan. C'est ici qu'on gagne leur confiance.

### Slide 8 — Le résultat contrasté
- **Affichage** : Deux colonnes — "Là où le craft tient" vs "Là où il lâche"
- **Idée** :
  - Craft tenu : intention garantie, pas de régression
  - Craft lâché : modules éprouvés mais on perd la certitude, retour à la dépendance recette
- **Intention** : Pas de triomphalisme. Montrer que le craft n'est pas magique — il est exigeant.

### Slide 9 — 7 mois : les fondations sont posées
- **Affichage** : "7 mois" en grand — avec le contexte en dessous (équipe neuve, friction orga, double apprentissage). *"On n'a pas fait mieux en temps. On a fait autrement — et on a posé les fondations."*
- **Idée** : Autant que l'existant. Les pratiques posées slide 6 réduisent l'incertitude et la charge mentale — plus de big bang. Mais pas encore de gain de temps visible : mise en marché retardée d'1 mois. Les fondations sont posées, le gain se matérialisera à l'acte 3. Thèse de l'acte — "Pour aller plus vite, il faut apprendre à livrer sûr." En conditions normales : ~6 mois.
- **Donnée** : 7 mois SFR vs 6-7 mois avant
- **Intention** : Transition — une question émerge : et si on dupliquait ?

---

## Acte 3 — L'industrialisation : la maîtrise comme levier (slides 10-14) — ~10 min

### Slide 10 — Santé Équilibre : la duplication
- **Affichage** : "2 mois" en grand — périmètre plus complet que SFR, zéro retard côté dev
- **Idée** : Produit plus standard. Duplication de SFR comme base. 2 mois pour une première version quasi complète en prod, avant la date de mise en marché.
- **Donnée** : 2 mois vs 7 mois vs 6-7 mois — la courbe se dessine

### Slide 11 — Le rapprochement métier/DSI
- **Affichage** : À définir — illustrer la bascule (avant/après)
- **Idée** : Premier levier, et pas des moindres. La complexité du produit à développer dépend directement des exigences métier. Avant : les actuaires conçoivent des produits indépendamment de la faisabilité technique et du budget. Après : les métiers se rapprochent d'eux-mêmes de la DSI pour co-concevoir des produits réalisables rapidement, en évitant les règles métier exotiques. Mouvement initié côté métier — étonnant et très apprécié des équipes de dev.
- **Intention** : Laure illustre ce levier — d'où la relation est partie, comment le rapprochement s'est construit chez Alptis.

### Slide 12 — Les 3 leviers techniques
- **Affichage** : 3 blocs visuels
- **Idée** :
  1. Capture de l'intention (tests = documentation du sens)
  2. Structure du code (découplage, patterns, conçu pour évoluer)
  3. Autonomie vis-à-vis des dépendances (contrats d'interface, mock/réel par config)
- **Intention** : La combinaison de ces leviers techniques avec le rapprochement métier produit le résultat.

### Slide 13 — Le déclic du template + projection
- **Affichage** : Schéma template → déclinaison produit
- **Idée** :
  - "On a une base livrable en prod. Pourquoi ne pas en faire un template ?"
  - Template vivant, recetté, toujours à jour. Corrections portées sur produit ET template.
  - Projection 2026 : objectif DSI parcours de vente en 150j (budget 200j), acté au budget
  - Formation TDD (ihexa) pour les devs hors équipe expérimentale
  - TDD continue sur les produits livrés (évolutions/maintenance)
- **Intention** : L'histoire ne s'arrête pas au départ de Didier. L'organisation a internalisé.

### Slide 14 — Formulation clé acte 3
- **Affichage** : *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*
- **Idée** : Ce n'est plus le dev qui bloque. +1 mois pour les services externes sur Santé Équilibre. Quasi aucun retour en recette.
- **Intention** : Le public craft comprend immédiatement ce que ça signifie.

---

## Conclusion (slides 15-16) — ~4 min

### Slide 15 — Retour à l'atelier
- **Affichage** : L'atelier transformé — même image qu'en ouverture, mais l'atelier a changé
- **Idée** : On ne réinvente plus la chaise à chaque commande. On a conçu un modèle de fabrication — testé, validé, vivant. Les artisans se concentrent sur les spécificités, pas sur ce qui est déjà résolu. Honnêteté : compromis, zones sans TDD, turbulences. Le craft n'est pas une recette magique — c'est un investissement avec une courbe d'apprentissage réelle. Mais là où l'intention a été tenue : pas de régression, pas de surprise, de la prévisibilité.
- **Intention** : Boucler l'analogie. Émotion + lucidité.

### Slide 16 — Punchline
- **Affichage** : *"Développer est un métier. Être artisan développeur en est un autre."*
- **Idée** : Silence. Laisser la phrase agir.
- **Intention** : Le public repart avec cette phrase. Provocation assumée, crédibilisée par les 30 minutes qui précèdent.

---

## Vue d'ensemble

| Slide | Acte | Titre court | Durée cumulée |
|-------|------|-------------|---------------|
| 1 | Ouverture | L'atelier de menuiserie | ~1,5 min |
| 2 | Ouverture | La question | ~3 min |
| 3 | Acte 1 | Contexte Alptis | ~5 min |
| 4 | Acte 1 | La douleur et le déclic | ~8 min |
| 5 | Acte 2 | Le pari SFR | ~10 min |
| 6 | Acte 2 | Ce qu'on met en place | ~12 min |
| 7 | Acte 2 | Ce qui se passe vraiment | ~14 min |
| 8 | Acte 2 | Résultat contrasté | ~16 min |
| 9 | Acte 2 | 7 mois — fondations posées | ~18 min |
| 10 | Acte 3 | 2 mois — Santé Équilibre | ~20 min |
| 11 | Acte 3 | Rapprochement métier/DSI | ~22 min |
| 12 | Acte 3 | Les 3 leviers techniques | ~24 min |
| 13 | Acte 3 | Template + projection 2026 | ~26 min |
| 14 | Acte 3 | Formulation clé acte 3 | ~28 min |
| 15 | Conclusion | Retour à l'atelier | ~30 min |
| 16 | Conclusion | Punchline | ~32 min |
