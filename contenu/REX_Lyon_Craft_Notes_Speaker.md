# Notes speaker par slide — REX Lyon Craft

> Livrable de l'étape 5.
> Aide-mémoire : ce qu'il faut dire à l'oral **en plus** de ce qui est affiché.
> **D** = Didier · **L** = Laure

---

## Slide 1 — Titre

- Bonjour, Merci de votre présence.
Nous vous faisons part d'un retour d'expérience à travers ce talk : "Et Craft ! La chaise".
Vous allez suivre avec nous, comment des pratiques Craft, ont permis chez Alptis,
Nous sommes passés de l'optimisation à l'industrialisation.

## Slide 2 — L'atelier de Liza (D)

- Et pour illustrer tout ça, nous vous proposons cette analogie avec l'atelier de Liza.
- Liza fabrique des chaises. Et jusqu'à présent.
- Une fois que Liza a fini sa chaise, elle teste et CRAC ! La chaise casse, il n'y a plus qu'à recommencer
- Cette histoire est une analogie de ce qui arrive sur de nombreux projets
- C'était un peu comme ça chez Alptis et nous allons vous raconter comment le Craft a permis de faire évoluer les choses, de transformer l'atelier de Liza.

## Slide 3 — Qui sommes-nous (D puis L)

- **D** : Bonjour à tous et merci pour votre présence, il est temps de faire les présentations.
Je m'appelle Didier et je suis dans le développement logiciel depuis une quinzaine d'années et tech lead Java depuis quelques années.
Ça fait 3 ans que le Craft me fascine et je vois chez Alptis une opportunité de l'expérimenter grandeur nature.
- **L** : Moi c'est Laure, je suis dans la tech depuis plus de 20 ans. Et oui ça ne se voit pas ! J'ai commencé en tant que dev fullstack. Arrivée chez Alptis en 2013, avec l'expérience et de l'ambition, j'ai été Lead et je suis maintenant Engineering manager depuis 3 ans. J'accompagne actuellement 5 équipes à plein temps.
- Nous allons vous raconter comment l'atelier de Liza s'est transformé.

## Slide 4 — La douleur et le déclic (L puis D)

