# Audit & rework du plan slides — Actions

> Ce fichier est le ticket de suivi de l'audit réalisé sur la trame narrative et le plan slide-by-slide.
> Chaque étape est autonome et peut être traitée dans une session Claude vierge.
>
> **Prérequis pour chaque étape** : lire intégralement les fichiers suivants avant toute modification :
> - `CLAUDE.md` (racine) — contexte projet, éléments non négociables, posture de travail
> - `contenu/REX_Lyon_Craft_Compte_Rendu.md` — trace immuable de la conversation initiale (ne pas modifier)
> - `contenu/REX_Lyon_Craft_Trame_Narrative.md` — trame narrative avec chiffres qualifiés
> - `contenu/REX_Lyon_Craft_Plan_Slides.md` — plan slide-by-slide actuel (17 slides)
> - `contenu/REX_Lyon_Craft_Plan_Action.md` — étapes et statuts du projet
> - Ce fichier (`contenu/REX_Lyon_Craft_Audit_Actions.md`) — pour connaître le statut de chaque action
>
> **Public cible** : Lyon Craft — développeurs et praticiens craft, public averti, pas à convaincre du bien-fondé du craft. Le talk doit les surprendre, les bousculer, leur donner quelque chose à emporter.
>
> **Objectif global de l'audit** : passer de 17 slides à 14-15 slides. Resserrer le récit, renforcer l'impact émotionnel, structurer le duo, éliminer le remplissage.

---

## Étape A — Resserrer l'acte 2 (slides 6-11)

**Statut** : 🔲 À faire

**Diagnostic** : L'acte 2 fait 6 slides (~13 min) pour un message qui tient en une phrase : "on a fait du craft sur SFR, c'était dur, on n'a pas gagné de temps mais on a posé les bases". Le public craft connaît TDD, mob, Kanban — il n'a pas besoin d'une liste. Ce qui l'intéresse c'est la friction avec le réel.

**Actions** :

1. **Slide 7 (Ce qu'on met en place)** : Retirer le format "5 piliers visuels" (TDD / Mob / Kanban / Livraison continue / Allègement périmètre). Le public craft connaît TDD, mob et Kanban — les lister c'est du remplissage. Ne garder en affichage que ce qui les surprendra : la livraison continue en prod (décision organisationnelle, pas juste technique) et l'allègement du périmètre (retrait des fonctionnalités de confort). Les pratiques attendues (TDD, mob, Kanban) passent en une phrase orale, pas en affichage.

2. **Fusionner slides 9 (résultat contrasté) + 10 (7 mois, fondations posées)** : Créer une seule slide "7 mois — résultat contrasté". Affichage : "7 mois" en grand + deux colonnes (craft tenu : intention garantie, pas de régression / craft lâché : modules éprouvés mais retour à la dépendance recette). Intégrer la formulation clé de l'acte 2 et la thèse "Pour aller plus vite, il faut apprendre à livrer sûr." Le contexte (équipe neuve, friction orga, double apprentissage) passe à l'oral.

3. **Slide 11 (analogie apprentissage)** : Décider entre deux options :
   - **Option muscler** : trouver une image forte qui cristallise la tension de l'acte 2 (l'artisan a montré, l'équipe essaye, certains lâchent sous pression — l'outil est là mais la main tremble encore).
   - **Option supprimer** : la transition vers l'acte 3 se fait directement sur la slide fusionnée 9+10, avec le pont "une question émerge : et si on dupliquait ?"
   - Proposer les deux options à l'utilisateur, argumenter, laisser trancher.

4. **Mettre à jour la vue d'ensemble** du plan slides (tableau en bas du fichier) : renuméroter, recalculer les durées cumulées.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`

**Résultat attendu** : acte 2 passe de 6 à 4 slides (~10 min au lieu de ~13 min).

---

## Étape B — Réécrire la formulation clé acte 2

**Statut** : 🔲 À faire — dépend de l'étape A

**Diagnostic** : La formulation actuelle *"On n'a pas fait mieux en temps. On a fait autrement — et on a posé les fondations."* est explicative, pas percutante. "Poser les fondations" est une métaphore morte. Comparée aux formulations des actes 1 et 3, elle ne se retient pas.

**Actions** :

