---
title: "Et Craft la chaise !"
theme: white
css: assets/custom.css
revealOptions:
  transition: slide
  slideNumber: false
  hash: true
---

<!-- .slide: class="slide-accent" -->

# Et Craft ! la chaise.

### De l'optimisation à l'industrialisation

**REX** ![Logo Alptis](assets/logo-alptis-color.svg) <!-- .element: style="width: 200px; vertical-align: middle; margin-bottom: 0.9em;" -->

**Didier ERIN** · **Laure CHAMPEL** 

Lyon Craft 2026

---

## L'atelier de Liza

![BD — Ça craque](assets/1_ca_craque.png) <!-- .element: style="max-height: 65vh;" -->

Note:
- illustrer ce talk
- Analogie
- nombreux projets informatique
- c'était comme ça chez Alptis

---

## Qui sommes-nous

<div class="speaker-row">
  <div class="speaker-card">
    <img src="assets/Didier.jpg" alt="Didier ERIN"/>
    <p><strong>Didier ERIN</strong><br/>Tech lead java<br/>Piqué par le Craft depuis 3 ans</p>
  </div>
  <div class="speaker-card">
    <img src="assets/Laure.jpg" alt="Laure CHAMPEL"/>
    <p><strong>Laure CHAMPEL</strong><br/>Engineering manager<br/>L'ancrage dans l'organisation de l'atelier</p>
  </div>
</div>

Note:
- **D** :
  - 15zaine d'année .. tech lead java .. 5 ans freelance 
  - 3 ans craft
  - opportunité
- **L** : 
  - 20 ans de tech, dev fullstack → 
  - Engineering manager, accompagne 5 équipes

---
## Quelques mots sur

![Logo Alptis](assets/logo-alptis-color.svg) <!-- .element: style="width: 200px; vertical-align: middle; margin-bottom: 0.9em;" -->

Courtier grossiste en assurance <!-- .element: class="fragment" -->

Parcours de vente <!-- .element: class="fragment" -->

Santé individuelle (complémentaire santé) <!-- .element: class="fragment" -->

Note:
- **L** 
  - Courtier grossiste assurance, santé, prévoyance, retraite, emprunteur 
  - Modèle collaboratif réseau courtiers → extranet → parcours de vente → souscription
  - Didier était équipe parcours de vente santé individuelle
  - clients cibles particulier, independant

---

*Comment l'atelier de Liza s'est transformé ?*

Note:
**L** — Nous allons vous racontez

---

## La douleur et le déclic

- Contexte : Migration Java 11 → 21 <!-- .element: class="fragment" -->
- Absence d'une batterie de test pertinente <!-- .element: class="fragment" -->
- Bugs et régressions détectés tardivement <!-- .element: class="fragment" -->
- Allers-retours dev ↔ recette <!-- .element: class="fragment" -->

Note:
- **L** 
  - décembre 2024, migration Java 11→21, compliquée, 
  - tests non pertinents, 
  - régressions tardives, 
  - allers-retours en recette
- **D** 
  - arrivé dans ce contexte
  - futur tech lead
  - période vécu : flou et d'incertitude empreinte de lassitude et de frustration

---

*Il faut que ça change !*

Note:
**D**
  - gentils chez Alptis
  - pas envie de revivre ça
  - TDD expérimenté de manière isolé
  - je me prépare à proposer de changer la façon de travailler
  - il faut que ça change

---

## La norme

<div class="norme-grid">
  <div class="norme-card">
    <span class="norme-chiffre">6–7</span>
    <span class="norme-unite">mois / produit</span>
  </div>
  <div class="norme-card">
    <span class="norme-chiffre">4–5</span>
    <span class="norme-unite">personnes</span>
    <span class="norme-detail">PO · QA · 2–3 devs</span>
  </div>
  <div class="norme-card">
    <span class="norme-chiffre">1</span>
    <span class="norme-unite">livraison en prod</span>
    <span class="norme-detail">Mise en marché</span>
  </div>
</div>

<div class="norme-workflow fragment">
<div><strong>Le workflow</strong></div>
  conception &nbsp;→&nbsp; dev &nbsp;→&nbsp; recette technique &nbsp;→&nbsp; recette fonctionnelle &nbsp;→&nbsp; démo métier
</div>

*Santé Select · Santé Protect · Santé Pro +* <!-- .element: class="fragment" style="font-size:0.7em; color: var(--text-muted);" -->

**C'est la norme. Le produit est satisfaisant.** <!-- .element: class="fragment" -->

