# Notes speaker par slide — REX Lyon Craft

> Livrable de l'étape 5.
> Aide-mémoire : ce qu'il faut dire à l'oral **en plus** de ce qui est affiché.
> **D** = Didier · **L** = Laure

---

## Slide — Titre

- Bonjour, Merci de votre présence.
Nous vous faisons part d'un retour d'expérience à travers ce talk : "Et Craft ! La chaise".
Vous allez suivre avec nous, comment des pratiques Craft, ont permis chez Alptis,
De passer de l'optimisation à l'industrialisation.

## Slide — L'atelier de Liza (D)

- Et pour illustrer tout ça, nous vous proposons cette analogie avec l'atelier de Liza.
- Liza fabrique des chaises. Et jusqu'à présent.
- Une fois que Liza a fini sa chaise, elle teste et CRAC ! La chaise casse, il n'y a plus qu'à recommencer
- Cette histoire est une analogie de ce qui arrive sur de nombreux projets
- C'était un peu comme ça chez Alptis et nous allons vous raconter comment le Craft a permis de faire évoluer les choses, de transformer l'atelier de Liza.

## Slide — Qui sommes-nous (D puis L)

- **D** : Il est temps de faire les présentations.
Je m'appelle Didier et je suis dans le développement logiciel depuis une quinzaine d'années principalement en tant que tech lead Java. Et depuis 5 ans, je suis freelance.
Ça fait 3 ans que le Craft me fascine et je vois chez Alptis une vraie première opportunité d'expérimenter ces pratiques grandeur nature.
- **L** : Moi c'est Laure, je suis dans la tech depuis plus de 20 ans. Et oui ça ne se voit pas ! J'ai commencé en tant que dev fullstack. J'ai enchainé plusieurs entreprises avant d'arriver chez Alptis en 2013. Avec l'expérience acquise et de l'ambition, je suis passée Lead sur des plus ou moins grandes équipes. Et à présent, je suis Engineering manager depuis 3 ans. J'accompagne actuellement 5 équipes à plein temps.


## Slide — Quelques mots sur Alptis (L)

- Alptis Assurance est un courtier grossiste en assurance spécialisé dans la protection de la personne. Nous concevons et distribuons des solutions de santé, prévoyance, retraite et emprunteur, destinées aux particuliers, travailleurs indépendants et entreprises. 
Alptis s’appuie sur un modèle collaboratif avec des réseaux de courtiers pour distribuer ses offres.
Les courtiers se rendent sur l'extranet Alptis Connect afin d'avoir accès aux différents parcours de vente qui leur permettent de tarifer nos offres et de les proposer à leur client et enfin de souscrire.
- Didier faisait partie de l'équipe en charge des parcours de vente pour les offres de santé individuelles, pour faire simple, ce sont des complémentaires santé. Les clients cibles pour ces offres sont des particuliers et des travailleurs indépendants principalement.

- Maintenant que vous en savez plus sur nous, nous allons vous raconter comment l'atelier de Liza s'est transformé.

## Slide — La douleur et le déclic (L puis D)

