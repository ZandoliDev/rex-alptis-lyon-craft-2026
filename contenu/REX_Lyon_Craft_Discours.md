# Notes orales par slide — REX Lyon Craft

> Livrable de l'étape 5.
> Ce qui se **dit**, pas ce qui s'affiche. Chaque bloc = le script oral d'une slide.
> Les indications entre crochets `[…]` sont des directions scéniques (ton, rythme, gestes).
> **D** = Didier · **L** = Laure · **→** = passage de parole

---

## Slide 1 — L'atelier (Didier) · ~1 min

**D** : [Ton calme, posé. Pas de sourire. Regard dans la salle.]

On a fini de construire la chaise.

[Pause courte.]

On s'assoit dessus.

[Pause.]

Ça craque.

[Laisser le silence — 2 secondes. Le public doit entendre le craquement mentalement.]

On retourne à l'établi. On regarde les pieds, les assemblages, on cherche ce qui a lâché. On répare. On se rassoit. Et on espère que cette fois, ça tient.

Ce n'est pas de la négligence. C'est comme ça qu'on a toujours fait.

[Pause. Transition vers Laure — regard, léger recul.]

---

## Slide 2 — La douleur et le déclic (Duo : Laure lead, Didier réagit) · ~3 min

**L** : Chez Alptis, on est en pleine migration Java 11 vers Java 21. Les produits existants tournent, mais chaque changement génère son lot de surprises. Des bugs détectés tard, des allers-retours entre le dev et la recette. Des cycles qui s'étirent sans qu'on sache vraiment pourquoi.

L'envie d'aller plus vite, elle est là. Mais sans filet, chaque accélération reste un pari.