Note:
- **L** : 1 PO, 1 QA, 2 à 3 devs, mep finale pour la mise en marché de l'offre (date définies avec le métier)
- Workflow : inspiration kanban, décrire les étapes, menti plusieurs livraisons en recette, métier -> pas de livraison prod sans tout le périmètre
- 6 à 7 mois temps contatés sur les 3 derniers produits
- Ça fonctionne, les métiers sont contents, le produit est satisfaisant

---
## Le constat

On repart chaque fois de zéro. <!-- .element: class="fragment" -->

Seulement 2 produits par an. <!-- .element: class="fragment" -->

**Mais souhait de produire plus.** <!-- .element: class="fragment" -->

Note:
**L** 
- On repart de zéro à chaque produit, 
- modules se ressemblent mais les règles métier sont spécifiques
- ré implémentation à chaque produit 
- -> Seulement 2 produits/an sur la santé individuelle
- pas suffisant pour le métier, 
- plus concurrentiel sur le marché, plus de choix pour les coutiers

---

<!-- .slide: class="slide-accent" -->

> *On veut produire plus vite, <br>
mais on serre les fesses quand on s'assoit sur la chaise.*

**Et si le vrai problème n'était pas la vitesse, mais la façon dont on fabrique les chaises ?** <!-- .element: class="fragment" -->

Note:
**D** 
- Pour le moment
- la situation est a suivante
- Et si 

---

## Repartir de zéro avec le craft

**Nouveau produit : Santé Frontaliers Suisses** <!-- .element: class="fragment" data-fragment-index="1" -->

Nouvelle équipe <!-- .element: class="fragment" data-fragment-index="2" -->

**Triple courbe d'apprentissage** <!-- .element: class="fragment" data-fragment-index="3" -->
* La santé individuelle <!-- .element: class="fragment" data-fragment-index="3" -->
* TDD <!-- .element: class="fragment" data-fragment-index="3" -->
* L'environnement Alptis <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
- **L** : connaissait Didier,mission Alptis, via Lyon Craft, DDD chez Alptis, non maitrise TDD, recruté pour faire bouger les pratiques, super oppourtunité !
- nouveau produit SFS, Nouvelle équipe → occasion de repartir sur des bases saines
- **D**
  - Ambition de taille
  - Stack tech -> on connait
  - montée en compétence 3 axes
  - il faut faire vite !

---

## Ce qu'on met en place

TDD (Test driven development) <!-- .element: class="fragment" -->

Mob programming <!-- .element: class="fragment" -->

User stories itératives <!-- .element: class="fragment" -->

Périmètre allégé <!-- .element: class="fragment" -->

Livraison continue <!-- .element: class="fragment" -->

Note:
**D** 
- plus tôt : vraiment gentils -> propose expérimenter TDD nouveau produit
- soutenu d'abord par Laure, management du service et mon équipe
- TDD : concept emergente / refacto continu / simplifacation / maniabilité
  - explications
- Mob programming : montée en compétence collective
  - explications
- US itératives 
- négociation PO / Métier : retrait fonctionnalité confort 
  - MVP : explications
- Livraison continue : charge mentale MEP

---

<!-- .slide: class="slide-accent" -->

## L'apprentissage

