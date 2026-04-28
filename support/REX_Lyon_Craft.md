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

# Et Craft la chaise !

### De l'optimisation à l'industrialisation

REX ![Logo Alptis](assets/logo-alptis-color.svg) <!-- .element: style="width: 200px; vertical-align: middle; margin-bottom: 0.9em;" -->

**Didier ERIN** · **Laure CHAMPEL** 

Lyon Craft 2026

---

## L'atelier de Liza

![BD — Ça craque](assets/1_ca_craque.png) <!-- .element: style="max-height: 65vh;" -->

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

---
## Quelques mots sur Alptis

![Logo Alptis](assets/logo-alptis-color.svg) <!-- .element: style="width: 200px; vertical-align: middle; margin-bottom: 0.9em;" -->

Courtier grossiste en assurance <!-- .element: class="fragment" -->

Parcours de vente <!-- .element: class="fragment" -->

Santé individuelle (complémentaire santé) <!-- .element: class="fragment" -->

---

*Comment l'atelier de Liza s'est transformé ?*

---

## La douleur et le déclic

- Contexte : Migration Java 11 → 21 <!-- .element: class="fragment" -->
- Absence d'une batterie de test pertinente <!-- .element: class="fragment" -->
- Bugs et régressions détectés tardivement <!-- .element: class="fragment" -->
- Allers-retours dev ↔ recette <!-- .element: class="fragment" -->
- « Alors, ... qu'est-ce que j'ai cassé ? » <!-- .element: class="fragment" -->

---

*Il faut que ça change !*

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
  </div>
</div>

<div class="norme-workflow fragment">
<div><strong>Le worflow</strong></div>
  conception &nbsp;→&nbsp; dev &nbsp;→&nbsp; recette technique &nbsp;→&nbsp; recette fonctionnelle &nbsp;→&nbsp; démo métier
</div>

*Santé Select · Santé Protect · Santé Pro +* <!-- .element: class="fragment" style="font-size:0.7em; color: var(--text-muted);" -->

**C'est la norme. Le produit est satisfaisant.** <!-- .element: class="fragment" -->

---
## Le constat

On repart chaque fois de zéro. <!-- .element: class="fragment" -->

Seulement 2 produits par an. <!-- .element: class="fragment" -->

**Mais souhait de produire plus.** <!-- .element: class="fragment" -->

---

<!-- .slide: class="slide-accent" -->

> *On veut produire plus vite, <br>
mais on serre les fesses quand on s'assoit sur la chaise.*

**Et si le vrai problème n'était pas la vitesse, mais la façon dont on fabrique les chaises ?** <!-- .element: class="fragment" -->

---

## Repartir de zéro avec le craft

**Nouveau produit : Santé Frontaliers Suisses** <!-- .element: class="fragment" data-fragment-index="1" -->

Nouvelle équipe <!-- .element: class="fragment" data-fragment-index="2" -->

**Triple courbe d'apprentissage** <!-- .element: class="fragment" data-fragment-index="3" -->
* TDD <!-- .element: class="fragment" data-fragment-index="3" -->
* La santé individuelle <!-- .element: class="fragment" data-fragment-index="3" -->
* L'environnement Alptis <!-- .element: class="fragment" data-fragment-index="3" -->

---

## Ce qu'on met en place

TDD <!-- .element: class="fragment" -->

Mob programming <!-- .element: class="fragment" -->

US itératives <!-- .element: class="fragment" -->

Périmètre allégé <!-- .element: class="fragment" -->

Livraison continue <!-- .element: class="fragment" -->

---

<!-- .slide: class="slide-accent" -->

## L'apprentissage

