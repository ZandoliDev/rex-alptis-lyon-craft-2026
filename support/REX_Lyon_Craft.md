---
title: "Et Craft la chaise !"
theme: moon
css: assets/custom.css
revealOptions:
  transition: slide
  slideNumber: true
  hash: true
---

<!-- .slide: data-background="#1b1040" -->

# Et Craft la chaise !

### REX Alptis Assurances
### Le TDD, de l'optimisation à l'industrialisation

![Logo Alptis](assets/logo-alptis-white.svg) <!-- .element: style="width: 200px; margin-top: 2em;" -->

**Didier ERIN** · **Laure CHAMPEL** — Lyon Craft 2026

Note: Slide de titre. Laisser la salle s'installer.

---

<!-- .slide: data-background="#1b1040" -->

## L'atelier

![BD — Ça craque](assets/1_ca_craque.png) <!-- .element: style="max-height: 65vh;" -->

Note: Didier. Vignette 1 : on a fini la chaise, on s'assoit. Vignette 2 : ça craque. Vignette 3 : retour à l'établi. « C'est pas de la négligence — c'est comme ça qu'on a toujours fait. »

---

## La douleur et le déclic

Migration Java 11 → 21

<div class="boucle">
  <span class="boucle-node">Dev</span>
  <span class="boucle-fleche">→</span>
  <span class="boucle-node">Recette</span>
  <span class="boucle-fleche">→</span>
  <span class="boucle-node boucle-node--alert">Bugs</span>
  <span class="boucle-fleche boucle-fleche--retour">↩</span>
</div>

Sans filet, chaque accélération reste un pari.

Note: Duo (Laure lead, Didier réagit). L : contexte migration en cours, bugs tard, allers-retours. D : incertitude « qu'est-ce que j'ai cassé ? », recette rallongée par précaution. D : c'est cette douleur qui fait émerger l'idée.

---

## Qui sommes-nous

<div class="speaker-row">
  <div class="speaker-card">
    <img src="assets/Didier.jpg" alt="Didier ERIN"/>
    <p><strong>Didier ERIN</strong><br/>Tech lead java<br/>L'artisan qui arrive, impulse le craft, structure les pivots</p>
  </div>
  <div class="speaker-card">
    <img src="assets/Laure.jpg" alt="Laure CHAMPEL"/>
    <p><strong>Laure CHAMPEL</strong><br/>Engineering manager<br/>L'ancrage dans l'organisation de l'atelier</p>
  </div>
</div>

*On va vous raconter comment cet atelier s'est transformé.*

Note: Duo — chacun se présente en une phrase. D : freelance craft, proposition de repartir sur des bases saines. L : Engineering manager. Continuité post-départ Didier.

---

## La norme

| | |
|---|---|
| **Durée** | 6 à 7 mois / produit |
| **Équipe** | 4-5 personnes (PO, QA, 3 devs) |
| **Produits** | Santé Select, Santé Protect, Santé Pro + |

C'est la norme et le produit est satisfaisant, <br/>
mais besoin de produire plus vite pour en sortir plus.

Note: Laure. Confirmé sur 3 produits. Ça fonctionne, le métier voudrait qu'on produise plus vite pour sortir plus de produits.

---

<!-- .slide: data-background="#1b1040" -->

> *"On veut produire plus vite, mais on serre les fesses quand on s'assoit sur la chaise."*

Et si le vrai problème n'était pas la vitesse à laquelle on fabrique — mais **la façon** dont on fabrique ?

Note: Didier. Écho au craquement de la slide 2. La question ouvre l'acte 2.

---

## Repartir de zéro avec le craft

**Santé Frontaliers Suisses** — nouveau produit.

Équipe nouvelle — zéro expérience Alptis.

Double courbe d'apprentissage : **craft** + **contexte métier**.

Note: Duo (L puis D). L : L'occasion de repartir sur des bases saines, nouveau produit, nouvelle équipe, nous décidons d'expérimenter le TDD. D : double pari craft + contexte métier. Pas un labo, un vrai produit avec une vraie date.

---

## Ce qu'on met en place

- **TDD** — conception émergente, refactorisation continue
- **Mob programming** — montée en compétence en temps réel
- **US itératives** — le produit émerge par incréments
- **Livraison continue** — déploiement tout au long du projet
- **Périmètre allégé** — focus cœur métier

Note: Didier. Donner le pourquoi de chaque levier, pas juste le quoi.

---

<!-- .slide: data-background="#1b1040" -->

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

~3 semaines de friction organisationnelle. Congés successifs.<br/>
TDD lâché sous pression de deadline sur certaines zones.

Note: Duo (D puis L). D : détailler les 4 phases, insister sur les 2 derniers mois (TDD lâché sous pression). L : ~3 semaines de friction orga (standardisation produit). D : côté front — 1 dev formé en pair, adopte le TDD en autonomie.

---

## 7 mois — résultat contrasté

*dont 1 mois de retard*

**Périmètre en TDD** — Intention garantie, pas de régression<br/>
**Périmètre sans TDD** — Modules éprouvés, mais retour à la dépendance de la recette<br/>

> *"On a mis 7 mois. Mais on desserre les fesses."*

*"Pour aller plus vite, il faut apprendre à livrer sûr."*

Note: Didier. Rappeler le contexte : équipe neuve, friction orga, double apprentissage → en conditions normales ~6 mois. Thèse : « pour aller plus vite, il faut apprendre à livrer sûr ».

---

## Le métier vient à nous

Nouveau produit à sortir. Le métier demande :

**"Comment minimiser le temps de réalisation ?"**

*"Si la chaise a les mêmes pieds, ça ira vite."*<br/>
→ *"OK pour les mêmes pieds."*

Décision : **dupliquer Santé Frontaliers Suisses**

Note: Laure. Raconter l'anecdote. Ce renversement a pris des années — le craft seul ne suffit pas.

---

## Résultat : Santé Équilibre

<div class="chiffre-hero">2 mois</div>

version quasi complète en prod

<div class="chiffre-sub">+ 1 mois</div>

branchements aux services externes

> *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*

*"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."*

Note: Didier. Duplication SFR : tests + structure du code. Nouveau levier : découplage services externes. En recette : quasi aucun retour. Le dev n'est le goulot à aucun moment.

---

## Le déclic du template

<div class="schema-template">
  <div class="schema-source">Template vivant<br/><span class="schema-detail">recetté, toujours à jour</span></div>
  <div class="schema-fleches">
    <span>→</span>
    <span>→</span>
    <span>→</span>
  </div>
  <div class="schema-produits">
    <span class="schema-produit">Produit A</span>
    <span class="schema-produit">Produit B</span>
    <span class="schema-produit">Produit …</span>
  </div>
</div>

Déclinaisons concentrées sur les **spécificités**

**Objectif DSI 2026** : parcours de vente en **150 jours**

> *Plan de la chaise en cours de réalisation*

Note: Laure. Template vivant, corrections sur produit ET template. Formation TDD en cours hors équipe expérimentale. L'organisation a internalisé.

---

<!-- .slide: data-background="#1b1040" -->

## L'atelier, aujourd'hui

![BD — L'atelier transformé](assets/3_atelier_transforme.png) <!-- .element: style="max-height: 50vh;" -->

> *"Développer est un métier.*
>
> *Être artisan développeur en est un autre."*

Note: Duo (D puis L). Vignette 1 : l'atelier transformé, les chaises tiennent. Vignette 2 : on se concentre sur la personnalisation. Punchline après silence. L : « Merci ».

---

<!-- .slide: data-background="#1b1040" -->

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
