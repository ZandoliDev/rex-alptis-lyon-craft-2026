# Trame narrative — REX Lyon Craft
> Livrable de l'étape 1 : chiffres intégrés et qualifiés dans la narration.  
> Base pour l'étape 2 (plan slide-by-slide).

---

## Chiffres structurants (version définitive qualifiée)

| Moment | Durée | Équipe | Périmètre | Nuances |
|--------|-------|--------|-----------|---------|
| Avant craft (moyenne sur 3 produits : Select, Protect, Select Pro) | 6-7 mois | 4-5 personnes constantes (PO, SA, 3 dev) | Standard — mise en prod = mise en marché, souvent avec retard | Référence de départ indiscutable : confirmée par l'équipe sur 3 produits |
| Produit 1 craft — SFR (Santé Frontaliers Suisses) | 7 mois | Variable sur 5 phases (1+3+1+1+1) | Standard — périmètre légèrement réduit sur les fonctionnalités de confort (ajoutées après coup) | ~3 semaines absorbées par friction organisationnelle (standardisation produit) ; équipe sans aucune expérience Alptis, apprend craft ET contexte simultanément ; mise en marché retardée d'1 mois (durée des dev) — malgré ce retard, livrer en 7 mois dans ce contexte d'expérimentation et de contraintes est considéré comme une bonne performance |
| Produit 2 craft — Santé Équilibre | 2 mois pour une première version quasi complète en prod, avant mise en marché | Non précisé | Plus standard, avec spécificités éditiques ; périmètre fonctionnel plus complet que SFR dès la mise en prod | +1 mois pour branchement services externes → mise en prod définitive avant la date de mise en marché, zéro retard côté dev |
| Produit 3 (projection) | ~3 mois (à confirmer avec Laure) | — | À ajuster selon spécificités | Chiffre indicatif, non définitif |

---

## Ouverture — L'analogie pour entrer dans le sujet

**Image de départ :** Un atelier de menuiserie. Des artisans fabriquent des chaises. Chaque chaise est construite, puis testée en fin de chaîne — on vérifie que ça tient quand on s'assoit dessus. Quand ça craque, on retourne à l'établi.

Ce n'est pas de la négligence. C'est simplement la façon dont l'atelier a toujours fonctionné.

**Tension posée :** Ce mode de fonctionnement a un coût invisible. Pas de catastrophe, mais des allers-retours, de l'incertitude, de la charge mentale. Et surtout : une difficulté croissante à fabriquer plus, plus vite, sans perdre en qualité.

**Question ouverte au public :** Et si le vrai problème n'était pas la vitesse à laquelle on fabrique — mais la façon dont on fabrique ?

---

## Acte 1 — L'héritage : travailler sans filet

**Thèse de l'acte :** Sans filet, chaque changement est une prise de risque. On avance, mais on subit.