**→ D** : [Enchaîne naturellement, comme s'il répondait.]

C'est à ce moment-là que j'arrive. Et la première chose que je constate, c'est cette incertitude permanente. À chaque modification, la même question : « qu'est-ce que j'ai cassé sans le savoir ? »

On fait tourner les tests manuels. On demande de la validation. On rallonge la recette par précaution. Et au final, on ralentit — pas parce qu'on est lents, mais parce qu'on n'est jamais sûrs.

C'est cette douleur-là qui fait émerger l'idée : et si on essayait autrement ?

---

## Slide 3 — Qui sommes-nous (Duo) · ~2 min

**D** : [Ton direct, détendu.]

Je suis Didier. Développeur freelance, praticien craft. Chez Alptis, c'est moi qui arrive avec la proposition : on repart sur des bases saines, on structure, on teste autrement.

**→ L** : [Se tourne vers la salle.]

Et moi c'est Laure. [Rôle chez Alptis — à compléter par Laure]. Je suis l'ancrage dans l'organisation. Celle qui était là avant Didier, et qui est toujours là après.

**→ D** : On va vous raconter comment cet atelier s'est transformé.

[Transition naturelle — pas de pause longue, on enchaîne sur la norme.]

---

## Slide 4 — La norme (Laure) · ~2 min

**L** : Avant qu'on parle de craft, il faut que vous compreniez d'où on part.

Chez Alptis, un parcours de vente santé, c'est 6 à 7 mois de réalisation. Une équipe de 4 à 5 personnes : un PO, un solution architect, trois développeurs. On a livré comme ça Select, Protect, Select Pro. Trois produits, même durée, même équipe.

[Ton factuel, pas de jugement.]

C'est la norme. Ça fonctionne. Personne ne la remet en question.

---

## Slide 5 — Formulation clé + question (Didier) · ~2 min

**D** : [Léger sourire, ton complice avec la salle.]

En fait, on veut produire plus vite… mais on serre les fesses quand on s'assoit dessus.

[Laisser la salle réagir — sourires, rires. 2-3 secondes.]

[Ton plus sérieux.]

Et si le vrai problème, ce n'était pas la vitesse à laquelle on fabrique — mais la **façon** dont on fabrique ?

[Silence. 3 secondes. Laisser la question s'installer. Change de slide.]

---

## Slide 6 — Le pari SFR (Duo : Laure contexte, Didier pari) · ~2 min

**L** : L'opportunité se présente avec un nouveau produit : Santé Frontaliers Suisses. SFR. Un produit from scratch — pas de legacy, pas de contraintes héritées.

Mais l'équipe est nouvelle. Personne n'a d'expérience Alptis. Ils découvrent le métier en même temps que la méthode.

**→ D** : C'est un double pari. Apprendre le craft et apprendre le contexte métier en même temps. Ce n'est pas un laboratoire confortable — c'est un vrai produit, avec de vraies contraintes et une vraie date de mise en marché.

---

## Slide 7 — Ce qu'on met en place (Didier) · ~2 min

**D** : On met en place cinq leviers. Et chacun est là pour une raison précise dans cette transformation.

[Rythme posé, un levier à la fois. Pointer ou marquer visuellement chaque item.]

**TDD** — conception émergente. Le code se construit par petits pas, refactoré en continu. C'est ça qui le rend industrialisable plus tard.

**Mob programming** — toute l'équipe travaille ensemble. Montée en compétence craft et fonctionnelle en temps réel. La review et la recette croisée deviennent quasi inutiles quand on code à trois.

**US itératives** — pas de cahier des charges figé. Le produit émerge par incréments livrables.

**Livraison continue en prod** — on déploie tout au long du projet. Pas de big bang à la mise en marché.

**Allègement du périmètre** — on retire les fonctionnalités de confort. Focus sur le cœur métier. Le reste vient après.

---

## Slide 8 — Ce qui se passe vraiment (Duo : Didier raconte, Laure réagit) · ~3 min

**D** : [Ton honnête, presque confessionnel.]

Maintenant, la réalité.

On démarre en mob à trois développeurs back. Pendant un mois et demi, c'est intense : transfert craft, découverte fonctionnelle, tout le monde apprend en même temps.

Puis on passe en pair — un mois et demi aussi. Le TDD tient, la review sert surtout à ancrer les pratiques.

Ensuite, phase hybride. Un mois. Absences alternées — tantôt moi, tantôt le dev expérimenté. On jongle. Une dev expérimentée Alptis rejoint l'équipe et suit le TDD sur les modules intégrés.

Et puis… les deux derniers mois. Je ne suis plus là. Le dev senior est seul sur certains modules, sous pression de deadline. Il n'est pas assez à l'aise pour pratiquer le TDD en autonomie.

Résultat : certaines zones sont livrées sans TDD.

**→ L** : [Complète, ton lucide.]

Côté orga, on a aussi absorbé trois semaines de friction — de la standardisation produit, pas de la complexité technique. Des contraintes qu'on n'avait pas anticipées.

**→ D** : Et côté front : un seul dev, le tech lead. Je lui ai montré la démarche en pair. Il a été conquis. Il l'a adoptée en autonomie sur tout le projet.

[Pause. Le public craft reconnaît cette réalité. C'est ici qu'on gagne leur confiance.]

---

## Slide 9 — 7 mois : résultat contrasté (Didier) · ~3 min

**D** : [Marquer le chiffre. Ton direct.]

Sept mois.

[Pause.]

Dont un mois de retard sur la mise en marché.

[Laisser le chiffre peser. Le public fait le calcul : autant qu'avant.]

Mais regardons de plus près. Là où le craft a tenu — l'intention est garantie. Pas de régression. On sait exactement ce que fait le code.

Là où le craft a été lâché — les modules fonctionnent. Peu de bugs. Mais on a perdu la certitude. On est revenus à la dépendance recette pour valider ce qu'on ne sait plus garantir soi-même.

[Pause.]

On a mis sept mois. Avec une équipe qui n'avait jamais touché au contexte Alptis. Avec un mois de friction organisationnelle. Avec une double courbe d'apprentissage.

[Ton plus léger, sourire.]

Sept mois. Mais on desserre les fesses.

[Laisser la salle réagir.]

Pour aller plus vite, il faut d'abord apprendre à livrer sûr.

---

## Slide 10 — L'apprentissage (Didier) · ~1 min

**D** : [Ton apaisé, rythme lent. Respiration narrative.]

L'artisan a montré les techniques d'assemblage. Le tenon-mortaise. Les outils adaptés.

On a retenu les techniques. On essaye de se les approprier.

On n'est pas encore complètement à l'aise.

[Pause. Le public fait le parallèle avec ce qu'on vient de raconter.]

Mais quelque chose a changé.

[Change de slide.]

---

## Slide 11 — Le renversement : le métier vient à nous (Laure) · ~3 min

**L** : [Ton storytelling — elle raconte un moment précis.]

Un jour, on reçoit une invitation à une réunion. Objectif flou. On ne sait pas trop ce qu'on va y faire.

On arrive. Et on comprend.

Le métier — les actuaires, ceux qui conçoivent les produits — nous demande **comment** concevoir le prochain produit pour minimiser le temps de réalisation.

[Pause. Laisser l'inversion s'installer.]

On leur dit : « Si vous faites x, ça ira vite. Si vous faites y, il nous faudra plus de temps. On préconise x. »

Leur réponse : « OK pour x. »

[Pause.]

Ce renversement n'est pas tombé du ciel. Il a fallu des années pour construire cette confiance. Des années de collaboration, d'agile, de preuves accumulées.

Mais c'est ce moment-là qui rend la suite possible. Le craft seul ne suffit pas — il faut que l'organisation bouge aussi.

---

## Slide 12 — Santé Équilibre : 2 mois + 1 mois (Didier) · ~3 min

**D** : [Ton affirmé. Le moment de la preuve.]

Nouveau produit : Santé Équilibre. On duplique SFR comme base. On part avec les tests — la capture de l'intention — et la structure du code. Les acquis de l'acte 2.

Nouveau levier : on découple vis-à-vis des services externes. Contrats d'interface définis en amont, simulation par configuration. On peut avancer sans attendre la disponibilité des autres équipes.

[Marquer le chiffre.]

Deux mois. Une version quasi complète en prod. Recette comprise. Avec un périmètre fonctionnel plus complet que SFR à sa mise en marché.

[Pause.]

Plus un mois — pour les branchements avec les services externes et les spécificités Santé Équilibre.

Et en recette ? Quasi aucun retour. Les retours hérités du produit 1 sont déjà absorbés.

[Ton posé, conclusif.]

Pendant deux mois, c'est la recette qui est le goulot. Puis un mois pour les services externes. Le développement n'est le goulot à aucun moment.

Le goulot s'est déplacé : du développement vers la recette et les dépendances externes.

Quand le changement devient maîtrisé, l'industrialisation devient rationnelle.

---

## Slide 13 — Le déclic du template + projection (Laure) · ~3 min

**L** : [Ton tourné vers l'avenir.]

À ce stade, on a un produit en prod, testé, recetté. Une base solide. Et la question vient naturellement : pourquoi ne pas en faire un template ?

C'est ce qu'on fait. Le template devient un produit vivant. Recetté de bout en bout. Toujours à jour. Les corrections sont portées sur le produit concerné **et** sur le template. Les fonctionnalités communes y sont intégrées. Chaque nouveau produit part de cette base — et les déclinaisons se concentrent sur ce qui est spécifique.

[Pause.]

En 2026, l'objectif DSI est acté au budget : un parcours de vente en 150 jours. Le budget alloué est de 200 jours.

[Ton personnel, engagé.]

Et l'histoire ne s'arrête pas au départ de Didier. On a lancé des formations TDD pour les développeurs qui n'étaient pas dans l'équipe expérimentale. Le TDD continue sur les produits déjà livrés, pour les évolutions et la maintenance.

L'organisation a internalisé.

---

## Slide 14 — L'atelier transformé + punchline (Duo) · ~2 min

**D** : [Retour au ton de la slide 1. Calme, posé.]

L'atelier n'est plus le même.

On sait comment faire une chaise qui tient debout.

**→ L** : [Enchaîne, même ton.]

On se concentre maintenant sur la personnalisation de la chaise — vis-à-vis de la demande du client.

[Silence. 3-4 secondes. Le public boucle sur l'image de l'ouverture.]

**→ D** : [Regarde la salle. Ton affirmé, pas agressif.]

Développer est un métier.

[Pause. 2 secondes.]

Être artisan développeur en est un autre.

[Silence long — 4-5 secondes. Ne rien ajouter. Laisser la phrase résonner.]

**→ L** : Merci.

[Slide de remerciement. Applaudissements.]

---

## Notes de mise en scène générales

### Transitions Didier ↔ Laure
- Les passages de parole se font **au regard**, pas à la voix. Celui qui va parler fait un demi-pas en avant ou se tourne vers la salle. Celui qui écoute recule légèrement ou se tourne vers l'autre.
- Sur les slides duo (2, 3, 6, 8, 14) : les deux sont actifs. Celui qui ne parle pas **réagit** (acquiescement, sourire, regard vers l'autre). Pas de statue.
- Répéter les transitions. C'est ce qui fait la différence entre un duo et deux monologues alternés.

### Rythme
- **Slides 1, 5, 10, 14** : rythme lent, silences marqués. Ce sont les moments d'émotion et d'analogie.
- **Slides 4, 7, 12** : rythme plus soutenu. Ce sont les slides de contenu factuel.
- **Slides 8, 9** : rythme moyen, ton d'honnêteté. Le public doit sentir qu'on ne triche pas.

### Gestion du temps
- Cible : 30-35 minutes de présentation.
- Si le temps presse : comprimer les slides 7 (leviers) et 8 (phases) — le public craft connaît ces pratiques.
- Ne jamais comprimer : slides 1, 5, 9, 11, 14 — ce sont les piliers émotionnels et narratifs.
