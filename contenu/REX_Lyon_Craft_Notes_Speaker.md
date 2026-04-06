# Notes speaker par slide — REX Lyon Craft

> Livrable de l'étape 5.
> Aide-mémoire : ce qu'il faut dire à l'oral **en plus** de ce qui est affiché.
> **D** = Didier · **L** = Laure

---

## Slide 1 — Titre

- Bonjour, Merci de votre présence pour ce retour d'expérience "Et Craft ! La chaise".

## Slide 2 — L'atelier de Liza (D)

- Voici l'atelier de Liza, elle fabrique des chaises
- Une fois que Liza a fini sa chaise, elle teste et CRAC ! La chaise casse, il n'y a plus qu'à recommencer
- Cette histoire est une analogie de ce qui arrive sur de nombreux projets
- C'est ce qui arrivait chez Alptis et nous allons vous raconter comment le Craft a permis de faire évoluer les choses, de transformer l'atelier de Liza.

## Slide 3 — La douleur et le déclic (L puis D)

- **L** : Le contexte de l'équipe : en pleine migration de java 11 vers java 21 sur plusieurs applications. La migration prend du temps et s'avère compliquée. Il y a beaucoup d'aller/retour au niveau de la recette car pas mal de régressions dans le code. Les bugs sont détectés tard dans le workflow. Cela est inconfortable pour l'équipe et fait perdre du temps.
- **D** : C'est dans ce contexte que j'arrive chez Alptis en tant que futur Tech Lead
- **D** : Ils sont bien gentils chez Alptis (et c'est vrai !) mais je n'ai clairement pas envie de revivre ça — il va falloir changer la façon de travailler. Ils veulent produire plus vite, sans filet, vouloir accélérer reste un pari.

## Slide 4 — Qui sommes-nous (D puis L)

- **D** : Bonjour à tous et merci pour votre présence, il est temps de faire les présentations. Je m'appelle Didier et je suis dans le développement logiciel depuis une quinzaine d'années. Ça fait 3 ans que le Craft me fascine et je vois chez Alptis une opportunité d'expérimenter ça grandeur nature.
- **L** : Moi c'est Laure, je suis dans la tech depuis plus de 20 ans. Et oui ça ne se voit pas ! J'ai commencé en tant que dev fullstack. Arrivée chez Alptis en 2013, avec l'expérience et de l'ambition, j'ai été Lead et je suis maintenant Engineering manager depuis 3 ans. J'accompagne actuellement 5 équipes à plein temps.
- Nous allons vous raconter comment l'atelier de Liza s'est transformé.

## Slide 5 — La norme (L)

- Effectivement, jusqu'à présent un produit était réalisé en 6 à 7 mois suivant les spécificités métiers avec une équipe de 4 à 5 personnes (1 PO, 1 QA et 3 devs front/back). 
- Cela s'est confirmé sur les 3 produits Santé Select, Santé Protect et Santé Pro +. Tous sont des produits dédiés à la santé individuelle. Cela fonctionne, les métiers sont contents, mais (car il y a toujours un mais quelque part) ils aimeraient sortir plus de produits et notre cadence actuelle ne le permet pas.

## Slide 6 — Formulation clé + question (D)

Pour le moment, la situation est la suivante : 
On veut produire plus vite,
mais on serre les fesses quand on s'assoit sur la chaise.

Et si le vrai problème n'était pas la vitesse, mais la façon dont on fabrique ?

## Slide 7 — Repartir de zéro avec le craft (L puis D)

- **L** : Cela faisait un moment qu'on parlait de craft avec Didier. J'en avais parlé au sein d'Alptis, nous parlions déjà DDD, mais peu ambitionnait le TDD. Pas toujours facile de s'y mettre quand personne ne le maitrise vraiment. 
Nouveau produit, 
nouvelle équipe, on décide d'expérimenter autre chose.
C'est l'occasion de repartir sur des bases saines. Didier intègre cette nouvelle équipe et instaure le TDD.
- **D** : Et l'ambition est de taille. L'équipe ne manque pas d'expérience technique. Java, VueJs, on maîtrise. Par contre, les parcours santé individuel, le TDD, l'environnement Alptis, ... C'est une autre histoire.
Il faut donc monter en compétence sur ces trois axes.

## Slide 8 — Ce qu'on met en place (D)

On va quand même un peu plus loin : 
- Le TDD pour la conception émergente et la refactorisation continue
- Le Mob programming, pour une montée en compétence plurielle et partagée (très efficace)
- Des US itératives pour construire le produit pas à pas sans anticipation
- Une livraison continue pour réduire la charge mentale liée à la MEP
- Un périmètre allégé, on négocie avec le métier pour réduire au strict minimum les fonctionnalités de confort et se cantonner à un MVP

## Slide 9 — L'apprentissage (D)

Revenons à Liza, il se trouve que dans son atelier aussi ça bouge.
Elle a fait appel à un maître artisan qui lui apprend à maîtriser la technique du tenon-mortaise. Elle doit prendre le temps pour l'acquérir. Mais une fois acquise, elle n'aura plus besoin de vérifier la solidité de ses chaises.

## Slide 10 — Ce qui se passe vraiment (D puis L)

- **D** : Revenons chez Alptis ... Ce n'était pas un long fleuve tranquille. La physionomie de l'équipe côté backend a évolué dans le temps et ses pratiques aussi :
- D'abord, ~1,5 mois : mob programming avec le précédent tech lead => je coach la pratique du TDD, il nous met au parfum sur les subtilités du produit et de l'environnement Alptis. On avance assez vite.
- Ensuite, il nous lâche. On n'est plus que deux côté backend, plus de mob, on essaye de faire du pair. C'est moins évident mais on ne lâche pas le TDD. Ça dure à peu près 2 mois. On est déjà moins efficace, Des subtilités du métier et de l'environnement Alptis nous échappent. On commence à prendre du retard.
- S'ensuit une période hybride : mêlées aux congés, on a du renfort mais qui aime bien travailler seul. Moins de pair, pas de mob, toujours du TDD (ou plutôt toujours des tests), mais moins maîtrisé. On n'arrive pas à rattraper le retard.
- Et pour finir, c'est moi qui pars en congés (pendant 2 mois, rien que ça). Globalement, il ne reste plus qu'un développeur, il fait ce qu'il peut, du bon travail mais ne se sentant pas encore très à l'aise avec le TDD, il reprend ses pratiques précédentes et assure la MEP avec succès.
- **L** : Dans le lot, il y a eu ~3 semaines de friction organisationnelle comprenant des allers/retours avec l'architecte solutions afin de prendre en compte la standardisation du produit (qui avait été réfléchie en amont mais l'équipe n'était pas présente à ce moment-là). La solution a donc été rechallengée avec la nouvelle équipe.
- **D** : côté front, j'ai fait une journée de pair programming avec notre dev front en début de projet. Le but étant de lui faire comprendre l'essence de la méthode TDD. Mission réussie, il est conquis, il s'y emploie pendant toute la durée du projet.

## Slide 11 — 7 mois : résultat contrasté (D)

Bilan : On a mis 7 mois pour faire un nouveau produit épuré. Globalement c'est le même temps que sur les produits précédents. Est-ce qu'on a été moins rapide pour autant ? Pas si sûr. Pour rappel :
- équipe inexpérimentée sur les pratiques Craft
- équipe inexpérimentée sur les produits Alptis
- équipe inexpérimentée sur le contexte Alptis
- de nouvelles exigences architecturales à intégrer

Mais étrangement, on a mis 7 mois, mais on desserre les fesses.

Pourquoi ? Parce qu'on est maintenant sûr de ce qu'on livre et le code est conçu sur mesure masquant une certaine complexité derrière sa simplicité.

À partir de là on a le sentiment que les prochaines fois seront bien.

## Slide 12 — Le métier vient à nous (L)

- Un peu avant la fin du produit Santé Frontaliers Suisses, le métier vient pour nous dire qu'ils veulent sortir un nouveau produit. Le challenge qu'il nous lance : aller plus vite !
Pour cela, les personnes du métier ont compris qu'il va falloir qu'elles nous aident et qu'elles travaillent avec nous pour simplifier le nouveau produit.
Nous avions déjà beaucoup discuté avec eux sur les autres produits en leur faisant des propositions pour aller plus vite, mais le métier n'était pas vraiment prêt à les entendre à l'époque.
À force de rappel, finalement cela infuse ! Il est prêt à simplifier et travailler avec nous pour co-construire le prochain produit et gagner du temps.

## Slide 13 — La décision (L)

- Suite aux différentes réunions avec le métier et plusieurs ateliers techniques derrière, le produit ressemble beaucoup à Santé Frontaliers Suisses qu'on finissait de développer en parallèle. Ce nouveau produit était même plus simple.
Nous décidons collégialement que le produit Santé Frontaliers Suisses (qui bénéficiait du TDD) était assez stable pour le dupliquer. Le TDD rendait plus facile le fait de l'adapter au métier du nouveau produit.
L'équipe était confiante que cela serait confortable pour tout le monde et nous faciliterait le développement.

## Slide 14 — Santé Équilibre en 3 mois (D)

Résultat, Santé Équilibre est sorti au bout de 3 mois.
2 mois pour avoir un premier MVP quasi complet
- duplication et adaptations réalisées en deux semaines
- ce qui a pris du temps ? La recette. La stratégie a été de faire une recette comme si le produit avait été créé from scratch par mesure de sécurité.
- très peu de retours, bien évidemment imputables également à Santé Frontaliers Suisses
- Pour permettre à la recette d'avancer au plus loin, nous avons pu créer un mécanisme pour simuler le comportement des services externes en attendant leur branchement via les fichiers de configuration

1 mois pour 
- implémenter un nouveau comportement spécifique
- implémenter les branchements avec les services externes
- implémenter quelques fonctionnalités de confort

Mais alors, l'industrialisation devient rationnelle !

## Slide 15 — Template + projection (L)

- Suite à cette réussite, une nouvelle idée survient et si on industrialisait pour ce type de produit !
Nous avons tout ce qu'il faut pour partir sur des bases solides. Les 2 derniers produits nous ont montré que cela était possible et que le gain de temps était réel, mais nous devons aller plus loin.
L'idée du template maintenable et évolutif est là ! Cela nous pose des questions au niveau de l'organisation des équipes. Nous revoyons un peu les choses et décidons de créer une nouvelle équipe socle qui serait en charge de ce genre de projet.
Le projet est remonté au niveau de la DSI afin de valider les changements d'organisation et un budget est décidé pour l'année suivante.
Aujourd'hui, l'équipe socle est montée et le template est en cours de réalisation. 200 jours ont été alloués dans le budget de la DSI pour soutenir notre projet.
Des réflexions sont en cours avec d'autres services au sein de la DSI afin de mettre en place cette notion de template plus largement notamment sur les documents contractuels.
Des formations sont en cours également pour propager le TDD dans les autres équipes.

## Slide 16 — L'atelier transformé (D)

Et Liza ? Eh bien maintenant, elle est plus sereine.
Elle enchaîne les commandes et se concentre maintenant sur les besoins spécifiques de ses clients.
Elle peut se revendiquer artisane, Alptis également.

Être artisan développeur, c'est une autre conception du métier.

- **L** : « Merci à tous de nous avoir écoutés. À vos questions ! »

## Slide 17 — Merci (L)

« Merci à tous de nous avoir écoutés. À vos questions ! »