**Situation concrète (anecdote d'entrée) :**
Didier arrive chez Alptis en pleine migration technique Java 11 → Java 21. Les produits existants — Select, Protect, Select Pro — sont en production depuis plusieurs mois. La migration s'étire, avec de nombreux allers-retours entre développement et recette, des bugs et régressions détectés tardivement. Des cycles qui auraient pu être raccourcis avec une batterie de tests complète et pertinente. *(Durée et coût précis à confirmer avec Laure.)*

**Ce que ça révèle :**
- Travailler sur un existant sans filet de tests suffisant, c'est avancer avec l'incertitude permanente de "qu'est-ce que j'ai cassé sans le savoir ?".
- Conséquences concrètes : demandes de validation fréquentes, recettes lourdes par précaution, charge mentale élevée, process de delivery ralenti.
- La qualité des produits existants n'est pas en cause — peu de bugs visibles en prod. Mais la qualité de *conception* et l'absence de filet rendent chaque évolution coûteuse.

**Chiffre de référence :** 6-7 mois par produit. Équipe de 4-5 personnes. C'est la norme. Personne ne la remet en question.

**Formulation clé :** *"On ne se demande pas si on peut aller plus vite. On se demande comment ne pas tout casser."*

**Pont vers l'acte 2 :** C'est dans ce contexte que commence l'expérimentation. Non pas pour aller plus vite — mais pour retrouver de la maîtrise.

---

## Acte 2 — L'expérimentation : repartir de zéro avec le craft

**Thèse de l'acte :** *"Pour aller plus vite, il faut apprendre à livrer sûr."*

**Situation concrète :**
Nouveau produit from scratch : Santé Frontaliers Suisses (SFR). L'occasion de repartir sur des bases saines. Équipe nouvelle, sans expérience Alptis — qui apprend le craft et le contexte métier en même temps.

**Ce qui se met en place :**
- TDD : conception émergente plutôt que projetée, refactorisation permanente, code qui exprime l'intention métier.
- Mob programming : transfert de compétences entre Didier (craft) et les membres de l'équipe (contexte fonctionnel et technique Alptis). Review et recette croisée allégées quand l'équipe travaille ensemble.
- Focalisation sur les règles métier avant les briques techniques : les scénarios sont validés tôt, la recette devient surtout un contrôle d'assemblage.

**Ce qui se passe vraiment (honnêteté sur les limites) :**
- ~3 semaines absorbées par des contraintes organisationnelles (standardisation des produits) — pas de la complexité technique.
- Variations d'effectifs sur 5 phases : mob → pair → solo → sans Didier → dev seul.
- Période de congés successifs : perte d'expertise temporaire, retours tardifs en recette.
- Phase 3 : arrivée d'une dev expérimentée Alptis, qui suit le mode TDD sur les modules intégrés en TDD. Mais le dev senior présent tout au long de la mission, seul sur certains modules, sous pression de deadline et sans Didier pour leader le TDD, ne se sent pas suffisamment à l'aise pour le pratiquer de manière autonome. Résultat : certaines zones livrées sans TDD.
- Résultat : là où le craft est appliqué, l'intention est garantie sans régression. Là où il est abandonné sous pression, les modules livrés sont globalement éprouvés — peu de bugs — mais on perd la certitude avant les tests. On retourne à la dépendance à la recette pour valider ce qu'on ne sait plus garantir soi-même.

**Chiffre :** 7 mois pour SFR. Soit autant que l'existant — avec une équipe qui démarre de zéro, un mois de friction organisationnelle, et une courbe d'apprentissage double (craft + contexte Alptis). En conditions normales : ~6 mois.

**Ce qui a changé :**
- Avant : on déployait en prod à la date de mise en marché, souvent avec retard.
- SFR : choix délibéré de livrer en prod en continu tout au long du projet — ce mode était techniquement possible avant, mais c'est une décision prise dès SFR pour réduire la charge mentale de la mise en production finale. La mise en marché a été retardée d'un mois, principalement due à la durée des développements. Malgré ce retard, livrer en 7 mois dans ce contexte d'expérimentation et de contraintes était déjà considéré comme une bonne performance.
- La certitude sur l'intention implémentée est là. Le goulot commence à se déplacer.

**Formulation clé :** *"On n'a pas fait mieux en temps. On a fait autrement — et on a posé les fondations."*

**Pont vers l'acte 3 :** Une fois l'intention capturée, la structure posée, les compétences acquises — une question émerge naturellement : et si on dupliquait ?

---

## Acte 3 — L'industrialisation : quand la maîtrise devient un levier

**Thèse de l'acte :** *"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."*

**Situation concrète :**
Nouveau produit : Santé Équilibre. Produit plus standard que SFR, avec des spécificités éditiques. La décision : dupliquer SFR comme base, valider que le système fonctionne, puis envisager l'industrialisation.

**Ce qui rend la duplication possible :**
Quatre éléments combinés — aucun ne suffit seul :
1. **Capture de l'intention** : les tests documentent ce que le code est censé faire. On duplique aussi le sens.
2. **Structure du code** : découplage, lisibilité, refactorisation, patterns. Le code est conçu pour évoluer.
3. **Autonomie vis-à-vis des dépendances** : accord préalable sur les contrats d'interface, simulation par configuration (mock vs réel). On peut avancer sans attendre les autres équipes.
4. **Rapprochement métier / DSI** : les actuaires co-conçoivent avec dev, PO et DSI. Moins de règles "exotiques", structure plus standard, faisabilité intégrée dès la conception.

**Ce que ça donne :**
- Santé Équilibre : **2 mois** pour avoir une première version quasi complète en prod, avant la date de mise en marché — avec un périmètre fonctionnel plus complet que SFR à sa mise en marché.
- La mise en prod définitive intervient avant la date de mise en marché. Zéro retard côté dev.
- +1 mois pour le branchement des services externes (goulot déplacé : ce n'est plus le développement qui bloque).
- En recette : quasi aucun retour — les retours hérités du produit 1 sont déjà absorbés.

**Le déclic du template :**
"On a une base livrable en prod. Pourquoi ne pas en faire un template produit ?"
- Le template devient un produit vivant, recetté de bout en bout, toujours à jour.
- Corrections portées sur le produit détecté ET sur le template.
- Fonctionnalités communes intégrées au template.
- Chaque nouveau produit part du template — les déclinaisons se concentrent sur les spécificités.

**Projection :**
Un 3e produit avec le template en place : ~3 mois (à confirmer avec Laure, à ajuster selon spécificités).

**Formulation clé :** *"Le goulot s'est déplacé : du développement vers la recette et les dépendances externes."*

---

## Conclusion — Fermeture de l'analogie et punchline

**Retour à l'atelier :**
L'atelier n'est plus le même. On ne réinvente plus la chaise à chaque commande. On a conçu un modèle de fabrication — testé, validé, vivant. Les artisans se concentrent sur ce qui est spécifique à chaque client, pas sur ce qui est déjà résolu.

Ce n'est pas de l'industrialisation au sens fordiste du terme. C'est de la maîtrise artisanale mise à l'échelle.

**Honnêteté finale :**
On n'a pas tout réussi du premier coup. Il y a eu des compromis, des zones sans TDD, des periodes de turbulence. Le craft n'est pas une recette magique — c'est un investissement, avec une courbe d'apprentissage réelle.

Mais là où l'intention a été tenue : pas de régression. Pas de surprise. De la prévisibilité.

**Punchline assumée :**
*"Développer est un métier. Être artisan développeur en est un autre."*

---

## Points à confirmer avec Laure avant le talk

- Durée et coût approximatif de la migration Java 11 → Java 21 (allers-retours dev-recette).
- Projection 3e produit : ~3 mois à valider.
- Détails sur l'organisation post-départ (template, formations, budget débloqué).
- Arbitrage sur les éléments citables publiquement (noms de produits, chiffres internes).
