---
title: "Et Craft la chaise !"
theme: moon
css: assets/custom.css
revealOptions:
  transition: slide
  slideNumber: false
  hash: true
---

<!-- .slide: class="slide-accent" -->

# Et Craft la chaise !

### Le TDD, de l'optimisation à l'industrialisation

REX ![Logo Alptis](assets/logo-alptis-white.svg) <!-- .element: style="width: 200px; vertical-align: middle; margin-bottom: 0.9em;" -->

**Didier ERIN** · **Laure CHAMPEL** 

Lyon Craft 2026

---

<!-- .slide: class="slide-accent" -->

## L'atelier de Liza

![BD — Ça craque](assets/1_ca_craque.png) <!-- .element: style="max-height: 65vh;" -->

---

## La douleur et le déclic

### Migration Java 11 → 21

Absence d'une batterie de test pertinente
- Bugs et régressions détectés tardivement 
- Allers-retours dev ↔ recette 
- « Alors, ... qu'est-ce que j'ai cassé ? »

**Sans filet, vouloir accélérer reste un pari.** <!-- .element: class="fragment" -->

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

*Comment l'atelier de Liza s'est transformé ?*

---

## La norme

| | |
|---|---|
| **Durée** | 6 à 7 mois / produit |
| **Équipe** | 4-5 personnes (PO, QA, 3 devs) |
| **Produits** | Santé Select, Santé Protect, Santé Pro + |

C'est la norme. Le produit est satisfaisant. <!-- .element: class="fragment" -->

**Mais besoin de produire plus.** <!-- .element: class="fragment" -->

---

<!-- .slide: class="slide-accent" -->

> *On veut produire plus vite, <br>
mais on serre les fesses quand on s'assoit sur la chaise.*

**Faut-il revoir la façon dont on fabrique nos chaises ?** <!-- .element: class="fragment" -->

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

Livraison continue <!-- .element: class="fragment" -->

Périmètre allégé <!-- .element: class="fragment" -->

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

## 7 mois — résultat contrasté

dont 1 mois de retard

<blockquote class="fragment"><em>Mais on desserre les fesses.</em></blockquote>

On livre sûr et simplifié, on peut aller plus vite <!-- .element: class="fragment" -->

---

## Le métier vient à nous

Nouveau produit à sortir. Le métier demande :

**"Comment minimiser le temps de réalisation ?"**

*"Si la chaise a les mêmes pieds, ça ira vite."* <!-- .element: class="fragment" -->

→ *"OK pour les mêmes pieds."* <!-- .element: class="fragment" -->

Décision : **dupliquer Santé Frontaliers Suisses** <!-- .element: class="fragment" -->

Note: Laure. Raconter l'anecdote. Ce renversement a pris des années — le craft seul ne suffit pas.

---

## Résultat : Santé Équilibre en 3 mois

Au bout de 2 mois, version quasi complète en prod.<br/>
\+ 1 mois pour les branchements aux services externes.

> *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."* <!-- .element: class="fragment" -->

*"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."* <!-- .element: class="fragment" -->

Note: Didier. Duplication SFR : tests + structure du code. Nouveau levier : découplage services externes. En recette : quasi aucun retour. Le dev n'est le goulot à aucun moment.

---

## Le déclic du template

Un produit vivant, recetté, toujours à jour.

Chaque nouveau produit part du template — les déclinaisons se concentrent sur les **spécificités**.

**Objectif DSI 2026** : parcours de vente en **150 jours**
> *Plan de la chaise en cours de réalisation*

Note: Laure. Template vivant, corrections sur produit ET template. Formation TDD en cours hors équipe expérimentale. L'organisation a internalisé.

---

<!-- .slide: class="slide-accent" -->

## L'atelier, aujourd'hui

![BD — L'atelier transformé](assets/3_atelier_transforme.png) <!-- .element: style="max-height: 50vh;" -->

> *"Développer est un métier.*
>
> *Être artisan développeur en est un autre."*

Note: Duo (D puis L). Vignette 1 : l'atelier transformé, les chaises tiennent. Vignette 2 : on se concentre sur la personnalisation. Punchline après silence. L : « Merci ».

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
</div>

Lyon Craft 2026
