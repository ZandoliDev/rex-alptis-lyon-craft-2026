---
title: "Développer est un métier. Être artisan développeur en est un autre."
theme: moon
revealOptions:
  transition: slide
  slideNumber: true
---

# Du craft à l'industrialisation

### REX Alptis — Lyon Craft 2026

**Didier** · **Laure**

---

## L'atelier

Un atelier de menuiserie. Des artisans fabriquent des chaises.

Chaque chaise est construite, puis testée en fin de chaîne — on vérifie que ça tient quand on s'assoit dessus.

Quand ça craque, on retourne à l'établi.

Note: Analogie d'ouverture — poser l'image mentale. Ton calme, descriptif.

---

## La question

Et si le vrai problème n'était pas **la vitesse** à laquelle on fabrique —

mais **la façon** dont on fabrique ?

---

<!-- .slide: data-background="#1a1a2e" -->

# Acte 1

## L'héritage : travailler sans filet

---

## Le contexte

Migration Java 11 → Java 21 en cours.

3 produits en production : Select, Protect, Select Pro.

Allers-retours dev ↔ recette. Bugs détectés tard. Cycles qui s'étirent.

---

## La norme

| | |
|---|---|
| **Durée** | 6 à 7 mois / produit |
| **Équipe** | 4-5 personnes (PO, SA, 3 dev) |
| **Livraison** | Mise en prod = mise en marché |

Personne ne remet cette norme en question.

---

## Le vrai sujet

> *"On veut produire plus vite, mais on serre les fesses quand on s'assoit dessus."*

Note: Formulation clé de l'acte 1. Laisser un silence après — la salle va sourire.

---

<!-- .slide: data-background="#1a1a2e" -->

# Acte 2

## L'expérimentation : repartir de zéro

*"Pour aller plus vite, il faut apprendre à livrer sûr."*

---

## SFR — Santé Frontaliers Suisses

Nouveau produit, from scratch.

Équipe nouvelle — sans expérience Alptis.

Double courbe d'apprentissage : **craft** + **contexte métier**.

---

## Ce qui se met en place

- **TDD** — conception émergente, refactorisation permanente
- **Mob programming** — transfert de compétences craft ↔ contexte
- **Règles métier d'abord** — scénarios validés tôt, recette allégée

---

## Ce qui se passe vraiment

- ~3 semaines absorbées par la friction organisationnelle
- Effectifs variables sur 5 phases
- Zones livrées sans TDD sous pression de deadline

Le craft n'est pas une recette magique.

---

## Le résultat

**7 mois** — autant que l'existant.

Mais avec une équipe qui démarre de zéro, un mois de friction, et une double courbe d'apprentissage.

> *"On n'a pas fait mieux en temps. On a fait autrement — et on a posé les fondations."*

---

## Ce qui a changé

**Avant** : on déploie en prod à la date de mise en marché, souvent avec retard.

**SFR** : livraisons en prod en continu tout au long du projet.

Le goulot commence à se déplacer.

---

<!-- .slide: data-background="#1a1a2e" -->

# Acte 3

## L'industrialisation

*"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."*

---

## Ce qui rend la duplication possible

1. **Capture de l'intention** — les tests documentent le sens
2. **Structure du code** — découplage, lisibilité, patterns
3. **Autonomie** — contrats d'interface, mocks par configuration
4. **Rapprochement métier / DSI** — co-conception dès le départ

---

## Santé Équilibre

| | |
|---|---|
| **Durée** | **2 mois** (première version en prod) |
| **Périmètre** | Plus complet que SFR à sa mise en marché |
| **Retard dev** | Zéro |
| **Retours en recette** | Quasi aucun |

+1 mois pour le branchement des services externes.

---

## Le goulot s'est déplacé

> *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*

Ce n'est plus le développement qui bloque.

---

## Le déclic du template

Un produit vivant, recetté, toujours à jour.

Chaque nouveau produit part du template — les déclinaisons se concentrent sur les **spécificités**.

Projection 3e produit : **~3 mois**.

---

<!-- .slide: data-background="#1a1a2e" -->

# Conclusion

---

## L'atelier, aujourd'hui

On ne réinvente plus la chaise à chaque commande.

On a conçu un **modèle de fabrication** — testé, validé, vivant.

Ce n'est pas de l'industrialisation fordiste.

C'est de la **maîtrise artisanale mise à l'échelle**.

---

## La punchline

> *"Développer est un métier.*
>
> *Être artisan développeur en est un autre."*

---

## Merci

**Didier** · **Laure**

Lyon Craft 2026