![BD — L'apprentissage](assets/2_l_apprentissage.png) <!-- .element: style="max-height: 65vh;" -->

---

## Ce qui se passe vraiment

<div class="frise-vertical">
  <div class="frise-phase fragment">
    <span class="frise-label">Mob</span>
    <span class="frise-duree">~1,5 mois</span>
  </div>
  <div class="frise-phase fragment">
    <span class="frise-label">Pair</span>
    <span class="frise-duree">~2 mois</span>
  </div>
  <div class="frise-phase fragment">
    <span class="frise-label">Hybride</span>
    <span class="frise-duree">~1,5 mois</span>
  </div>
  <div class="frise-phase frise-phase--warning fragment">
    <span class="frise-label">Sans Didier</span>
    <span class="frise-duree">~2 mois</span>
  </div>
</div>

---

## Comme si ça ne suffisait pas ... 

Un besoin de standardisation mal exprimé à l'équipe <!-- .element: class="fragment" -->

Des dépendances avec des équipes externes <!-- .element: class="fragment" -->


---

## 7 mois — résultat contrasté

dont 1 mois de retard

<blockquote class="fragment"><em>Mais on desserre les fesses.</em></blockquote>

On livre sûr et simplifié, on peut aller plus vite <!-- .element: class="fragment" -->

---

## Le métier vient à nous

Nouveau produit à sortir : <strong>Santé Equilibre</strong>

*<strong>"Comment aller plus vite ?"</strong>* <!-- .element: class="fragment" -->

*"Si toutes les chaises ont les mêmes pieds, ça ira vite."* <!-- .element: class="fragment" -->

*"OK pour les mêmes pieds."* <!-- .element: class="fragment" -->

---

## La décision

- Nouveau produit très similaire <!-- .element: class="fragment" -->
- Code stable et testé <!-- .element: class="fragment" -->
- Base saine pour des adaptations rapides <!-- .element: class="fragment" -->

**Décision : dupliquer Santé Frontaliers Suisses** <!-- .element: class="fragment" -->

---

## Santé Équilibre en 3 mois

2 mois : produit quasi complet

→ La recette devient le goulot d'étranglement <!-- .element: class="fragment" -->

→ Des retours imputables à Santé Frontaliers Suisses <!-- .element: class="fragment" -->

→ simulation des services externes à la demande <!-- .element: class="fragment" -->

---

## Santé Équilibre en 3 mois

1 mois de rab pour :

→ nouveau comportement spécifique <!-- .element: class="fragment" -->

→ branchement avec les services externes <!-- .element: class="fragment" -->

→ quelques fonctionnalités de confort sur Santé Frontaliers Suisses et Santé Équilibre <!-- .element: class="fragment" -->

**"Mais alors ? L'industrialisation devient rationnelle !"** <!-- .element: class="fragment" -->

---

## Le déclic du template

Un produit interne vivant, recetté, toujours à jour.

200 jours alloués à la création de ce template <!-- .element: class="fragment" --> 

Objectif DSI 2026 : produire un parcours de vente en <!-- .element: class="fragment" --> 

**150 jours**  <!-- .element: class="fragment" -->

---

## Au-delà de la vitesse de production ?

J'ai planté des graines qui germent. <!-- .element: class="fragment" --> 

Le TDD n'est pas juste un buzzword <!-- .element: class="fragment" --> 

Une expérience tellement enrichissante <!-- .element: class="fragment" --> 

Une infusion en douceur est le meilleur gage de réussite <!-- .element: class="fragment" --> 

---

## Et la suite ...

- Équipe socle est en place <!-- .element: class="fragment" -->
- Template est en cours de développement <!-- .element: class="fragment" -->
- Formations sur le TDD pour les autres équipes <!-- .element: class="fragment" -->
- Réflexions dans d'autres services pour industrialiser via des templates <!-- .element: class="fragment" -->

---

<!-- .slide: class="slide-accent" -->

## L'atelier, aujourd'hui

![BD — L'atelier transformé](assets/3_atelier_transforme.png) <!-- .element: style="max-height: 50vh;" -->

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
  </div>
  <div style="background-color:white;padding:20px;">
    <img src="assets/qr-code-openfeedback.png" alt="feedback" height="150px"  />
    <p><strong>Feeback</strong></p>
  </div>
</div>

Lyon Craft 2026