![BD — L'apprentissage](assets/2_l_apprentissage.png) <!-- .element: style="max-height: 65vh;" -->

Note:
**D**
- Liza fait appel à un maître artisan
- tenon mortaise
- ça prend du temps, long à acquérir
- mais une fois maîtrisé : plus besoin de vérifier la solidité

---

## Ce qui se passe vraiment

<div class="frise-vertical">
  <div class="frise-phase fragment">
    <span class="frise-label">Mob programming</span>
    <span class="frise-duree">~1,5 mois</span>
  </div>
  <div class="frise-phase fragment">
    <span class="frise-label">Pair & solo programming</span>
    <span class="frise-duree">~2 mois</span>
  </div>
  <div class="frise-phase fragment">
    <span class="frise-label">Renfort et congés programming</span>
    <span class="frise-duree">~1,5 mois</span>
  </div>
  <div class="frise-phase frise-phase--warning fragment">
    <span class="frise-label">Sans Didier programming</span>
    <span class="frise-duree">~2 mois</span>
  </div>
</div>

Note:
- aveu : pas un long fleuve tranquille
- physionomie de l'équipe côté back
- Mob ~1,5 mois : ancien TL présent
   - co-coaching / bon rythme confiant
   - workflow : pas de conception / pas de revue de code / pas de recette croisée
   - insiste sur 2 aspects TDD => baby step / refacto en continu
- Pair / solo : ancien TL nous lache
  - plus 2 / pas de mob / essaye pair mais ça demande plus d'énergie
  - moins efficace, retard commence, subtilités métier / Alptis
  - allers retours en recette à cause de la méconnaissance
  - Revue de code / recette croisée / on prend du retard / pr => 2 mois
- ~1,5 mois : périodes de congés, renfort expérimenté aime travaillé seule
  - pas de mob / TDD survit tant bien que mal / test / refacto
  - retart pas rattrapé / pressé par la deadline
- Sans Didier, 2 mois de congés, dev solo / succes de la MEP
  - pression de la deadline
  - pas à l'aise pour le TDD
  - retour aux habitudes, plus de TDD, plus de test / fonctionnalité éprouvée
- Dev front : convaincu dès le départ après une journée de pair, TDD tout le long

---

## Comme si ça ne suffisait pas ... 

Un besoin de standardisation mal exprimé à l'équipe <!-- .element: class="fragment" -->

Des dépendances avec des équipes externes <!-- .element: class="fragment" -->

Note:
- **L** ~3 semaines de friction : standardisation architecturale mal transmise, rechallengée avec la nouvelle équipe
- Dépendances extérieures : documents contractuels, tarification, signature électronique… "Tout ce qui est dehors de l'équipe c'est le mal" → chaque équipe a ses propres contraintes et workflow → coordination, réu synchro, temps

---

## 7 mois — résultat contrasté

dont 1 mois de retard <!-- .element: class="fragment" -->

avec une équipe <!-- .element: class="fragment" -->
* inexpérimentée sur les pratiques Craft  <!-- .element: class="fragment" -->
* inexpérimentée sur les produits Alptis  <!-- .element: class="fragment" -->
* inexpérimentée sur le contexte Alptis <!-- .element: class="fragment" -->
* de nouvelle exigences à intégrer <!-- .element: class="fragment" -->

Note:
**D**
- 7 mois ... dont 1 mois de retard
- pour faire un produit épuré
- c'est le même temps qu'avant pour faire moins
- Mois rapide pour autant ?
- Pour rappel

---

On a mis 7 mois

<blockquote class="fragment"><em>Mais on desserre les fesses.</em></blockquote>

On livre du code sûr, simplifié <!-- .element: class="fragment" -->

*On peut maintenant aller plus vite* <!-- .element: class="fragment" -->

Note:
**D** 
- On a mis 7 mois
- mais on desserre les fesses
- d'une part sûr de ce qu'on livre
- d'autre part, code affiche simplicité
- briques angoissantes -> plus un sujet de craintes.
- serein prochain produit
- on sait qu'on peut aller plus vite

---

## Le métier vient à nous

<div class="fragment">Nouveau produit à sortir : <em>Santé Equilibre</em></div>

**"Comment aller plus vite ?"** <!-- .element: class="fragment" -->

*"Si toutes les chaises ont les mêmes pieds, ça ira vite."* <!-- .element: class="fragment" -->

**"OK pour les mêmes pieds."** <!-- .element: class="fragment" -->

Note:
- **L** : avant la fin de SFS, métier vient pour SEQ → challenge "Comment aller plus vite"
- discussion sur les précédents produits, moins de fonctionnalités, mais livrer plus vite (seulement tarif pour tester l'offre)→ métier pas prêt 
- autre vision simplification règles métier: analogie → “si toutes les chaises ont les mêmes pieds” → métier prêt à simplifier et co-construire
- Cela infuse ! : ils sont OK pour des bases communes

---

## La décision

- Santé Equilibre très similaire <!-- .element: class="fragment" -->
- Code stable et testé <!-- .element: class="fragment" -->
- Base saine pour des adaptations rapides <!-- .element: class="fragment" -->

**Décision : dupliquer Santé Frontaliers Suisses** <!-- .element: class="fragment" -->

Note:
**L**
- réunions métiers et techniques → Santé Équilibre très similaire à SFS, même plus simple
- SFS bénéficie du TDD : code stable, base saine → adaptations faciles
- Décision collégiale : dupliquer SFS et adapter

---

## Santé Équilibre en 3 mois

2 mois : produit quasi complet <!-- .element: class="fragment" -->

→ La recette devient le goulot d'étranglement <!-- .element: class="fragment" -->

→ Des retours imputables à Santé Frontaliers Suisses <!-- .element: class="fragment" -->

→ simulation des services externes à la demande <!-- .element: class="fragment" -->

Note:
**D**
- Santé Equilibre est sorti au bout de 3 mois
- Et à l'heure !
- Concrètrement, 2 mois produit quasi complet
  - 2 semaines dupliquer adapter
  - La recette est le nouveau goulot : stratégie “from scratch” par prudence
  - Très peu de retours, et imputables SFS
  - Pour aider la recette périmètre
    - Simulation des services externes mise en place facilement grâce à la qualité du code

---

## Et pendant le mois de rab

→ nouveau comportement spécifique <!-- .element: class="fragment" -->

→ branchement avec les services externes <!-- .element: class="fragment" -->

→ quelques fonctionnalités de confort sur Santé Frontaliers Suisses et Santé Équilibre <!-- .element: class="fragment" -->

*Mais alors ? L'industrialisation devient rationnelle !* <!-- .element: class="fragment" -->

Note:
- implémenter nouveau comportement spécifique
- branchements services externes
- mais également
  - luxe fonctionnalités de confort 
    - Santé Équilibre
    - comme Santé Frontaliers Suisses

---

## Le déclic du template

Un produit interne vivant, recetté, toujours à jour. <!-- .element: class="fragment" -->

200 jours alloués à la création de ce template <!-- .element: class="fragment" --> 

Objectif DSI 2026 : produire un parcours de vente en <!-- .element: class="fragment" --> 

**150 jours**  <!-- .element: class="fragment" -->

Note:
- **L** : SEQ réussite, si on industrialisait ?
- 2 derniers produits, c'est possible, gain de temps ! aller plus loin avec le template
- Nouvelle équipe socle à créer, organisation revue, remontée DSI
- Budget DSI : 200 jours alloués — objectif : produire un parcours en 150 jours

---

## Au-delà des chiffres ?

J'ai planté des graines qui germent. <!-- .element: class="fragment" --> 

Le TDD n'est pas juste un buzzword <!-- .element: class="fragment" --> 

Une infusion en douceur est un bon gage d'adoption <!-- .element: class="fragment" --> 

Une expérience très enrichissante <!-- .element: class="fragment" --> 

Au-delà de mes espérances <!-- .element: class="fragment" --> 

Note:
- **D** résultat non quantifiable / non négligeable
- mon équipe : J'ai planté des graines qui germent 
  - Pas de connaissance du Craft /=> convaincu par le TDD
  - un se lance à la découverte vaste nouveau monde
- autres équipe curiosité piquée par l'exemple
  - ma volonté de péréniser 
  - Atelier TDD MOB en condition réelle (vrai code de 0)
  - Tous très bon retours (que 3) / pertinence des pratiques
- les autres (PO, managers) m'ont fait confiance mais 
  - les produits sont plutôt stables
  - SFS en retard donc pas trop convaincus par la méthode
  - maintenant voient les bénéfices
  - ça se travaille / TDD n'est pas juste un buzzword
- Avec du recul
  - attitue Agile Craft Infusion en douceur
  - en co-construction / en baby step => infusion douce bon gage
- Si on m'avait dit ... ouais bon, exagèe pas
- FIER

---

## Et la suite ...

Équipe socle est en place <!-- .element: class="fragment" -->

Template est en cours de développement <!-- .element: class="fragment" -->

Formations sur le TDD pour les autres équipes <!-- .element: class="fragment" -->

Réflexions dans d'autres services pour industrialiser via des templates <!-- .element: class="fragment" -->

Note:
**L** — Ce qui est en cours
- Équipe socle en place (1 PO, 2 devs)
- Template en développement
- Formations TDD dans les autres équipes du pôle
- Réflexions template plus large dans d'autres services de la DSI

---

<!-- .slide: class="slide-accent" -->

## L'atelier, aujourd'hui

![BD — L'atelier transformé](assets/3_atelier_transforme.png) <!-- .element: style="max-height: 50vh;" -->

Note:
**D** — Retour sur Liza
- Liza est sereine, chaîne les commandes, se concentre sur les besoins spécifiques
- Elle peut se revendiquer artisane. Alptis aussi.

---

<!-- .slide: class="slide-accent" -->

## Merci

<div class="speaker-row">
  <div class="speaker-card">
    <img src="assets/Didier.jpg" alt="Didier ERIN"/>
    <p><strong>Didier ERIN</strong></p>
  </div>
  <div class="speaker-card">
    <img src="assets/Laure.jpg" alt="Laure CHAMPEL"/>
    <p><strong>Laure CHAMPEL</strong></p>
    <img src="assets/qr-code-linkedin-laure.png" alt="feedback" height="150px" style="border-radius:10% !important"  />
  </div>
  <div style="background-color:white;padding:20px;">
    <img src="assets/qr-code-openfeedback.png" alt="feedback" height="150px"  />
    <p><strong>Feedback</strong></p>
  </div>
</div>

Lyon Craft 2026

Note:
**L** — Clôture
- Merci de nous avoir écoutés
- On répond à vos questions
