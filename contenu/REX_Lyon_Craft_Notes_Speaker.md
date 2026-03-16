# Notes speaker par slide — REX Lyon Craft

> Livrable de l'étape 5.
> Aide-mémoire : ce qu'il faut dire à l'oral **en plus** de ce qui est affiché.
> **D** = Didier · **L** = Laure

---

## Slide 1 — L'atelier (D)

- La BD pose l'image, le texte oral raconte : chaise construite, on s'assoit, ça craque, retour à l'établi
- Constat sans jugement : « c'est comme ça qu'on a toujours fait »
- Ne pas expliquer l'analogie — le public comprendra au fil du talk

## Slide 2 — La douleur et le déclic (L puis D)

- **L** : contexte Alptis — migration Java 11 → 21 en cours, bugs détectés tard, allers-retours dev ↔ recette
- **L** : l'envie d'aller plus vite existe, mais sans filet chaque accélération = pari
- **D** : arrivée en pleine migration — incertitude permanente « qu'est-ce que j'ai cassé ? »
- **D** : on rallonge la recette par précaution, on ralentit parce qu'on n'est jamais sûrs
- **D** : c'est cette douleur qui fait émerger l'idée d'essayer autrement

## Slide 3 — Qui sommes-nous (D puis L)

- **D** : freelance craft, arrive avec la proposition de repartir sur des bases saines
- **L** : [son rôle chez Alptis — à compléter]. Ancrage orga, continuité post-départ Didier
- Conclure ensemble : « on va vous raconter comment cet atelier s'est transformé »

## Slide 4 — La norme (L)

- Poser le référentiel : 6-7 mois / produit, équipe 4-5 (PO, SA, 3 dev)
- Confirmé sur 3 produits : Select, Protect, Select Pro
- Insister : ça fonctionne, personne ne remet en question

## Slide 5 — Formulation clé + question (D)

- Écho au craquement de la slide 1
- La question ouvre l'acte 2 : le problème c'est la façon de fabriquer, pas la vitesse

## Slide 6 — Le pari SFR (L puis D)

- **L** : nouveau produit from scratch — Santé Frontaliers Suisses. Équipe nouvelle, zéro expérience Alptis
- **D** : double pari — apprendre craft + contexte métier en même temps. Pas un labo, un vrai produit avec une vraie date

## Slide 7 — Ce qu'on met en place (D)

- Expliquer le **pourquoi** de chaque levier, pas juste le quoi :
  - TDD : c'est ce qui rend le code industrialisable
  - Mob : review et recette croisée allégées quand on code à 3
  - US itératives : le produit émerge, pas de CDC figé
  - Livraison continue : pas de big bang
  - Allègement périmètre : confort retiré, focus cœur métier

## Slide 8 — Ce qui se passe vraiment (D puis L)

- **D** : les 4 phases back — mob, pair, hybride, sans Didier
  - Phase hybride : absences alternées, arrivée d'une dev expérimentée Alptis
  - Derniers 2 mois : dev senior seul, pression deadline → TDD lâché sur certaines zones
- **L** : ~3 semaines de friction orga (standardisation produit, pas de la complexité technique)
- **D** : côté front — 1 dev formé en pair, adopte le TDD en autonomie sur tout le projet

## Slide 9 — 7 mois : résultat contrasté (D)

- 7 mois = autant qu'avant — mais avec équipe neuve, friction orga, double apprentissage
- Contraste craft tenu / craft lâché : intention garantie vs retour dépendance recette
- Contexte à rappeler à l'oral : en conditions normales, ~6 mois
- Thèse : « pour aller plus vite, il faut apprendre à livrer sûr »

## Slide 10 — L'apprentissage (D)

- La BD porte le message — à l'oral juste accompagner l'image
- Respiration, transition vers l'acte 3
- L'équipe a retenu les techniques, pas encore complètement à l'aise

## Slide 11 — Le renversement (L)

- Raconter l'anecdote : invitation à une réunion, objectif flou
- Arrivée → le métier (actuaires) demande comment concevoir le produit pour minimiser le temps de réalisation
- « Si x, ça ira vite. Si y, plus de temps. On préconise x. » → « OK pour x. »
- Ce renversement a pris des années de collaboration — pas tombé du ciel
- Le craft seul ne suffit pas, il faut que l'orga bouge aussi

## Slide 12 — Santé Équilibre : 2 mois + 1 mois (D)

- On duplique SFR : tests (capture intention) + structure du code
- Nouveau levier : découplage services externes (contrats d'interface, mock/réel par config)
- 2 mois : version quasi complète en prod, recette comprise, périmètre > SFR
- +1 mois : branchements services externes
- En recette : quasi aucun retour — retours hérités déjà absorbés
- Le dev n'est le goulot à aucun moment

## Slide 13 — Template + projection (L)

- Déclic : « on a une base en prod, pourquoi pas un template ? »
- Template vivant, recetté, toujours à jour — corrections portées sur produit ET template
- Objectif DSI 2026 : 150j (budget 200j)
- Formation TDD en cours pour les devs hors équipe expérimentale
- TDD continue sur les produits livrés (évolutions/maintenance)
- L'organisation a internalisé — ça ne s'arrête pas au départ de Didier

## Slide 14 — L'atelier transformé + punchline (D puis L)

- **D** : la BD montre l'atelier transformé — accompagner l'image
- **D** : on sait faire une chaise qui tient, on se concentre sur la personnalisation
- **L** : enchaîner sur le même ton
- Punchline après un silence : « Développer est un métier. Être artisan développeur en est un autre. »
- **L** : « Merci »
