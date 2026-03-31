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

**Didier ERIN** · **Laure CHAMPEL** — Lyon Craft 2026

---

<!-- .slide: class="slide-accent" -->

## L'atelier de Liza

![BD — Ça craque](assets/1_ca_craque.png) <!-- .element: style="max-height: 65vh;" -->

Note: 

Didier<br/>
Voici un atelier d'une Liza, elle fabrique des chaises dans son atelier.<br/>
Une fois que Liza a fini sa chaise, elle teste et CRAC ! <br/>
La chaise casse, dommage, il n'y a plus qu'à recommencer

Cette histoire est une analogie de ce qui arrive sur de nombreux projets <br/>
C'est ce qui arrivait chez Alptis et nous allons vous raconter comment le Craft a permis de faire évoluer les choses.

---

## La douleur et le déclic

### Migration Java 11 → 21

Absence d'une batterie de test pertinente
- Bugs et régressions détectés tardivement <!-- .element: class="fragment" -->
- Allers-retours dev ↔ recette <!-- .element: class="fragment" -->
- « Alors, ... qu'est-ce que j'ai cassé ? » <!-- .element: class="fragment" -->

**Sans filet, chaque accélération reste un pari.** <!-- .element: class="fragment" -->

Note: Laure / Didier

Laure<br/>
contexte migration en cours<br/>
bugs tard<br/>
allers-retours<br/>

Didier<br/>
C'est dans ce contexte que j'arrive chez Alptis en tant que futur Tech Lead.
"Ils sont bien gentils chez Alptis, je n'ai clairement pas envie de revivre ça <br/>
Il va falloir changer la façon de travailler"

---

## Qui sommes-nous

<div class="speaker-row">
  <div class="speaker-card">
    <img src="assets/Didier.jpg" alt="Didier ERIN"/>
    <p><strong>Didier ERIN</strong><br/>Tech lead java<br/>Piqué par le Craft depuis 3 ans, souhaite expérimenter ça en vrai</p>
  </div>
  <div class="speaker-card">
    <img src="assets/Laure.jpg" alt="Laure CHAMPEL"/>
    <p><strong>Laure CHAMPEL</strong><br/>Engineering manager<br/>L'ancrage dans l'organisation de l'atelier</p>
  </div>
</div>

*On va vous raconter comment l'atelier de Liza s'est transformé.*

Note: Didier / Laure

Didier<br/>
Bonjour à tous et merci pour votre présence, il est temps de faire les présentations<br/>
Je m'appelle Didier et je suis dans le développement logiciel depuis une quinzaine d'années.<br/>
Ça fait 3 ans que le Craft me fascine et je vois chez Alptis une opportunité d'expérimenter ça grandeur nature.

Laure<br/>

— chacun se présente en une phrase. D : freelance craft, proposition de repartir sur des bases saines. L : Engineering manager. Continuité post-départ Didier.

---

## La norme

| | |
|---|---|
| **Durée** | 6 à 7 mois / produit |
| **Équipe** | 4-5 personnes (PO, QA, 3 devs) |
| **Produits** | Santé Select, Santé Protect, Santé Pro + |

C'est la norme. Le produit est satisfaisant.

Mais besoin de produire **plus vite** pour en sortir **plus**. <!-- .element: class="fragment" -->

Note: Laure. Confirmé sur 3 produits. Ça fonctionne, le métier voudrait qu'on produise plus vite pour sortir plus de produits.

---

<!-- .slide: class="slide-accent" -->

> *"On veut produire plus vite, mais on serre les fesses quand on s'assoit sur la chaise."*

Et si le vrai problème n'était pas la vitesse à laquelle on fabrique — mais **la façon** dont on fabrique ? <!-- .element: class="fragment" -->

Note: Didier. Écho au craquement de la slide 2. La question ouvre l'acte 2.

---

## Repartir de zéro avec le craft

**Santé Frontaliers Suisses** — nouveau produit.

Équipe nouvelle — zéro expérience Alptis.

Double courbe d'apprentissage : **craft** + **contexte métier**.

Note: Duo (L puis D). L : L'occasion de repartir sur des bases saines, nouveau produit, nouvelle équipe, nous décidons d'expérimenter le TDD. D : double pari craft + contexte métier. Pas un labo, un vrai produit avec une vraie date.

---

## Ce qu'on met en place

- **TDD** — conception émergente, refactorisation continue <!-- .element: class="fragment" -->
- **Mob programming** — montée en compétence en temps réel <!-- .element: class="fragment" -->
- **US itératives** — le produit émerge par incréments <!-- .element: class="fragment" -->
- **Livraison continue** — déploiement tout au long du projet <!-- .element: class="fragment" -->
- **Périmètre allégé** — focus cœur métier <!-- .element: class="fragment" -->

Note: Didier. Donner le pourquoi de chaque levier, pas juste le quoi.

---

<!-- .slide: class="slide-accent" -->

## L'apprentissage

![BD — L'apprentissage](assets/2_l_apprentissage.png) <!-- .element: style="max-height: 65vh;" -->

Note: Didier. Vignette 1 : le maître artisan montre les techniques. Vignette 2 : l'apprentie essaye. Vignette 3 : pas encore à l'aise, mais quelque chose a changé.

---

## Ce qui se passe vraiment

<div class="frise">
  <div class="frise-phase" style="flex: 1.5;">
    <span class="frise-label">Mob</span>
    <span class="frise-duree">~1,5 mois</span>
  </div>
  <div class="frise-phase" style="flex: 1.5;">
    <span class="frise-label">Pair</span>
    <span class="frise-duree">~1,5 mois</span>
  </div>
  <div class="frise-phase" style="flex: 1;">
    <span class="frise-label">Hybride</span>
    <span class="frise-duree">~1 mois</span>
  </div>
  <div class="frise-phase frise-phase--warning" style="flex: 2;">
    <span class="frise-label">Sans Didier</span>
    <span class="frise-duree">~2 mois</span>
  </div>
</div>

~3 semaines de friction organisationnelle. Congés successifs. <!-- .element: class="fragment" -->

TDD lâché sous pression de deadline sur certaines zones. <!-- .element: class="fragment" -->

Note: Duo (D puis L). D : détailler les 4 phases, insister sur les 2 derniers mois (TDD lâché sous pression). L : ~3 semaines de friction orga (standardisation produit). D : côté front — 1 dev formé en pair, adopte le TDD en autonomie.

---

## 7 mois — résultat contrasté

*dont 1 mois de retard*

**Périmètre en TDD** — Intention garantie, pas de régression <!-- .element: class="fragment" -->

**Périmètre sans TDD** — Modules éprouvés, mais retour à la dépendance de la recette <!-- .element: class="fragment" -->

> *"On a mis 7 mois. Mais on desserre les fesses."* <!-- .element: class="fragment" -->

*"Pour aller plus vite, il faut apprendre à livrer sûr."* <!-- .element: class="fragment" -->

Note: Didier. Rappeler le contexte : équipe neuve, friction orga, double apprentissage → en conditions normales ~6 mois. Thèse : « pour aller plus vite, il faut apprendre à livrer sûr ».

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