- **L** : En décembre 2024, l'équipe était en pleine migration de java 11 vers java 21 sur plusieurs applications de son périmètre. La migration a pris du temps et s'est avérée compliquée. Il y avait des tests en place mais pas toujours pertinents. Cela ne permettait pas de constater les impacts réels de la migration. Les bugs ont été détectés tard dans le workflow, il y a eu beaucoup d'aller/retour au niveau de la recette car pas mal de régressions dans le code. Cela était inconfortable pour l'équipe et faisait perdre du temps.
- **D** : C'est dans ce contexte que j'arrive chez Alptis en tant que futur Tech Lead
J'ai donc vécu cette période de flou et d'incertitude empreinte de lassitude et de frustration. Et je sais qu'on peut faire mieux, avec le TDD notamment.
- **D** : Ils sont bien gentils chez Alptis (et c'est vrai !) mais je n'ai clairement pas envie de revivre ça — Je sais déjà que je vais proposer de revoir la façon de travailler. Ayant déjà expérimenté le TDD de manière isolée, je sais qu'on peut être plus à l'aise et plus sûr de nos livraisons.


## Slide — La norme (L)

- Alors quelle est la norme à ce moment-là ? 
Jusqu'à présent un produit était réalisé en 6 à 7 mois suivant les spécificités métiers, avec généralement une équipe de 4 à 5 personnes (1 PO, 1 QA et 2 à 3 devs front/back). 
Au niveau du rythme de livraisons sur un produit, on était à 1 livraisons en prod. 
Une finale pour la mise en marché de l'offre (généralement date définies avec le métier).

- le workflow des équipes est le suivant: d'abord la partie conception pour réfléchir dans l'équipe à la fonctionnalité (sous forme de User Story) aussi bien technique que fonctionnel. 
Ensuite le développement est réalisé, puis suis une première recette croisée technique (seulement les devs), cela leur permet de faire une première passe et de corriger plus rapidement entre eux. 
Une fois cette recette croisée réalisée et validée, la recette fonctionnelle par le/la PO et/ou le/la QA peut se faire. 
Suivait ensuite une démo faite au métier pour avoir différents feedback.
Bon en fait je vous ai un peu menti, on faisait bien plusieurs livraisons au métier mais seulement en environnement de recette. Le métier ne voulait pas que cela soit mis en prod tant que tout le périmètre cible n'était pas atteint.

- Nous avons pu constater ce temps de réalisation sur les 3 produits précédents Santé Select, Santé Protect et Santé Pro +. Tous sont des produits dédiés à la santé individuelle. 

Cela fonctionne. Les métiers sont contents. Le produit est satisfaisant à sa sortie. 

## Slide — Le constat (L)

- Quelque chose est récurrent, on constate qu'on repart à chaque fois de zéro, beaucoup de modules se ressemblent mais les règles métier sont spécifiques et demandent à revoir l'implémentation à chaque fois.

- Les étapes d'un parcours de vente restent souvent les mêmes. Certaines dont la partie choix des garanties et la tarification sont à réadapter pour chaque produit. Cela prend du temps et nous ne sortions que 2 produits sur le périmètre santé individuel par an.
 
- Cela n'est pas suffisant pour le métier. Ils aimeraient en sortir plus dans le but d'être plus concurrentiel sur le marché et d'avoir plus de choix à proposer aux courtiers.


## Slide — Formulation clé + question (D)

Pour le moment, la situation est la suivante : 
On veut produire plus vite,
mais on serre les fesses quand on s'assoit sur la chaise.

Et si le vrai problème n'était pas seulement la vitesse, mais surtout la façon dont on fabrique les chaises ?

## Slide — Repartir de zéro avec le craft (L puis D)

- **L** : Avant qu'il intègre notre pôle, je connaissais déjà Didier. Il avait fait une première mission chez Alptis mais dans un autre pôle et nous nous sommes recroisés plusieurs fois lors de conférences dont Lyon Craft. Nous avions échangé plusieurs fois sur les pratiques craft. J'en avais parlé au sein d'Alptis, nous parlions déjà DDD, mais peu ambitionnait le TDD. Pas toujours facile de s'y mettre quand personne ne le maitrise vraiment. Lors d'un remplacement de prestation, j'ai vu une opportunité d'intégrer quelqu'un qui pourrait m'aider à mettre en place des nouvelles pratiques dans nos équipes plus facilement. Didier était disponible et était motivé pour faire bouger les choses avec moi. Super opportunité pour nous !
Nous profitons alors d'un nouveau produit : Santé Frontaliers Suisses, 
Une nouvelle équipe est en place, nous décidons d'expérimenter autre chose.
C'est l'occasion de repartir sur des bases saines. Didier est dans cette nouvelle équipe et instaure le TDD.
- **D** : Et l'ambition est de taille. L'équipe ne manque pas d'expérience sur la stack technique. Java, VueJs, on maîtrise. Par contre, les parcours de vente de complémentaire santé, le TDD, l'environnement Alptis, ... C'est une autre histoire.
Il faut donc monter en compétence sur ces trois axes ... et faire plus vite !

## Slide — Ce qu'on met en place (D)

Je l'ai dit plus tôt, ils sont vraiment sympas chez Alptis à ce point que quand je propose d'expérimenter le TDD sur le nouveau produit, je suis soutenu, évidemment par Laure, mais surtout par le management du service et mon équipe pour tenter l'expérimentation de cette pratique malgré les enjeux forts sur ce nouveau produit. Et pas que ...

Voilà ce que nous décidons d'expérimenter pour développer ce Santé Frontaliers Suisses :
- Le TDD pour profiter de la conception émergente et la refactorisation continue. On espère ainsi réussir à améliorer le code, sa stabilité et sa maniabilité.
C'est une méthode de développement en un cycle itératif de 3 phases :
  - un test en échec
  - une implémentation bête, même crade pour valider le test
  - une refactorisation pour nettoyer et sculpter le code
- Le Mob programming, pour une montée en compétence plurielle, partagée et homogène dans l'équipe
Il s'agit d'une pratique qui consiste réunir plusieurs développeurs autour d'un même clavier pour développer une même fonctionnalité.
- Des user stories itératives pour construire le produit pas à pas comme si on était sur un tout nouveau produit. Nous avions la chance de pouvoir compter sur des personnes, dont notre PO, qui ont une très bonne connaissance du produit et du contexte Alptis et garantir l'efficacité de cette approche.
- Un périmètre allégé. En effet, notre PO réussit à négocier avec le métier pour réduire au strict minimum les fonctionnalités dites de confort et se cantonner à un produit qui se rapproche le plus possible d'un MVP. Un MVP ou minimal viable product est un produit avec le minimum de fonctionnalités possibles pour être exploité.
- Et enfin, une livraison continue pour réduire la charge mentale liée à la MEP. On a la possibilité technique de le faire sans que le produit ne soit accessible aux clients, on ne va pas se priver. Globalement, on livre toutes les semaines.

## Slide — L'apprentissage (D)

Revenons à Liza, il se trouve que dans son atelier aussi ça bouge.
Elle a fait appel à un maître artisan qui va tenter de lui apprendre à maîtriser, par exemple, la technique du tenon-mortaise. 
Elle doit prendre le temps pour l'acquérir, ce n'est pas forcément simple 
Mais une fois cette technique d'assemblage acquise, elle n'aura plus besoin de vérifier la solidité de ses chaises.
En tout cas, c'est l'idée.

## Slide — Ce qui se passe vraiment (D)

- Voyons comment ça avance chez Alptis ... Et bien, ce n'était pas un long fleuve tranquille. La physionomie de notre équipe côté backend a évolué dans le temps et nos pratiques aussi :

- D'abord, ~1,5 mois : on travaille en mob programming avec le précédent tech lead qui fait encore partie des effectifs => je coach la pratique du TDD, lui nous met au parfum sur les subtilités du produit et de l'environnement Alptis. On avance assez vite. Ça marche très bien, petit à petit le rythme se fluidifie. On est au top et confiant. Le workflow s'en trouve simplifié : plus de conception en amont, plus de revue de pr, plus de recette croisée, on fait tout en même temps pendant le développement.

Durant cette phase, j'insiste sur notions importante  :
  - le test first en baby step, qui aide à obtenir une conception taillée sur mesure. Baby step car à chaque étape, le nouveau test n'ajoute qu'une infime contrainte supplémentaire par rapport aux tests existants.
  - et l'aspect refacto en continu, cette 3eme phase du TDD à ne pas négligée et qui demande des bonnes compétences de design logiciel. C'est elle qui va assurer la maniabilité du code dans le temps.

- Ensuite, notre précédent tech lead nous lâche. On n'est plus que deux côté backend, Et bien forcément, on ne fait plus de mob, on essaye de faire du pair. 
C'est moins évident parce que c'est un exercice qui demande plus d'énergie dans cette configuration. Mais on ne lâche pas le TDD. Ça dure à peu près 2 mois. On est déjà moins efficace, des subtilités du métier et de l'environnement Alptis nous échappent. On commence à prendre du retard et à perdre confiance.

D'ailleurs, il y a quelques aller-retour en recette, mais il s'agissait surtout de subtilités sur le produit et l'environnement Alptis dont nous n'avions pas connaissance.

La reveu de code et la recette croisée refont surface. Pas la phase de conception en amont.

- S'ensuit une période hybride : mêlées aux congés, on a du renfort expérimenté. Elle est ouverte au TDD mais préfère travailler seule. Le délai met un peu de pression, on fait moins de pair, pas de mob, l'esprit du TDD n'est pas loin pas sûr qu'il soit correctement appliqué. En tout cas on teste et on fait de la refacto en continu. Pendant cette phase, nous n'arrivons pas à rattraper le retard.
- Et pour finir, c'est moi qui pars en congés (pendant 2 mois, rien que ça). Globalement, il ne reste plus qu'un développeur, il assure la MEP avec succès, mais, ne se sentant pas encore très à l'aise avec le TDD, il a repris sa méthode de travail habituelle, reprenant principalement ce qui a été fait sur les autres produits. Heureusement, on est sur des fonctionnalités très éprouvées et le manque de tests n'impacte pas la qualité.

- côté front, notez qu'en début de projet, j'ai fait une journée de pair programming avec notre dev front. Le but étant de lui faire comprendre l'essence de la méthode TDD. Mission réussie, il est conquis, il s'y emploie pendant toute la durée du projet.

## Slide — Comme si ça ne suffisait pas ... (L)
- **L** : Dans le lot, il y a eu ~3 semaines de friction organisationnelle comprenant des allers/retours avec l'architecte solutions afin de prendre en compte la standardisation du produit (qui avait été réfléchie en amont mais l'équipe n'était pas présente à ce moment-là). La solution a donc été rechallengée avec la nouvelle équipe.
Dans tous nos parcours, nous avons des dépendances avec des équipes externes. Notamment, pour ce qui concerne la gestion des documents contractuels, la tarification, la partie signature électronique et j'en passe... Et comme on dit souvent "Tout ce qui est dehors de l'équipe c'est le mal " ! Forcément, ces équipes ne travaillent pas de la même manière, n'ont pas toujours les mêmes workflows ou les mêmes contraintes. Cela demande de la coordination, des réunions de synchronisation et donc du temps.


## Slide — 7 mois : résultat contrasté (D)

Bilan : On a mis 7 mois, dont 1 mois de retard sur la date de livraison initiale, pour faire un nouveau produit épuré. Globalement c'est le même temps que sur les produits précédents. 
Est-ce qu'on a été moins rapide pour autant ? Pas si sûr. Pour rappel, nous avions :  
- une équipe inexpérimentée sur les pratiques Craft
- une équipe inexpérimentée sur les produits Alptis
- une équipe inexpérimentée sur le contexte Alptis
- de nouvelles exigences architecturales à intégrer

Ceci dit, étrangement, on a mis 7 mois à produire moins, mais on desserre les fesses.

Pourquoi ? 

D'une part parce qu'on est maintenant sûr de ce qu'on livre  grâce à une batterie de tests riche, pertinente et découplée des implémentations.

D'autre part, le code affiche une simplicité qui masque une certaine complexité. Grâce au TDD et son principe d'émergence de la conception et de refacto continue, certaines briques angoissantes sur les précédents produits ont gagné en simplicité si bien que ce ne sont plus des sujets de craintes.

A partir de là, on est assez serein sur le prochain produit à développer.

## Slide — Le métier vient à nous (L)

- Un peu avant la fin du produit Santé Frontaliers Suisses, le métier vient pour nous dire qu'ils veulent sortir un nouveau produit qui s'appellerait Santé Equilibre. Le challenge qu'il nous lance : Comment aller plus vite ?
  
Nous avions déjà beaucoup discuté avec eux sur les précédents produits en leur faisant des propositions plus agiles pour aller plus vite. Par exemple, ne sortir qu'une partie du parcours à présenter aux courtiers pour leur permettre de tester les tarifs d'une offre et qu'ils puissent souscrire, bon en mode papier, mais on est agile, ça aurait été une première version. Cela aurait permis de tester l'offre et de voir si les tarifs étaient compétitifs. Le métier, à ce moment-là n'était pas prêt à rogner sur les fonctionnalités. Nous leur avons donc présenté les choses différemment en leur disant que s'ils ne veulent pas rogner sur les fonctionnalités, il faudra beaucoup simplifier les règles métier.
Les personnes du métier ont compris qu'il allait falloir qu'elles nous aident et qu'elles travaillent avec nous pour simplifier le nouveau produit.
Si on revient sur notre analogie ça équivaut à leur faire remarquer que "Si toutes les chaises ont les mêmes pieds, ça ira plus vite !".
À force de rappel, finalement cela infuse ! Ils sont prêts à simplifier et travailler avec nous pour co-construire Santé Equilibre et gagner du temps.
Ils sont Ok pour avoir les mêmes pieds !


## Slide — La décision (L)

- Suite aux différentes réunions avec le métier et plusieurs ateliers techniques, nous constatons que le produit ressemble beaucoup à Santé Frontaliers Suisses qu'on finissait de développer en parallèle. Ce nouveau produit était même plus simple.
Le produit Santé Frontaliers Suisses bénéficiait du TDD, était stable, les bases étaient saines.
Si nous partons de là, il serait simple de faire les adaptations pour les nouvelles règles sur le prochain produit.
Nous décidons collégialement que le produit Santé Frontaliers Suisses sera dupliqué.
L'équipe était confiante, cela serait confortable pour tout le monde et nous faciliterait le développement.

## Slide — Santé Équilibre en 3 mois (D)

Résultat, Santé Équilibre est sorti au bout de 3 mois, à l'heure !
En 2 mois pour avoir un premier MVP quasi complet
- pendant les deux premières semaines, nous avions terminé la duplication et les adaptations.
- ce qui a pris du temps ? La recette. C'est elle le nouveau goulot d'étranglement. La stratégie adoptée, par prudence, a été de faire une recette comme si le produit avait été créé from scratch.
- très peu de retours, bien évidemment imputables également à Santé Frontaliers Suisses
- Et pour éviter d'attendre les livrables des autres équipes, nous avons pu mettre en place, très facilement, un système de simulation des services externes en attendant leur branchement

## Slide — Santé Équilibre en 3 mois (D)

Ensuite, le mois suivant a servi à : 
- implémenter un nouveau comportement spécifique
- implémenter les branchements avec les services externes
- mais également à implémenter quelques fonctionnalités de confort sur Santé Équilibre comme sur Santé Frontaliers Suisses

Mais alors ? l'industrialisation devient rationnelle !

## Slide — Le déclic du template (L)

- Suite à cette réussite, une nouvelle idée survient et si on industrialisait pour ce type de produit !
Nous avons tout ce qu'il faut pour partir sur des bases solides. Les 2 derniers produits nous ont montré que cela était possible et que le gain de temps était réel, mais nous devons aller plus loin.
L'idée du template maintenable et évolutif est là ! Un produit interne vivant, recetté et toujours à jour.

Cela nous pose des questions au niveau de l'organisation des équipes. Nous revoyons un peu les choses et décidons de créer une nouvelle équipe socle qui serait en charge de ce genre de projet.
Le projet est remonté au niveau de la DSI afin de valider les changements d'organisation et un budget est décidé pour l'année suivante. 200 jours ont été alloués dans le budget de la DSI pour soutenir notre projet. Le projet "produire un parcours de vente en 150 jours" est acté.

## Slide — Au-delà de la vitesse de production ? (D)

- Il y a un résultat non quantifiable de cette expérimentation et non négligeable pour autant.
- D'abord auprès des développeurs qui ont travaillé avec moi. Je peux dire que j'ai planté des graines qui commencent à germer. Aucun d'eux ne savait véritablement ce qu'est le Craft. Le TDD et le mob programming, ils avaient entendu les termes mais sans jamais s'y intéresser, se cantonnant aux idées reçues.
 - Depuis, l'un d'eux s'est vraiment plongé dans le monde du Craft en allant jusqu'à explorer les autres pratiques, se rendant compte du vaste monde derrière ce mot
- J'ai pu toucher également les développeurs d'autres équipes. Avant la fin de ma mission, je voulais trouver le moyen de faire perdurer ce que j'avais commencé à mettre en place. J'ai donc proposé un atelier avec d'autres développeurs que ceux de mon équipe sur le TDD en mob programming. J'ai eu d'excellents retours et tous (bon, ils n'étaient que 3 hein) se sont rendus compte de la pertinence de ces méthodes de développement et ont formulé le souhait de le mettre en pratique.
- Pour les autres (PO, managers, ...), je crois que malgré la confiance qu'ils me faisaient, ils n'étaient pas tous convaincus qu'on aurait pu vraiment faire mieux. Comme dit au début, le produits étaient déjà très satisfaisants. Et le premier projet n'a pas aidé en ce sens. Leur avis est différent aujourd'hui mais ils restent conscients que ces pratiques se travaillent et que les bénéfices n'arrivent pas du jour au lendemain. Le TDD n'est pas juste un buzzword.
- Et pour moi ? Cette expérience a été tellement enrichissante. Déjà parce qu'elle m'a assuré que je ne me trompais pas de direction.
- Ensuite parce que ça n'a pas été simple de s'adapter à tous les tempérament. Toutes les méthodes ne conviennent pas à tout le monde. 
- Et puis, j'étais loin d'imaginer l'ampleur de l'impact qu'elle aurait eu chez Alptis. Et j'en suis fier.
- Enfin, pour les puristes, je sais pertinemment qu'on a expérimenté qu'une micro partie du panel du monde du Craft. Ceci dit, d'abord je ne suis moi même pas un puriste, et surtout, je suis persuadé que l'infusion en douceur est le meilleur gage de réussite.

## Slide — Et aujourd'hui ... (L)

- Aujourd'hui, l'équipe socle est en place (1 PO, 2 devs front/back) et le template est en développement.
Des formations sont en cours pour propager le TDD dans les autres équipes du pôle.
Il existe plusieurs réflexions avec d'autres services au sein de la DSI afin de mettre en place cette notion de template plus largement notamment sur les documents contractuels.


## Slide — L'atelier transformé (D)

Et Liza ? Eh bien maintenant, elle est plus sereine.
Elle enchaîne les commandes et se concentre maintenant sur les besoins spécifiques de ses clients.
Elle peut se revendiquer artisane, Alptis également.

Par manque de temps, nous ne sommes pas rentrer dans certains détails : le détail de pratiques, comment je me suis adaptés aux affinités de chacun

## Slide — Merci (L)

« Merci à tous de nous avoir écoutés. Nous pouvons répondre à vos questions. »
