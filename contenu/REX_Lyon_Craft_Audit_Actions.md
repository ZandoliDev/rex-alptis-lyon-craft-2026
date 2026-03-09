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

## Étape A — Resserrer l'acte 2 (slides 6-10)

**Statut** : ✅ Fait

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

**Statut** : ✅ Fait

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

## Étape C — Réordonner l'acte 3 (slides 11-16 → 11-14)

**Statut** : ✅ Fait

**Diagnostic** : L'acte 3 est raconté de manière factuelle. La slide 13 (renversement métier) est la pépite émotionnelle mais elle est coincée entre des slides techniques. La slide 16 (formulation clé isolée) risque de tomber à plat comme un panneau qu'on lit. La slide 15 est trop dense (4 idées).

**Diagnostic révisé** : La chronologie réelle a inversé l'ordre prévu par l'audit. Le renversement métier (rapprochement actuaires/DSI) est une **condition préalable** à SEQ, pas une conséquence. Les acquis craft de SFR (capture de l'intention, structure du code) sont hérités par duplication. Le seul levier nouveau sur SEQ est le découplage vis-à-vis des services externes. La slide "3 leviers techniques" n'a donc plus de raison d'exister en tant que telle.

**Actions réalisées** :

1. **Réordonné** : le renversement métier ouvre l'acte 3 (slide 11) — c'est ce qui rend la duplication envisageable. Puis SEQ avec les chiffres décomposés (slide 12). La slide "3 leviers techniques" est supprimée — les acquis SFR passent à l'oral, le découplage services externes est intégré dans la slide SEQ.

2. **Formulation clé acte 3** intégrée dans la slide SEQ (slide 12), après la décomposition "2 mois + 1 mois" — la décomposition du chiffre EST la preuve du déplacement du goulot. Slide isolée supprimée.

3. **Slide template + projection allégée** (slide 13) : en affichage le template vivant + objectif 150j. À l'oral : formation ihexa, TDD en maintenance.

4. **Vue d'ensemble mise à jour** : renuméroté (14 slides), durées recalculées.

**Précisions factuelles intégrées** (échanges avec Didier) :
- 2 mois = version quasi complète en prod, **recette comprise**. Le code est prêt rapidement, la recette déroule par prudence un process "from scratch" — quasi aucun retour, ceux qui remontent sont reproductibles sur SFR. Pendant ces 2 mois, la recette est le goulot.
- +1 mois = branchements services externes + spécificités SEQ. Le goulot se déplace une deuxième fois.
- Le dev n'est le goulot à aucun moment.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`, `contenu/REX_Lyon_Craft_Audit_Actions.md`

**Résultat** : acte 3 passe de 6 à 4 slides (~11 min), avec le renversement métier en ouverture d'acte et le chiffre décomposé comme climax. Plus de slide "citation" isolée, plus de slide "leviers techniques" redondante.

---

## Étape D — Dynamiser l'ouverture (slide 1)

**Statut** : ✅ Fait

**Diagnostic** : L'ouverture actuelle décrit un atelier paisible ("Un atelier. On fabrique des chaises."). Pour un public expert à Lyon Craft, les 90 premières secondes décident de l'attention. L'analogie menuiserie est bonne, mais l'entrée manque de friction — on décrit un décor au lieu de créer une tension.

**Actions réalisées** :

1. **Slide 1 dynamisée** : "On a fini de construire la chaise. On s'assoit dessus. Ça craque. On retourne à l'établi. Ce n'est pas de la négligence — c'est comme ça qu'on a toujours fait." Tension immédiate, image sensorielle (le craquement), pas de décor.

2. **Réordonnancement des 5 premières slides** (1-4-2-3-5 → 1-2-3-4-5) : L'atelier (tension) → La douleur (migration, allers-retours) → Qui sommes-nous (après la douleur, le public veut savoir) → La norme (chiffres comme explication) → Formulation clé + question (charnière vers acte 2). La tension arrive dès la slide 1 au lieu de la slide 4-5.

3. **Slide 5 allégée** : le rappel de l'analogie ("on teste les chaises à la fin") est supprimé — déjà posé en slide 1. La slide se concentre sur la formulation clé et la question d'ouverture vers l'acte 2.

4. **Cohérence vérifiée** : le "ça craque" de la slide 1 amorce le "on serre les fesses quand on s'assoit dessus" de la slide 5 sans le griller.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`, `contenu/REX_Lyon_Craft_Trame_Narrative.md`

**Résultat** : le public est accroché dès les 30 premières secondes. La présentation du duo arrive après la douleur (slide 3, ~6 min).

---

## Étape E — Structurer le duo Didier/Laure

**Statut** : ✅ Fait

**Diagnostic** : En l'état, la trame est écrite comme un monologue de Didier avec Laure qui intervient sur la slide 13 (renversement métier) et peut-être la slide 15 (projection). Si Laure ne parle pas avant la minute 26, le public l'a oubliée. Un talk en duo raté, c'est un monologue avec un témoin.

**Actions réalisées** :

1. **Répartition complète slide par slide** définie avec Didier :
   - Didier solo : slides 1, 5, 7, 9, 10, 12 (~13 min)
   - Laure solo : slides 4, 11, 13 (~8 min)
   - Duo : slides 2, 3, 6, 8, 14 (~10 min)

2. **Moments de duo identifiés** :
   - Slide 2 (~4 min) : Laure lead sur la douleur et le contexte, Didier réagit sur son arrivée
   - Slide 3 (~6 min) : chacun se présente
   - Slide 6 (~12 min) : Laure contexte orga, Didier pari craft
   - Slide 8 (~16 min) : Didier raconte les 4 phases, Laure réagit côté orga
   - Slide 14 (~31 min) : duo sur la conclusion

3. **Laure parle dès la slide 2** (~1 min). Jamais plus de 2 slides consécutives sans elle. Présente sur 8 slides sur 14 (3 solo + 5 duo).

4. **Plan slides mis à jour** : ligne "Qui parle" ajoutée à chaque slide + tableau de répartition en vue d'ensemble.

**Fichiers modifiés** : `contenu/REX_Lyon_Craft_Plan_Slides.md`

**Résultat** : le duo est visible et équilibré. Laure parle dès la minute 1, avec des interventions réparties sur tout le talk.

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