1. Proposer 3 à 5 formulations alternatives. Critères :
   - Courte (une phrase, pas deux)
   - En tension avec le chiffre "7 mois" (autant qu'avant)
   - Capte le courage d'investir sans gain visible immédiat
   - Mémorable — le public doit pouvoir la citer en sortant
   - Cohérente avec le fil rouge menuiserie et les thèses non négociables (voir `CLAUDE.md`)
   - Exemple de direction : *"7 mois. Autant qu'avant. Sauf que cette fois, on savait ce qu'on avait livré."*

2. Présenter les options à l'utilisateur avec les arguments pour/contre de chacune. Laisser trancher.

3. Mettre à jour la formulation dans `REX_Lyon_Craft_Plan_Slides.md` (slide fusionnée 9+10 ou équivalent après étape A) ET dans `REX_Lyon_Craft_Trame_Narrative.md` (section "Formulation clé" de l'acte 2).

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`, `contenu/REX_Lyon_Craft_Trame_Narrative.md`

**Résultat attendu** : une formulation percutante qui se retient, au même niveau que les deux autres thèses.

---

## Étape C — Réordonner l'acte 3 (slides 12-17)

**Statut** : 🔲 À faire — dépend de l'étape A (numérotation)

**Diagnostic** : L'acte 3 est raconté de manière factuelle. La slide 13 (renversement métier) est la pépite émotionnelle mais elle est coincée entre des slides techniques. La slide 16 (formulation clé isolée) risque de tomber à plat comme un panneau qu'on lit. La slide 15 est trop dense (4 idées).

**Actions** :

1. **Réordonner** : placer les leviers techniques (ex-slide 14) AVANT le renversement métier (ex-slide 13). Logique narrative : les chiffres (2 mois) → comment c'est techniquement possible (leviers) → ce que ça a changé dans l'organisation (le renversement = climax de l'acte 3). Le renversement métier doit arriver en dernier dans la séquence, avec de l'espace narratif autour de lui.

2. **Intégrer la formulation clé acte 3** (*"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*) dans une slide existante — soit après les chiffres de Santé Équilibre (quand le public réalise que 2 mois c'est un tiers du temps d'avant), soit dans la slide du renversement métier. Supprimer la slide isolée (ex-slide 16).

3. **Alléger la slide 15 (template + projection)** : garder en affichage le template vivant + l'objectif 150j. Passer à l'oral : formation ihexa, TDD en maintenance sur produits livrés.

4. **Mettre à jour la vue d'ensemble** : renuméroter, recalculer les durées.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`

**Résultat attendu** : acte 3 passe de 6 à 4-5 slides, avec le renversement métier comme climax clair. Plus de slide "citation" isolée.

---

## Étape D — Dynamiser l'ouverture (slide 1)

**Statut** : 🔲 À faire — indépendante des étapes A-C

**Diagnostic** : L'ouverture actuelle décrit un atelier paisible ("Un atelier. On fabrique des chaises."). Pour un public expert à Lyon Craft, les 90 premières secondes décident de l'attention. L'analogie menuiserie est bonne, mais l'entrée manque de friction — on décrit un décor au lieu de créer une tension.

**Actions** :

1. Proposer 2 à 3 variantes d'attaque pour la slide 1. Pistes :
   - Commencer par le test qui échoue : "Une chaise sort de l'atelier. On s'assoit dessus. Ça craque." — puis zoom arrière sur l'atelier.
   - Commencer par la question : "Combien de chaises vous avez livrées cette semaine sans être sûrs qu'elles tiennent ?"
   - Commencer par le geste : "Dans cet atelier, on vérifie les chaises à la fin. Et quand ça craque, on retourne à l'établi."
   - Chaque variante doit poser une tension immédiate, pas un décor.

2. Vérifier la cohérence avec la formulation clé de l'acte 1 (*"On veut produire plus vite, mais on serre les fesses quand on s'assoit dessus."*) — l'ouverture doit amorcer cette image sans la griller.

3. Présenter les options à l'utilisateur avec recommandation. Laisser trancher.

4. Mettre à jour la slide 1 dans `REX_Lyon_Craft_Plan_Slides.md` et la section "Ouverture" dans `REX_Lyon_Craft_Trame_Narrative.md`.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`, `contenu/REX_Lyon_Craft_Trame_Narrative.md`

**Résultat attendu** : le public est accroché dès les 30 premières secondes.

---

## Étape E — Structurer le duo Didier/Laure

**Statut** : 🔲 À faire — dépend des étapes A, C et D (plan slides stabilisé)

**Diagnostic** : En l'état, la trame est écrite comme un monologue de Didier avec Laure qui intervient sur la slide 13 (renversement métier) et peut-être la slide 15 (projection). Si Laure ne parle pas avant la minute 26, le public l'a oubliée. Un talk en duo raté, c'est un monologue avec un témoin.

**Contexte important** (voir `CLAUDE.md` et `REX_Lyon_Craft_Compte_Rendu.md`) :
- **Didier** : freelance craft, impulsion, structuration, pivots techniques. Ce talk sert aussi à valoriser ses compétences.
- **Laure** : toujours chez Alptis, ancrage organisationnel, continuité et résultats post-départ de Didier.
- La répartition doit être une **conversation**, pas des relais.

**Actions** :

1. Proposer une répartition complète slide par slide. Pistes à explorer :
   - **Laure ouvre l'acte 1** : le contexte Alptis (slides 3-4), c'est son terrain — elle y est encore, elle incarne l'organisation.
   - **Didier prend le lead sur l'acte 2** : l'expérimentation craft, c'est son expertise.
   - **Alternance sur l'acte 3** : Laure sur le renversement métier et la projection, Didier sur les leviers techniques.
   - **Ouverture** : Didier seul (analogie menuiserie, c'est sa voix narrative) ou en duo (l'un décrit, l'autre complète).
   - **Conclusion** : Didier pour la punchline (c'est sa conviction), Laure pour l'honnêteté finale (les compromis, ce qui reste à faire).

2. Identifier **3 à 4 moments de ping-pong** : pas des relais formels mais des réactions naturelles. Ex : Didier raconte les 4 phases (slide 8), Laure réagit sur ce qu'elle observait côté orga. Laure raconte le renversement métier, Didier exprime sa surprise. Ces moments doivent être répartis dans le talk, pas concentrés à la fin.

3. Valider que Laure a du temps de parole **dès les 10 premières minutes** — pas seulement à la fin.

4. Mettre à jour `REX_Lyon_Craft_Plan_Slides.md` : ajouter pour chaque slide une ligne "**Qui parle**" avec le format `Didier`, `Laure`, ou `Duo (Didier lead, Laure réagit)`.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`

**Résultat attendu** : le duo est visible et équilibré tout au long du talk. Laure n'est pas un témoin silencieux pendant 25 minutes.

---

## Étape F — Stabiliser le plan slides final

**Statut** : 🔲 À faire — dépend de toutes les étapes précédentes (A à E)

**Diagnostic** : Après les modifications des étapes A à E, le plan slides doit être cohérent, renuméroté, avec des durées réalistes.

**Actions** :

1. Renuméroter toutes les slides de 1 à N (objectif : 14-15 slides).
2. Recalculer les durées cumulées dans la vue d'ensemble (objectif : 30-35 min de présentation + 10-15 min de Q&R).
3. Vérifier la cohérence entre le plan slides et la trame narrative :
   - Chaque formulation clé du plan slides correspond à celle de la trame.
   - Chaque chiffre est identique dans les deux fichiers.
   - Les éléments non négociables de `CLAUDE.md` sont tous présents.
4. Mettre à jour le statut de l'étape 2 dans `REX_Lyon_Craft_Plan_Action.md` (passer de 🔲 à ✅).
5. Mettre à jour ce fichier : passer toutes les étapes A-F à ✅.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`, `contenu/REX_Lyon_Craft_Plan_Action.md`, `contenu/REX_Lyon_Craft_Audit_Actions.md`

**Résultat attendu** : plan slides stabilisé, prêt pour l'étape 3 du projet (trancher les points ouverts) puis l'étape 4 (notes orales par slide).

---

## Ordre de traitement recommandé

```
A (resserrer acte 2) → B (formulation clé acte 2) → C (réordonner acte 3)
                                                        ↑
D (ouverture) ──────────────────────────────────────────┘
                                                        ↓
                                               E (duo Didier/Laure)
                                                        ↓
                                               F (stabilisation finale)
```

A et D peuvent être traitées en parallèle. B dépend de A. C dépend de A (numérotation). E dépend de A, C et D (plan stabilisé). F vient en dernier.
