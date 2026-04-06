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
- **D** : Et l'ambition est de taille. L'équipe ne manque pas d'expérience technique. Java, VueJs, on maîtrise. Par contre, les parcours santé individuel, le TDD, l'environnement Alptis, ... C'est un autre histoire.
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
- D'abord, ~1,5 mois : mod programmning avec le précédent tech lead => je coach la pratique du TDD, il nous mets au parfum sur les subtilité du produit et de l'environnement Alptis. On avance assez vite.
- Ensuite, il nous lâche. On n'est plus que deux côté backend, plus de mob, on essaye de faire du pair. c'est moins évident mais on ne lâche pas le TDD
- S'en suit une période hybride : période de congés, on a du renfort mais qui aime bien travailler seul. On a pris de retard. Moins de pair, pas de mob, toujours du TDD (ou plutôt toujours des tests), mais moins maîtrisé.
- Et pour finir, c'est moi qui part en congés (pendant 2 mois, rien que ça), globalement, il ne reste plus qu'un développeur, il fait ce qu'il peut, du bon travaille mais ne se sentant pas encore très à l'aise avec le TDD, il reprend ses pratique précédentes et assure la MEP avec succès.
- **L** : Dans le lot, il y a eu ~3 semaines de friction organisationnelle comprenant des allers/retours avec l'architecte solutions afin de prendre en compte la standardisation du produit (qui avait été réfléchie en amont mais l'équipe n'était pas présente à ce moment là). La solution a donc été rechallengée avec la nouvelle équipe.
- **D** : côté front, j'ai fait une journée de pair programming avec notre dev front. Le but étant de lui faire comprendre l'essence de la méthode TDD. Mission réussi, il est conquis, il s'y emploi pendant toute la durée du projet.

## Slide 11 — 7 mois : résultat contrasté (D)

- Rappeler le contexte : équipe neuve, friction orga, double apprentissage → en conditions normales ~6 mois
- Thèse : « pour aller plus vite, il faut apprendre à livrer sûr »

## Slide 12 — Le métier vient à nous (L)

- On doit sortir un nouveau produit, le métier demande comment minimiser le temps de réalisation
- « Si la chaise a les mêmes pieds, ça ira vite. Sinon, plus long — on préconise les mêmes pieds. » → « OK pour les mêmes pieds. »
- Décision technique de dupliquer SFR
- Ce renversement a pris des années — le craft seul ne suffit pas

## Slide 13 — Résultat : Santé Équilibre en 3 mois (D)

- Duplication SFR : tests + structure du code
- Nouveau levier : découplage services externes (contrats d'interface, mock/réel par config)
- En recette : quasi aucun retour
- Le dev n'est le goulot à aucun moment

## Slide 14 — Template + projection (L)

- Template vivant, recetté, corrections sur produit ET template
- Formation TDD en cours hors équipe expérimentale
- L'organisation a internalisé

## Slide 15 — L'atelier transformé + punchline (D puis L)

- Vignette 1 : l'atelier transformé, les chaises tiennent
- Vignette 2 : on se concentre sur la personnalisation
- Punchline après silence
- **L** : « Merci »