- **L** : L'équipe était en pleine migration de java 11 vers java 21 sur plusieurs applications de son périmètre. La migration a pris du temps et s'est avéré compliquée. Il y avait des tests en place mais pas toujours pertinents. Cela ne permettait pas de constater les impacts réels de la migration. Les bugs sont détectés tard dans le workflow, il y a eu beaucoup d'aller/retour au niveau de la recette car pas mal de régressions dans le code. Cela était inconfortable pour l'équipe et faisait perdre du temps.
- **D** : C'est dans ce contexte que j'arrive chez Alptis en tant que futur Tech Lead
J'ai donc vécu cette période de flou et d'incertitude emprunte de lassitude et de frustration. Et je sais qu'on peut faire mieux.
- **D** : Ils sont bien gentils chez Alptis (et c'est vrai !) mais je n'ai clairement pas envie de revivre ça — il va falloir changer la façon de travailler.
Ayant déjà expérimenté le TDD, je sais qu'on peut être plus à l'aise

## Slide 5 — Quelques mots sur Alptis
- Alptis Assurance est un courtier grossiste en assurance spécialisé dans la protection de la personne. Nous concevons et distribuons des solutions de santé, prévoyance, retraite et emprunteur, destinées aux particuliers, travailleurs indépendants et entreprises. 
Alptis s’appuie sur un modèle collaboratif avec des réseaux de courtiers pour distribuer ses offres.
Les courtiers se rendent donc sur l'extranet Alptis Connect afin d'avoir accès aux différents parcours de vente qui leur permet de tarifer nos offres et de les proposer à leur client et de souscrire.
- Didier faisait partie de l'équipe en charge des parcours de vente pour les offres de santé individuelles, ce sont des complémentaires santé. Les clients cibles pour ces offres sont des particuliers et des travailleurs indépendants principalement.

## Slide 6 — La norme (L)

- Alors quelle est la norme à ce moment là ? 
Jusqu'à présent un produit était réalisé en 6 à 7 mois suivant les spécificités métiers avec une équipe de 4 à 5 personnes (1 PO, 1 QA et 3 devs front/back). 
- Nous avons pu le contstater sur les 3 produits précédents Santé Select, Santé Protect et Santé Pro +. Tous sont des produits dédiés à la santé individuelle. 
Cela fonctionne, les métiers sont contents, le produit est satisfaisant à sa sortie. Nous sortions 2 produits sur le périmètre santé individuel par an. Cela n'est pas suffisant pour le métier, ils aimeraient en sortir plus dans le but d'être plus concurrentiel et d'avoir plus d'offres à proposer aux courtiers.


## Slide 7 — Formulation clé + question (D)

Pour le moment, la situation est la suivante : 
On veut produire plus vite,
mais on serre les fesses quand on s'assoit sur la chaise.

Et si le vrai problème n'était pas la vitesse, mais la façon dont on fabrique les chaises ?

## Slide 8 — Repartir de zéro avec le craft (L puis D)

- **L** : Avant qu'il intègre notre pôle, je connaissais déjà Didier. Il avait fait une première mission chez Alptis mais dans un autre pôle et nous nous sommes recroisés plusieurs fois lors de conférences dont Lyon Craft. Nous avions échangé plusieurs fois sur les pratiques craft. J'en avais parlé au sein d'Alptis, nous parlions déjà DDD, mais peu ambitionnait le TDD. Pas toujours facile de s'y mettre quand personne ne le maitrise vraiment. Lors d'un remplacement de prestation, j'ai vu une opportunité d'intégré quelqu'un qui pourrait m'aider à mettre en place des pratiques dans nos équipes plus facilement. Didier était disponible et était motivé pour faire bouger les choses avec moi, super opportunité pour nous !
Nouveau produit : Santé Frontaliers Suisses, 
Nouvelle équipe, on décide d'expérimenter autre chose.
C'est l'occasion de repartir sur des bases saines. Didier intègre cette nouvelle équipe et instaure le TDD.
- **D** : Et l'ambition est de taille. L'équipe ne manque pas d'expérience sur la stack technique. Java, VueJs, on maîtrise. Par contre, les parcours santé individuel, le TDD, l'environnement Alptis, ... C'est une autre histoire.
Il faut donc monter en compétence sur ces trois axes.

## Slide 9 — Ce qu'on met en place (D)

Et voilà ce que nous décidons d'expérimenter :
- Le TDD pour la conception émergente et la refactorisation continue
- Le Mob programming, pour une montée en compétence plurielle et partagée (très efficace)
- Des US itératives pour construire le produit pas à pas sans anticipation
- Une livraison continue pour réduire la charge mentale liée à la MEP
- Un périmètre allégé, on négocie avec le métier pour réduire au strict minimum les fonctionnalités de confort et se cantonner à un MVP

## Slide 10 — L'apprentissage (D)

Revenons à Liza, il se trouve que dans son atelier aussi ça bouge.
Elle a fait appel à un maître artisan qui va tenter de lui apprendre à maîtriser, par exemple, la technique du tenon-mortaise. 
Elle doit prendre le temps pour l'acquérir. 
Mais une fois acquise, avec cette technique d'assemblage, elle n'aura plus besoin de vérifier la solidité de ses chaises.
En tout cas, c'est l'idée.

## Slide 11 — Ce qui se passe vraiment (D)

- **D** : Retour chez Alptis ... Ce n'était pas un long fleuve tranquille. La physionomie de l'équipe côté backend a évolué dans le temps et ses pratiques aussi :
- D'abord, ~1,5 mois : mob programming avec le précédent tech lead => je coach la pratique du TDD, il nous met au parfum sur les subtilités du produit et de l'environnement Alptis. On avance assez vite.
- Ensuite, il nous lâche. On n'est plus que deux côté backend, plus de mob, on essaye de faire du pair. C'est moins évident mais on ne lâche pas le TDD. Ça dure à peu près 2 mois. On est déjà moins efficace, Des subtilités du métier et de l'environnement Alptis nous échappent. On commence à prendre du retard.
- S'ensuit une période hybride : mêlées aux congés, on a du renfort mais qui aime bien travailler seul. Moins de pair, pas de mob, toujours du TDD (ou plutôt toujours des tests), mais moins maîtrisé. On n'arrive pas à rattraper le retard.
- Et pour finir, c'est moi qui pars en congés (pendant 2 mois, rien que ça). Globalement, il ne reste plus qu'un développeur, il assure la MEP avec succès, mais, ne se sentant pas encore très à l'aise avec le TDD, il a repris sa méthode de travail habituelle.
- **D** : côté front, notez qu'en début de projet, j'ai fait une journée de pair programming avec notre dev front. Le but étant de lui faire comprendre l'essence de la méthode TDD. Mission réussie, il est conquis, il s'y emploie pendant toute la durée du projet.

## Slide 12 — Comme si ça ne suffisait pas ... (L)
- **L** : Dans le lot, il y a eu ~3 semaines de friction organisationnelle comprenant des allers/retours avec l'architecte solutions afin de prendre en compte la standardisation du produit (qui avait été réfléchie en amont mais l'équipe n'était pas présente à ce moment-là). La solution a donc été rechallengée avec la nouvelle équipe.
Dans tous nos parcours, nous avons de dépendances avec des services externes. Notamment, pour ce qui concerne la gestion des documents contractuels, la tarification, la partie signature électronique et j'en passe... Et comme on dit souvent "Tout ce qui est dehors de l'équipe c'est le mal " ! Forcément, ces équipes ne travaillent pas de la même manière, n'ont pas toujours les mêmes workflow ou les mêmes contraintes. Cela demande de la coordination, des réunions de synchronisation et donc du temps.


## Slide 13 — 7 mois : résultat contrasté (D)

Bilan : On a mis 7 mois pour faire un nouveau produit épuré. Globalement c'est le même temps que sur les produits précédents. 
Est-ce qu'on a été moins rapide pour autant ? Pas si sûr. Pour rappel, nous avions :
- une équipe inexpérimentée sur les pratiques Craft
- une équipe inexpérimentée sur les produits Alptis
- une équipe inexpérimentée sur le contexte Alptis
- de nouvelles exigences architecturales à intégrer

Et étrangement, on a mis 7 mois à produire moins, mais on desserre les fesses.

Pourquoi ? Parce qu'on est maintenant sûr de ce qu'on livre et le code affiche une simplicité qui masque une certaine complexité.

A partir de là, on est assez serein sur le prochain produit à développer.

## Slide 14 — Le métier vient à nous (L)

- Un peu avant la fin du produit Santé Frontaliers Suisses, le métier vient pour nous dire qu'ils veulent sortir un nouveau produit. Le challenge qu'il nous lance : Comment aller plus vite ?
Pour cela, les personnes du métier ont compris qu'il va falloir qu'elles nous aident et qu'elles travaillent avec nous pour simplifier le nouveau produit.
Nous avions déjà beaucoup discuté avec eux sur les autres produits en leur faisant des propositions plus agiles pour aller plus vite, mais le métier n'était pas vraiment prêt à les entendre à l'époque.
Si on revient sur notre analogie ça équivaut à leur faire remarquer que "Si toutes les chaises ont les mêmes pieds, ça ira plus vite !".
À force de rappel, finalement cela infuse ! Ils sont prêts à simplifier et travailler avec nous pour co-construire le prochain produit et gagner du temps.
Ils sont Ok pour avoir les mêmes pieds !


## Slide 15 — La décision (L)

- Suite aux différentes réunions avec le métier et plusieurs ateliers techniques, le produit ressemble beaucoup à Santé Frontaliers Suisses qu'on finissait de développer en parallèle. Ce nouveau produit était même plus simple.
Le produit Santé Fronatliers Suisses bénéficiait du TDD, était stable, les bases étaient saines.
Si nous partons de là, il serait simple de faire les adaptations pour les nouvelles règles sur le prochain produit.
Nous décidons collégialement que le produit Santé Frontaliers Suisses sera dupliqué.
L'équipe était confiante que cela serait confortable pour tout le monde et nous faciliterait le développement.

## Slide 16 — Santé Équilibre en 3 mois (D)

Résultat, Santé Équilibre est sorti au bout de 3 mois.
2 mois pour avoir un premier MVP quasi complet
- En deux semaines, nous avions terminé
- ce qui a pris du temps ? La recette. C'est elle le nouveau goulot d'étranglement. La stratégie adoptée, par prudence, a été de faire une recette comme si le produit avait été créé from scratch.
- très peu de retours, bien évidemment imputables également à Santé Frontaliers Suisses
- Et pour éviter d'attendre les livrables des autres équipe, nous avons pu mettre en place, très facilement, un système de simulation des services externes en attendant leur branchement

1 mois pour 
- implémenter un nouveau comportement spécifique
- implémenter les branchements avec les services externes
- implémenter quelques fonctionnalités de confort

Mais alors ? l'industrialisation devient rationnelle !

## Slide 17 — Le déclic du template (L)

- Suite à cette réussite, une nouvelle idée survient et si on industrialisait pour ce type de produit !
Nous avons tout ce qu'il faut pour partir sur des bases solides. Les 2 derniers produits nous ont montré que cela était possible et que le gain de temps était réel, mais nous devons aller plus loin.
L'idée du template maintenable et évolutif est là ! Un produit interne vivant, recetté et toujours à jour.

Cela nous pose des questions au niveau de l'organisation des équipes. Nous revoyons un peu les choses et décidons de créer une nouvelle équipe socle qui serait en charge de ce genre de projet.
Le projet est remonté au niveau de la DSI afin de valider les changements d'organisation et un budget est décidé pour l'année suivante. 200 jours ont été alloués dans le budget de la DSI pour soutenir notre projet. Le projet "produire un parcours de vente en 150 jours" est acté.

Aujourd'hui, l'équipe socle est montée et le template est en cours de réalisation.
Des réflexions sont en cours avec d'autres services au sein de la DSI afin de mettre en place cette notion de template plus largement notamment sur les documents contractuels.
Des formations sont en cours également pour propager le TDD dans les autres équipes.

## Slide 18 — L'atelier transformé (D)

Et Liza ? Eh bien maintenant, elle est plus sereine.
Elle enchaîne les commandes et se concentre maintenant sur les besoins spécifiques de ses clients.
Elle peut se revendiquer artisane, Alptis également.

## Slide 19 — Merci (L)

« Merci à tous de nous avoir écoutés. À vos questions ! »
