# Notes speaker par slide — REX Lyon Craft

> Livrable de l'étape 5.
> Aide-mémoire : ce qu'il faut dire à l'oral **en plus** de ce qui est affiché.
> **D** = Didier · **L** = Laure

---

## Slide 1 — Titre

- Pas de prise de parole, laisser la salle s'installer

## Slide 2 — L'atelier de Liza (D)

- Voici l'atelier de Liza, elle fabrique des chaises
- Une fois que Liza a fini sa chaise, elle teste et CRAC ! La chaise casse, il n'y a plus qu'à recommencer
- Cette histoire est une analogie de ce qui arrive sur de nombreux projets
- C'est ce qui arrivait chez Alptis et nous allons vous raconter comment le Craft a permis de faire évoluer les choses

## Slide 3 — La douleur et le déclic (L puis D)

- **L** : Le contexte de l'équipe : en pleine migration de java 11 vers java 21 sur plusieurs applications. La migration prend du temps et s'avère compliquée. Il y a beaucoup d'aller/retour au niveau de la recette car pas mal de régressions dans le code. Les bugs sont détectés tard dans le workflow. Cela est inconfortable pour l'équipe et fait perdre du temps.
- **D** : C'est dans ce contexte que j'arrive chez Alptis en tant que futur Tech Lead
- **D** : "Ils sont bien gentils chez Alptis, je n'ai clairement pas envie de revivre ça — il va falloir changer la façon de travailler"

## Slide 4 — Qui sommes-nous (D puis L)

- **D** : Bonjour à tous et merci pour votre présence, il est temps de faire les présentations. Je m'appelle Didier et je suis dans le développement logiciel depuis une quinzaine d'années. Ça fait 3 ans que le Craft me fascine et je vois chez Alptis une opportunité d'expérimenter ça grandeur nature.
- **L** : Moi c'est Laure, je suis dans la tech depuis plus de 20 ans. Et oui ça ne se voit pas ! J'ai commencé en tant que dev fullstack. Arrivée chez Alptis en 2013, avec l'expérience et de l'ambition, j'ai été Lead et je suis maintenant Engineering manager depuis 3 ans. J'accompagne actuellement 5 équipes à plein temps.
- « On va vous raconter comment l'atelier de Liza s'est transformé »

## Slide 5 — La norme (L)

- Effectivement, jusqu'à présent un produit était réalisé en 6 à 7 mois suivant les spécificités métiers avec une équipe de 4 à 5 personnes (1 PO, 1 QA et 3 devs front/back). 
- Cela s'est confirmé sur les 3 produits Santé Select, Santé Protect et Santé Pro +. Tous sont des produits dédiés à la santé individuelle. Cela fonctionne, les métiers sont contents, mais (car il y a toujours un mais quelque part) ils aimeraient sortir plus de produits et notre cadence actuelle ne le permet pas.

## Slide 6 — Formulation clé + question (D)

- Écho au craquement de la slide 2
- La question ouvre l'acte 2

## Slide 7 — Repartir de zéro avec le craft (L puis D)

- **L** : Cela faisait un moment qu'on parlait de craft avec Didier. J'en avais parlé au sein d'Alptis, nous parlions déjà DDD, mais peu ambitionnait le TDD. Pas toujours facile de s'y mettre quand personne ne le maitrise vraiment. Nouveau produit, nouvelle équipe, on décide d'expérimenter autre chose. C'est l'occasion de repartir sur des bases saines. Didier intègre cette nouvelle équipe et instaure le TDD.
- **D** : double pari craft + contexte métier. Pas un labo, un vrai produit avec une vraie date

## Slide 8 — Ce qu'on met en place (D)

- Donner le **pourquoi** de chaque levier, pas juste le quoi

## Slide 9 — L'apprentissage (D)

- Vignette 1 : le maître artisan montre les techniques
- Vignette 2 : l'apprentie essaye de se les approprier
- Vignette 3 : pas encore complètement à l'aise, mais quelque chose a changé

## Slide 10 — Ce qui se passe vraiment (D puis L)

- **D** : détailler les 4 phases, insister sur les 2 derniers mois (TDD lâché sous pression)
- **L** : Dans le lot, il y a eu ~3 semaines de friction organisationnelle comprenant des allers/retours avec l'architecte solutions afin de prendre en compte la standardisation du produit (qui avait été réfléchie en amont mais l'équipe n'était pas présente à ce moment là). La solution a donc été rechallengée avec la nouvelle équipe.
- **D** : côté front — 1 dev formé en pair, adopte le TDD en autonomie

## Slide 11 — 7 mois : résultat contrasté (D)

- Rappeler le contexte : équipe neuve, friction orga, double apprentissage → en conditions normales ~6 mois
- Thèse : « pour aller plus vite, il faut apprendre à livrer sûr »

## Slide 12 — Le métier vient à nous (L)

- Un peu avant la fin du produit Santé Frontaliers Suisses, le métier vient pour nous dire qu'ils veulent sortir un nouveau produit. Le challenge qu'il nous lance : Aller plus vite !
Pour cela, les personnes du métier ont compris qu'il va falloir qu'elles nous aident et qu'elles travaillent avec nous pour simplifier le nouveau produit.
Nous avions déjà beaucoup discuté avec eux sur les autres produits en leur faisant des propositions pour aller plus vite, mais le métier n'était pas vraiment prêts à les entendre à l'époque.
A force de rappel, finalement cela infuse ! Il est prêt à simplifier et travailler avec nous pour co-construire le prochain produit pour gagner du temps.

## Slide 12 bis — La décision (L)

- Suite aux différentes réunions avec le métier et plusieurs ateliers techniques derrière, le produit ressemble beaucoup à Santé Frontaliers Suisses qu'on finissait de développer en parallèle. Ce nouveau produit était même plus simple.
Nous décidons collégialement que le produit Santé Frontaliers Suisses (qui bénéficiait du TDD) était assez stable pour le dupliquer. Le TDD rendait plus facile le fait de l'adapter au métier du nouveau produit.
L'équipe était confiante que cela serait confortable pour tout le monde et nous faciliterait le développement.

## Slide 13 — Résultat : Santé Équilibre en 3 mois (D)

- Duplication SFR : tests + structure du code
- Nouveau levier : découplage services externes (contrats d'interface, mock/réel par config)
- En recette : quasi aucun retour
- Le dev n'est le goulot à aucun moment

## Slide 14 — Template + projection (L)

- Suite à cette réussite, une nouvelle idée survient et si on industrialisait pour ce type de produit !
Nous avons tout ce qu'il faut pour partir sur des bases solides. Les 2 derniers produits nous ont montré que cela était possible et que le gain de temps était réel, mais nous devons aller plus loin.
L'idée du template maintenable et évolutif est là ! Cela nous pose des questions au niveau de l'organisation des équipes. Nous revoyons un peu les choses et décidons de créer une nouvelle équipe socle qui serait en charge de ce genre de projet.
Le projet est remonté au niveau de la DSI afin de valider les changements d'organisation et un budget est décidé pour l'année suivante.
Aujourd'hui, l'équipe socle est montée et le template est en cours de réalisation. 200 jours ont été alloué dans le budget de la DSI pour soutenir notre projet.
Des formations sont en cours également pour propager le TDD dans les autres équipes.

## Slide 15 — L'atelier transformé + punchline (D puis L)

- Vignette 1 : l'atelier transformé, les chaises tiennent
- Vignette 2 : on se concentre sur la personnalisation
- Punchline après silence
- **L** : « Merci à tous de nous avoir écouté. A vos questions ! »
