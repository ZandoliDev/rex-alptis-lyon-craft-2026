# Plan slide-by-slide — REX Lyon Craft

> Livrable de l'étape 2.
> Talk de 45 minutes (30-35 min de présentation + 10-15 min de Q&R) — 16 slides.
> Répartition duo Didier/Laure : à définir à l'étape suivante.
> Formulation clé acte 1 : tranchée (PR #2).

---

## Ouverture (slides 1-2) — ~3 min

### Slide 1 — L'atelier
- **Affichage** : Image/métaphore visuelle d'un atelier de menuiserie — on fabrique des chaises
- **Idée** : "Un atelier. On fabrique des chaises."
- **Intention** : Poser l'image. Pas de jugement, pas de contexte, juste un lieu et une activité. Le public entre dans l'histoire.

### Slide 2 — Qui sommes-nous
- **Affichage** : Didier + Laure — noms, rôles
- **Idée** : "On va vous raconter comment cet atelier s'est transformé." Didier : l'artisan qui arrive, impulse le craft, structure les pivots. Laure : l'ancrage dans l'organisation, la continuité après le départ de Didier.
- **Intention** : Inclure le public — vous allez observer cette transformation avec nous. Poser le duo naturellement, pas un slide CV.

---

## Acte 1 — L'héritage : travailler sans filet (slides 3-5) — ~7 min

### Slide 3 — Le contexte Alptis
- **Affichage** : Chiffres clés — 6-7 mois / produit, équipe de 4-5 personnes (PO, SA, 3 dev), 3 produits livrés (Select, Protect, Select Pro)
- **Idée** : Poser le décor. C'est la norme. Ça fonctionne.
- **Donnée** : 6-7 mois par produit, confirmé sur 3 produits

### Slide 4 — La douleur et le déclic
- **Affichage** : Visuel d'allers-retours dev ↔ recette (boucle)
- **Idée** : La migration Java 11 → 21 s'étire. Bugs et régressions détectés tardivement. Cycles qui auraient pu être raccourcis avec un filet de tests. C'est cette douleur qui motive la proposition craft. L'envie d'aller plus vite existe — mais sans filet, chaque accélération reste un pari. On veut produire plus vite, mais on n'a aucune garantie sur ce qu'on produit.
- **Anecdote** : Arrivée de Didier en pleine migration, l'incertitude permanente du "qu'est-ce que j'ai cassé ?"

### Slide 5 — Analogie + formulation clé + question
- **Affichage** : L'atelier — "on teste les chaises à la fin. Quand ça craque, on retourne à l'établi." Puis la formulation clé : *"On veut produire plus vite, mais on serre les fesses quand on s'assoit dessus."* Puis : "Et si le vrai problème n'était pas la vitesse — mais la façon dont on fabrique ?"
- **Idée** : Le public a vu le problème concret (migration, allers-retours). L'analogie le cristallise. La formulation clé fait mouche — elle dit en une phrase ce que la slide 4 a montré. La question ouvre l'acte 2.
- **Intention** : Charnière entre acte 1 et acte 2. L'analogie, la formulation et la question forment un crescendo. Le public fait le lien lui-même.

---

## Acte 2 — L'expérimentation : repartir de zéro (slides 6-10) — ~11 min

### Slide 6 — Le pari : un nouveau produit from scratch
- **Affichage** : "SFR — Santé Frontaliers Suisses" + contexte (équipe nouvelle, zéro expérience Alptis)
- **Idée** : L'occasion de repartir sur des bases saines. Mais double courbe d'apprentissage : craft + contexte métier.
- **Intention** : Montrer que ce n'est pas un laboratoire confortable — c'est un vrai produit, avec de vraies contraintes.

### Slide 7 — Ce qu'on met en place
- **Affichage** : 5 leviers de transformation
  - TDD — conception émergente : code construit par petits pas, refactoré en continu — c'est ce qui le rend industrialisable
  - Mob programming : montée en compétence TDD et fonctionnelle de toute l'équipe, en temps réel
  - US itératives : pas de cahier des charges figé, le produit émerge par incréments livrables
  - Livraison continue en prod : on déploie tout au long du projet, pas un big bang à la mise en marché
  - Allègement du périmètre : fonctionnalités de confort retirées, focus sur le cœur métier
- **Intention** : Pas une liste de pratiques craft — chaque levier est là pour une raison dans cette transformation. Le public comprend le pourquoi, pas juste le quoi.

### Slide 8 — Ce qui se passe vraiment
- **Affichage** : Frise des 4 phases back — Mob (~1,5 mois) → Pair (~1,5 mois) → Hybride (~1 mois) → Sans Didier (~2 mois). Note : côté front, 1 dev formé en pair par Didier, adopte le TDD en autonomie.
- **Idée** : L'accompagnement craft se réduit progressivement. ~3 semaines de friction orga. Congés successifs. Phase hybride avec absences alternées. Puis dev senior seul, pression de deadline, TDD lâché sur certaines zones.
- **Intention** : Honnêteté brute. Le public craft sait que la réalité ne ressemble jamais au plan. C'est ici qu'on gagne leur confiance.

### Slide 9 — 7 mois : résultat contrasté
- **Affichage** :
  - "7 mois" en grand, puis en sous-titre : *dont 1 mois de retard*
  - Deux colonnes — "Craft tenu" (intention garantie, pas de régression) vs "Craft lâché" (modules éprouvés mais retour à la dépendance recette)
  - Formulation clé : *"On n'a pas fait mieux en temps. On a fait autrement — et on a posé les fondations."*
  - Thèse : *"Pour aller plus vite, il faut apprendre à livrer sûr."*
- **Idée** : Le chiffre frappe d'abord — 7 mois, autant qu'avant. Les deux colonnes montrent que c'est nuancé, pas triomphal. La formulation clé assume le résultat. La thèse donne le sens. Le contexte (équipe neuve, friction orga, double apprentissage) passe à l'oral.
- **Donnée** : 7 mois SFR vs 6-7 mois avant
- **Intention** : Honnêteté + courage. Le public respecte qu'on ne triche pas sur les chiffres. Le gain se matérialisera à l'acte 3.

### Slide 10 — Analogie : l'apprentissage
- **Affichage** : L'atelier — l'artisan a montré les techniques d'assemblage, le tenon-mortaise, formé sur les outils adaptés. On a retenu les techniques, on essaye de se les approprier, on n'est pas encore complètement à l'aise.
- **Intention** : Respiration. Le public fait le parallèle avec la réalité qu'on vient de raconter. Transition vers l'acte 3.

---

## Acte 3 — L'industrialisation : la maîtrise comme levier (slides 11-16) — ~12 min

### Slide 11 — Santé Équilibre : la duplication
- **Affichage** : "2 mois" en grand — périmètre plus complet que SFR, zéro retard côté dev
- **Idée** : Produit plus standard. Duplication de SFR comme base. 2 mois pour une première version quasi complète en prod, avant la date de mise en marché.
- **Donnée** : 2 mois vs 7 mois vs 6-7 mois — la courbe se dessine

### Slide 12 — Le renversement : le métier vient à nous
- **Affichage** : Anecdote visuelle — invitation à une réunion, objectif flou. Puis le retournement.
- **Idée** : On reçoit une invitation. On ne sait pas trop pourquoi. On arrive — et on comprend : le métier nous demande comment concevoir le produit pour minimiser le temps de réalisation. "Si x, ça ira vite. Si y, il nous faudra plus de temps — on préconise x." → "OK pour x." Rechallenge des règles spécifiques pour qu'elles conviennent au plus grand nombre. Ce renversement n'est pas tombé du ciel — il a fallu des années pour construire cette confiance.
- **Intention** : C'est Laure qui raconte — c'est son vécu, la continuité qu'elle incarne. Didier réagit en tant que témoin surpris de ce retournement. Le public comprend que le craft seul ne suffit pas — il faut que l'organisation bouge aussi. Et que ça prend du temps.

### Slide 13 — Les 3 leviers techniques
- **Affichage** : 3 blocs visuels
- **Idée** :
  1. Capture de l'intention (tests = documentation du sens)
  2. Structure du code (découplage, patterns, conçu pour évoluer)
  3. Autonomie vis-à-vis des dépendances (contrats d'interface, mock/réel par config)
- **Intention** : La combinaison de ces leviers techniques avec le rapprochement métier produit le résultat.

### Slide 14 — Le déclic du template + projection
- **Affichage** : Schéma template → déclinaison produit
- **Idée** :
  - "On a une base livrable en prod. Pourquoi ne pas en faire un template ?"
  - Template vivant, recetté, toujours à jour. Corrections portées sur produit ET template.
  - Projection 2026 : objectif DSI parcours de vente en 150j (budget 200j), acté au budget
  - Formation TDD (ihexa) pour les devs hors équipe expérimentale
  - TDD continue sur les produits livrés (évolutions/maintenance)
- **Intention** : L'histoire ne s'arrête pas au départ de Didier. L'organisation a internalisé.

### Slide 15 — Formulation clé acte 3
- **Affichage** : *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*
- **Idée** : Ce n'est plus le dev qui bloque. +1 mois pour les services externes sur Santé Équilibre. Quasi aucun retour en recette.
- **Intention** : Le public craft comprend immédiatement ce que ça signifie.

### Slide 16 — L'atelier transformé + punchline
- **Affichage** : L'atelier — même lieu, mais transformé. On sait comment faire une chaise qui tient debout. On se concentre maintenant sur la personnalisation de la chaise vis-à-vis de la demande du client. Puis : *"Développer est un métier. Être artisan développeur en est un autre."*
- **Intention** : Boucler l'analogie — émotion, lucidité. Silence. La punchline arrive sur l'émotion. Le public repart avec cette phrase et cette image. Provocation assumée, crédibilisée par les 35 minutes qui précèdent.

---

## Vue d'ensemble

| Slide | Acte | Titre court | Durée cumulée |
|-------|------|-------------|---------------|
| 1 | Ouverture | L'atelier | ~1 min |
| 2 | Ouverture | Qui sommes-nous | ~3 min |
| 3 | Acte 1 | Contexte Alptis | ~5 min |
| 4 | Acte 1 | La douleur et le déclic | ~8 min |
| 5 | Acte 1 | Analogie + formulation + question | ~10 min |
| 6 | Acte 2 | Le pari SFR | ~12 min |
| 7 | Acte 2 | Ce qu'on met en place | ~14 min |
| 8 | Acte 2 | Ce qui se passe vraiment | ~16 min |
| 9 | Acte 2 | 7 mois — résultat contrasté | ~19 min |
| 10 | Acte 2 | Analogie — l'apprentissage | ~20 min |
| 11 | Acte 3 | 2 mois — Santé Équilibre | ~22 min |
| 12 | Acte 3 | Le renversement : le métier vient à nous | ~24 min |
| 13 | Acte 3 | Les 3 leviers techniques | ~26 min |
| 14 | Acte 3 | Template + projection 2026 | ~28 min |
| 15 | Acte 3 | Formulation clé acte 3 | ~29 min |
| 16 | Acte 3 | L'atelier transformé + punchline | ~33 min |
