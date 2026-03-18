# Plan slide-by-slide — REX Lyon Craft

> Livrable de l'étape 2.
> Talk de 45 minutes (30-35 min de présentation + 10-15 min de Q&R) — 15 slides.
> Répartition duo Didier/Laure : définie (étape E de l'audit).
> Formulation clé acte 1 : tranchée (PR #2).

---

## Slide 1 — Titre

- **Affichage** : *Et Craft la chaise* — *REX Alptis — Le TDD, un vrai gain de temps* + logo Alptis (`support/assets/logo-alptis-white.svg`) + Didier & Laure + Lyon Craft 2026

---

## Ouverture + Acte 1 — L'héritage : travailler sans filet (slides 2-6) — ~10 min

### Slide 2 — L'atelier
- **Qui parle** : Didier
- **Affichage** : Mini BD — `support/assets/bd-atelier-avant.jpg`
- **Idée** : "On a fini de construire la chaise. On s'assoit dessus. Ça craque. On retourne à l'établi. Ce n'est pas de la négligence — c'est comme ça qu'on a toujours fait."
- **Intention** : Tension immédiate. Le public entend le craquement avant de comprendre l'histoire. Pas de jugement — un constat. Amorce l'analogie menuiserie qui traverse tout le talk.

### Slide 3 — La douleur et le déclic
- **Qui parle** : Duo (Laure lead, Didier réagit) — Laure présente la douleur et le contexte dans lequel Didier arrive, Didier enchaîne sur ce qu'il constate.
- **Affichage** : Visuel d'allers-retours dev ↔ recette (boucle)
- **Idée** : La migration Java 11 → 21 s'étire. Bugs et régressions détectés tardivement. Cycles qui auraient pu être raccourcis avec un filet de tests. C'est cette douleur qui motive la proposition craft. L'envie d'aller plus vite existe — mais sans filet, chaque accélération reste un pari. On veut produire plus vite, mais on n'a aucune garantie sur ce qu'on produit.
- **Anecdote** : Arrivée de Didier en pleine migration, l'incertitude permanente du "qu'est-ce que j'ai cassé ?"

### Slide 4 — Qui sommes-nous
- **Qui parle** : Duo — chacun se présente en une phrase.
- **Affichage** : Didier + Laure — noms, rôles
- **Idée** : "On va vous raconter comment cet atelier s'est transformé." Didier : l'artisan qui arrive, impulse le craft, structure les pivots. Laure : l'ancrage dans l'organisation, la continuité après le départ de Didier.
- **Intention** : La présentation arrive après la douleur — le public veut savoir qui parle. Pas un slide CV, une réponse à une question que le public se pose déjà.

### Slide 5 — La norme
- **Qui parle** : Laure
- **Affichage** : Chiffres clés — 6-7 mois / produit, équipe de 4-5 personnes (PO, SA, 3 dev), 3 produits livrés (Select, Protect, Select Pro)
- **Idée** : Voilà d'où on part. C'est la norme. Ça fonctionne. Personne ne la remet en question.
- **Donnée** : 6-7 mois par produit, confirmé sur 3 produits

### Slide 6 — Formulation clé + question
- **Qui parle** : Didier
- **Affichage** : *"On veut produire plus vite, mais on serre les fesses quand on s'assoit dessus."* Puis : "Et si le vrai problème n'était pas la vitesse à laquelle on fabrique — mais la façon dont on fabrique ?"
- **Idée** : La formulation clé fait écho au craquement de la slide 2. La question ouvre l'acte 2.
- **Intention** : Charnière entre acte 1 et acte 2. Le public boucle mentalement sur l'image de la slide 2. Le crescendo est plus court — l'analogie est déjà posée, la formulation clé et la question suffisent.

---

## Acte 2 — L'expérimentation : repartir de zéro (slides 7-11) — ~11 min

### Slide 7 — Le pari : un nouveau produit from scratch
- **Qui parle** : Duo (Laure contexte orga, Didier pari craft)
- **Affichage** : "SFR — Santé Frontaliers Suisses" + contexte (équipe nouvelle, zéro expérience Alptis)
- **Idée** : L'occasion de repartir sur des bases saines. Mais double courbe d'apprentissage : craft + contexte métier.
- **Intention** : Montrer que ce n'est pas un laboratoire confortable — c'est un vrai produit, avec de vraies contraintes.

### Slide 8 — Ce qu'on met en place
- **Qui parle** : Didier
- **Affichage** : 5 leviers de transformation
  - TDD — conception émergente : code construit par petits pas, refactoré en continu — c'est ce qui le rend industrialisable
  - Mob programming : montée en compétence TDD et fonctionnelle de toute l'équipe, en temps réel
  - US itératives : pas de cahier des charges figé, le produit émerge par incréments livrables
  - Livraison continue en prod : on déploie tout au long du projet, pas un big bang à la mise en marché
  - Allègement du périmètre : fonctionnalités de confort retirées, focus sur le cœur métier
- **Intention** : Pas une liste de pratiques craft — chaque levier est là pour une raison dans cette transformation. Le public comprend le pourquoi, pas juste le quoi.

### Slide 9 — Ce qui se passe vraiment
- **Qui parle** : Duo (Didier raconte les 4 phases, Laure réagit sur ce qu'elle observait côté orga)
- **Affichage** : Frise des 4 phases back — Mob (~1,5 mois) → Pair (~1,5 mois) → Hybride (~1 mois) → Sans Didier (~2 mois). Note : côté front, 1 dev formé en pair par Didier, adopte le TDD en autonomie.
- **Idée** : L'accompagnement craft se réduit progressivement. ~3 semaines de friction orga. Congés successifs. Phase hybride avec absences alternées. Puis dev senior seul, pression de deadline, TDD lâché sur certaines zones.
- **Intention** : Honnêteté brute. Le public craft sait que la réalité ne ressemble jamais au plan. C'est ici qu'on gagne leur confiance.

### Slide 10 — 7 mois : résultat contrasté
- **Qui parle** : Didier
- **Affichage** :
  - "7 mois" en grand, puis en sous-titre : *dont 1 mois de retard*
  - Deux colonnes — "Craft tenu" (intention garantie, pas de régression) vs "Craft lâché" (modules éprouvés mais retour à la dépendance recette)
  - Formulation clé : *"On a mis 7 mois. Mais on desserre les fesses."*
  - Thèse : *"Pour aller plus vite, il faut apprendre à livrer sûr."*
- **Idée** : Le chiffre frappe d'abord — 7 mois, autant qu'avant. Les deux colonnes montrent que c'est nuancé, pas triomphal. La formulation clé assume le résultat. La thèse donne le sens. Le contexte (équipe neuve, friction orga, double apprentissage) passe à l'oral.
- **Donnée** : 7 mois SFR vs 6-7 mois avant
- **Intention** : Honnêteté + courage. Le public respecte qu'on ne triche pas sur les chiffres. Le gain se matérialisera à l'acte 3.

### Slide 11 — Analogie : l'apprentissage
- **Qui parle** : Didier
- **Affichage** : Mini BD — `support/assets/bd-apprentissage.jpg`
- **Intention** : Respiration. Le public fait le parallèle avec la réalité qu'on vient de raconter. Transition vers l'acte 3.

---

## Acte 3 — L'industrialisation : la maîtrise comme levier (slides 12-15) — ~12 min

### Slide 12 — Le renversement : le métier vient à nous
- **Qui parle** : Laure
- **Affichage** : Anecdote visuelle — invitation à une réunion, objectif flou. Puis le retournement.
- **Idée** : On reçoit une invitation. On ne sait pas trop pourquoi. On arrive — et on comprend : le métier nous demande comment concevoir le produit pour minimiser le temps de réalisation. "Si x, ça ira vite. Si y, il nous faudra plus de temps — on préconise x." → "OK pour x." Rechallenge des règles spécifiques pour qu'elles conviennent au plus grand nombre. Ce renversement n'est pas tombé du ciel — il a fallu des années pour construire cette confiance. C'est ce renversement qui rend la duplication envisageable.
- **Intention** : Le renversement ouvre l'acte 3 — c'est la condition préalable, pas une conséquence. C'est le vécu de Laure, la continuité qu'elle incarne. Le public comprend que le craft seul ne suffit pas — il faut que l'organisation bouge aussi.

### Slide 13 — Santé Équilibre : 2 mois + 1 mois
- **Qui parle** : Didier
- **Affichage** :
  - "2 mois" en grand — version quasi complète en prod, recette comprise, périmètre plus complet que SFR
  - Puis "+1 mois" — branchements services externes + spécificités SEQ
  - Formulation clé : *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*
  - Thèse : *"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."*
- **Idée** : Duplication de SFR comme base — on part avec les tests (capture de l'intention) et la structure du code, acquis de l'acte 2. Nouveau levier : découplage vis-à-vis des services externes (contrats d'interface, mock/réel par config), qui permet de travailler sans attendre leur disponibilité. Le code est prêt rapidement. La recette déroule par prudence un process "from scratch" — quasi aucun retour, et ceux qui remontent sont reproductibles sur SFR. Pendant 2 mois, c'est la recette qui est le goulot. Puis +1 mois pour les services externes. Le dev n'est plus le goulot à aucun moment.
- **Donnée** : 2 mois (recette comprise) + 1 mois (services externes) vs 7 mois vs 6-7 mois — la courbe se dessine
- **Intention** : La décomposition du chiffre EST la preuve. Le public fait le calcul lui-même. La formulation clé cristallise ce que les chiffres montrent.

### Slide 14 — Le déclic du template + projection
- **Qui parle** : Laure
- **Affichage** : Schéma template → déclinaison produit + objectif DSI 150j (budget 200j) acté au budget 2026
- **Idée** :
  - "On a une base livrable en prod. Pourquoi ne pas en faire un template ?"
  - Template vivant, recetté, toujours à jour. Corrections portées sur produit ET template. Chaque nouveau produit part du template — les déclinaisons se concentrent sur les spécificités.
  - Projection 2026 : objectif DSI parcours de vente en 150j (budget 200j), acté au budget.
- **Oral** : Formation TDD pour les devs hors équipe expérimentale. TDD continue sur les produits livrés (évolutions/maintenance).
- **Intention** : L'histoire ne s'arrête pas au départ de Didier. L'organisation a internalisé.

### Slide 15 — L'atelier transformé + punchline
- **Qui parle** : Duo
- **Affichage** : Mini BD — `support/assets/bd-atelier-transforme.jpg` + *"Développer est un métier. Être artisan développeur en est un autre."*
- **Intention** : Boucler l'analogie — émotion, lucidité. Silence. La punchline arrive sur l'émotion. Le public repart avec cette phrase et cette image. Provocation assumée, crédibilisée par les 35 minutes qui précèdent.

---

## Vue d'ensemble

| Slide | Acte | Titre court | Qui parle | Durée cumulée |
|-------|------|-------------|-----------|---------------|
| 1 | — | Titre | — | ~0 min |
| 2 | Ouverture | L'atelier — "ça craque" | Didier | ~1 min |
| 3 | Acte 1 | La douleur et le déclic | Duo (Laure lead) | ~4 min |
| 4 | Acte 1 | Qui sommes-nous | Duo | ~6 min |
| 5 | Acte 1 | La norme | Laure | ~8 min |
| 6 | Acte 1 | Formulation clé + question | Didier | ~10 min |
| 7 | Acte 2 | Le pari SFR | Duo | ~12 min |
| 8 | Acte 2 | Ce qu'on met en place | Didier | ~14 min |
| 9 | Acte 2 | Ce qui se passe vraiment | Duo | ~16 min |
| 10 | Acte 2 | 7 mois — résultat contrasté | Didier | ~19 min |
| 11 | Acte 2 | Analogie — l'apprentissage | Didier | ~20 min |
| 12 | Acte 3 | Le renversement : le métier vient à nous | Laure | ~23 min |
| 13 | Acte 3 | SEQ : 2 mois + 1 mois | Didier | ~26 min |
| 14 | Acte 3 | Template + projection 2026 | Laure | ~28 min |
| 15 | Acte 3 | L'atelier transformé + punchline | Duo | ~31 min |

### Répartition du temps de parole

| | Didier solo | Laure solo | Duo |
|---|---|---|---|
| Slides | 2, 6, 8, 10, 11, 13 | 5, 12, 14 | 3, 4, 7, 9, 15 |
| Nombre | 6 | 3 | 5 |
| Durée estimée | ~13 min | ~8 min | ~10 min |
