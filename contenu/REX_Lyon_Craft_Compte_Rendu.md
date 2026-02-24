# Compte rendu ultra détaillé — Conversation de travail (REX Lyon Craft)

Date de génération : 2026-02-24 09:22

> Objectif de ce document : permettre de **retracer l'évolution** de la conversation et de **capitaliser** sur toutes les décisions, formulations, pivots, contraintes, idées, anecdotes et éléments de contenu identifiés, afin de servir de base à :
> - l'élaboration du **talk**,
> - la création du **support de présentation**,
> - la préparation du **discours** associé à chaque diapo.

---

## 0) Contexte initial et cadre de travail

### 0.1 Contexte conférence / talk
- Talk prévu dans le cadre de **Lyon Craft** (conférence orientée craft / communautés dev).
- Format : **retour d'expérience (REX)** en **duo** avec **Laure** (toujours chez Alptis, continuité post-départ).
- Intention : ne pas faire un talk "théorie craft / pratiques", mais parler à un public initié craft sur **le 'comment' convaincre** / **comment ça se met en place**, et sur **l'impact** (organisationnel, delivery, time-to-market).

### 0.2 Matériel de départ
- Une présentation interne Alptis fournie par Laure sert de base, mais le rendu final doit être une présentation **Didier** (identité LinkedIn : indigo–sable, motif afro-caraïbéen discret).

### 0.3 Cadre de coaching
- Demande explicite : accompagnement **étape par étape**, sans "biaiser" les réponses.
- Au départ : interdiction de fournir des exemples issus de la mission (coaching pur).
- Puis évolution : demande d'exemples possibles (au moins hors-sujet), et enfin consolidation via journal de travail.

---

## 1) Mise en place d'un journal et d'un support de capitalisation

### 1.1 Besoin exprimé
- Besoin d'un outil "brainstorm / exploration / extraction" pour coucher :
  - éléments affichables (slides),
  - éléments d'oral,
  - anecdotes,
  - preuves / observations,
  - tensions et pivots.

### 1.2 Journal de travail
- Création et mise à jour d'un journal : `REX_Lyon_Craft_Journal.md` puis version `v2`.
- Objectif : document vivant pour :
  - garder la trace,
  - reprendre plus tard ou dans une nouvelle conversation,
  - alimenter la construction de slides + discours.

---

## 2) Clarification de l'angle du talk : de la "qualité" à la "maîtrise"

### 2.1 Idées fortes initiales (formulations successives)
- Idée de base (très tôt) :
  - "Les pratiques craft, même appliquées imparfaitement, avec l'esprit craft, apportent énormément de bénéfices."
  - "Le craft est un investissement qui paye rapidement."
- Tentatives de formulation :
  - "Plus de qualité = perte de temps = perte d'argent." (tension perçue côté client)
  - "En prenant le temps de faire de la qualité, on a gagné du temps."
  - "Prendre le temps de crafter permet de gagner du temps."
  - "Pour accélérer, miser sur la qualité."

### 2.2 Déplacement de la tension (point important)
- Problème relevé : certaines questions orientées "sur Didier" n'étaient pas pertinentes car Didier est convaincu du craft.
- Tension plus juste : côté **organisation / client** (Alptis), qui perçoit :
  - un coût initial,
  - des risques,
  - un doute sur le ROI.

### 2.3 Croyance ciblée identifiée
- Croyance organisationnelle explicitée :
  - "Nos produits sont déjà qualitatifs, peu de bugs : est-ce que ça vaut le coup d'investir plus ?"
- Clarification :
  - la "qualité" ne se résume pas au "faible taux de bugs" ;
  - la qualité concerne aussi l'**évolutivité**, la **prévisibilité**, la **charge mentale**, la **capacité de duplication/industrialisation**.

---

## 3) Définition progressive de ce que 'qualité' veut dire ici

### 3.1 Pistes de conséquences sans qualité (listées en brut)
- Retarder la demande du client.
- Produit qui suit mal la demande du marché.
- Développeurs qui se lancent à reculons.
- Client réticent à faire nouvelles demandes.
- Obsolescence plus rapide.
- Clients se tournant vers des acteurs plus réactifs.
- Vélocité d'adaptation technologique et capacité d'innovation réduites.
- Difficulté à innover rapidement / sortir régulièrement de nouvelles fonctionnalités.

### 3.2 Clarification majeure : filet de sécurité + conception
- Point soulevé :
  - "Filet de sécurité" (tests) et "qualité de conception" sont liés :
  - des tests ne suffisent pas si la conception rend l'évolution difficile.

### 3.3 Mot / concept qui émerge : **prévisibilité**
- Formulations convergentes :
  - "On sait de manière assez fiable ce qui va être impacté."
  - "Maîtriser les impacts de la majorité des changements à absorber."
  - "L'impact réel (pas supposé) des évolutions sur le produit."

---

## 4) Chronologie vécue en mission (structure en 3 phases)

### 4.1 Phase 1 — Corrections et petites évolutions sur existant
- Contexte : Didier arrive quand 3 parcours existaient déjà.
- Activité principale : corrections / petites évolutions.
- Difficulté : manque de maîtrise lié au manque de tests suffisamment nombreux et pertinents.
- Besoin central : "Être sûr que je n'ai rien cassé."
- Conséquences :
  - demande de validation,
  - ralentissement,
  - process de delivery lourd par précaution,
  - charge mentale élevée.

### 4.2 Phase 2 — Expérimentation craft (nouveau produit from scratch)
- Repartir de zéro avec une nouvelle méthodologie, bases reposées.
- Mise en place :
  - TDD,
  - conception émergente (vs conception projetée),
  - refactorisation permanente,
  - bonnes pratiques de lisibilité,
  - découplage et découpage,
  - usage de patterns pour simplifier,
  - focalisation règles métier avant briques techniques.
- Intention : ne pas reproduire certains travers / erreurs majeures de conception.

### 4.3 Phase 3 — Duplication intelligente / projection industrialisation
- Contexte métier : parcours de vente santé très similaires (différences estimées ~5%).
- Théoriquement industrialisable, mais avant craft : absence de sérénité.
- Découverte clé :
  - duplication envisageable grâce à :
    - intention capturée (tests),
    - compétences craft acquises (refacto, découplage, lisibilité, patterns),
    - structure de code permettant une base de duplication,
    - réduction de dépendance à certaines validations tardives.

---

## 5) Process de delivery : avant / après (résumé structuré)

### 5.1 Process initial (avant)
- Organisation Kanban avec phases :
  1. Conception : décrire impacts techniques pour réaliser une feature/tâche.
  2. Développement : réalisation + code review + recette croisée entre développeurs.
  3. Recette : QA ou PO (avec retours possibles).
  4. Tâche prête pour livraison (ou "livrable en prod").

- Synthèse "avant" (formulation itérée) :
  - Dev
  - Tests déployés (par prudence)
  - Review
  - Recette croisée
  - Recette QA
  - Retours

### 5.2 Process pendant TDD + mob (nuancé)
- Première formulation :
  - Dev
  - Tests déployés
  - Recette QA
  - Retours d'ajustement
- Nuance importante ajoutée ensuite :
  - la recette croisée n'a pas complètement disparu, elle a été **allégée** ;
  - en mob, on déployait en environnement de dev pour vérifier l'ensemble ; cela existait aussi avant (par le dev seul), mais la différence était le niveau de certitude sur les scénarios métiers via tests, hors précisions fonctionnelles tardives.

---

## 6) Pratiques craft mises en place et bénéfices observés

### 6.1 TDD : effets décrits
- Passage de "conception projetée" à "conception émergente" + refactorisation permanente.
- Simplification drastique du code, amélioration de la lisibilité.
- Code plus expressif dans son intention.
- Focalisation sur règles métiers avant briques techniques.
- Objectif/effet : garantir que l'implémentation répond correctement aux règles métier.
- Avant : validation surtout via tests en environnement complet (dev/recette).
- Après : scénarios métiers validés très tôt ; en recette on vérifie plutôt que le tout branché s'emboîte techniquement.
- Résultat exprimé : plus de certitude → plus de sérénité ; moins de dépendance à la recette.

### 6.2 Mob programming : effets décrits
- Transfert de compétences efficace :
  - Didier : craft,
  - un autre membre : expertise fonctionnelle/tech des parcours.
- Simplification du process de dev :
  - review et recette croisée devenaient moins nécessaires quand backend à 3 en mob.
- Frontend :
  - 1 seul dev, formé 1 journée (TDD + conception émergente),
  - puis il observe/applique seul jusqu'à la fin du projet.

### 6.3 Discussion sur la formulation "déplacer la preuve"
- Formulation jugée trop abstraite par Didier ("ça demande clarification").
- Alternative préférée : parler de validations techniques et fonctionnelles **avant** recette, feedback immédiat, et de la recette qui devient surtout un contrôle d'assemblage technique.

---

## 7) Réalité terrain : limites, accidents, régressions (récit détaillé)

### 7.1 Contraintes d'architecture imposées
- Intégration de contraintes liées à des choix d'architecture décidés au niveau service (structures standardisées, etc.).

### 7.2 Variations d'effectifs et d'appétence
- Mob programming surtout en début de projet (3 backend).
- Milieu de projet :
  - 2 backend → pair programming,
  - retour de review différée,
  - TDD maintenu,
  - review utilisée surtout pour garantir l'adoption des bonnes pratiques.
- Résultat : plus de retours en recette (méconnaissance métier/aspects techniques).

### 7.3 Période de congés successifs et perte d'expertise
- Productivité diminue.
- Plus de personne expérimentée → subtilités découvertes tard, en fin de recette.
- Effet : perte de temps, ajustements tardifs.

### 7.4 Arrivée d'une 3e personne expérimentée mais peu encline au mob
- Maintien review différée + TDD.
- Certaines parties livrées sans TDD (retour partiel "à l'ancienne") :
  - dev novice craft,
  - manque de compétences disponibles dans l'équipe,
  - pression deadline.

### 7.5 Enseignement majeur (exprimé par Didier)
- Courbe d'apprentissage non anodine.
- Mob programming pas adapté à tous les profils.
- Nécessité d'investir du temps avant autonomie/maturité.
- Malgré les compromis : l'intention implémentée restait globalement garantie sans régression sur les zones couvertes.

---

## 8) Acte 3 : construction progressive (éléments clés)

### 8.1 Démarche de départ
- "On duplique notre premier produit craft pour valider que le système de duplication fonctionne."
- "Ensuite, si OK, on envisagera l'industrialisation."

### 8.2 Dimension métier (actuaires) : bascule structurante
- Avant : actuaires conçoivent des produits indépendamment de la faisabilité technique/budget.
- Après le premier produit craft :
  - les métiers se rapprochent dev/PO/DSI pour co-concevoir un produit faisable rapidement,
  - en évitant des règles métiers "exotiques",
  - en convergeant vers une structure plus standard.
- Ce mouvement est présenté comme l'aboutissement de plusieurs années d'évolution agile/collaboration dans le service.

### 8.3 Duplication : déplacement du goulot d'étranglement vers la recette
- Process gardé identique au produit from scratch (par prudence / stabilité).
- Mais :
  - duplication du code **et** des tests,
  - base déjà prod-ready (puisque le produit source est en prod),
  - en recette : quasi aucun retour, retours hérités du produit 1.
- Déclic : dérouler un process "from scratch" story par story devient en partie une perte de temps ; goulot = recette.
- Décision : continuer le process pour éviter de gérer trop de changements simultanés.

### 8.4 Autonomie vis-à-vis des dépendances externes
- Parcours de vente branché à d'autres services (gestion contrat, éditique, signature électronique, etc.).
- Habitude : attendre les livraisons des autres équipes.
- Avec la base craft :
  - accord préalable sur le contrat d'interface,
  - possibilité de simuler/mocker par configuration (mock vs réel),
  - validation end-to-end sur une large portion (A→W), permettant d'avancer sans dépendre totalement des équipes externes.

### 8.5 Pivot complet (recadrage important)
- Didier précise que le pivot complet doit intégrer :
  - dépendances externes,
  - structure du code,
  - rapprochement MOE/métier,
  - capture de l'intention (tests) + compétences craft.

---

## 9) Industrialisation : changement de focale (ce que vous appelez "industrialiser")

### 9.1 Industrialisation ≠ uniquement factoriser le code
- Industrialiser = industrialiser aussi la façon de produire :
  - process agile,
  - travail du PO,
  - travail QA,
  - dev,
  - et la gestion du flux (au sens "chaîne de production").

### 9.2 Template : un produit vivant (déclic)
- Raisonnement : "On a une base livrable en prod : pourquoi ne pas en faire un template produit ?"
- Le template devient :
  - un produit à part entière,
  - recetté de bout en bout,
  - vivant/évolutif,
  - toujours à jour des décisions d'archi/process/modes de dev.

### 9.3 Règles de fonctionnement du template
- Toujours le template qui est dupliqué pour le prochain produit.
- Corrections :
  - corrigées sur le produit où détectées,
  - et portées sur le template.
- Fonctionnalités :
  - si commune/basique → intégrée au template.
- Recette :
  - le template passe lui-même une recette globale,
  - les déclinaisons se concentrent sur les spécificités (en conservant une non-régression globale au besoin).

### 9.4 Thèse de l'acte 3 (formulation retenue)
- **"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."**

---

## 10) Travail sur la phrase centrale / tension (itérations)

### 10.1 Sur "accélérer"
- Désaccord sur certaines formulations trop théoriques.
- Proposition qui a émergé et que Didier apprécie :
  - **"Pour aller plus vite, il faut apprendre à livrer sûr."**
- Ajustement factuel majeur :
  - en fin de projet, sous pression deadline + manque de compétences, craft a été temporairement lâché sur certaines zones → essentiel pour crédibilité.

### 10.2 Conclusion / provocation assumée
- Objectif émotionnel : que le public se dise "ah ouais le craft c'est pas que pour faire cool".
- Didier décide d'assumer une conclusion plus "provoc" (à condition de démonstration préalable).
- Phrase retenue :
  - **"Développer est un métier. Être artisan développeur en est un autre."**

---

## 11) Fil rouge : analogie menuiserie (construction et ajustements)

### 11.1 Objectif analogie
- Captiver, pragmatique, mémorable.
- Décision : analogie pour **ouvrir** et **fermer** le talk, avec touches de rappel par acte.

### 11.2 Première version de l'analogie (structure)
- Acte 1 : construire des chaises en vérifiant surtout à la fin.
- Acte 2 : formation par un artisan, apprentissage d'outils/techniques d'assemblage.
- Acte 3 : réorganisation atelier + modèle de fabrication, focus sur design et spécificités client.

### 11.3 Ajustement important : artisan ≠ industriel
- Didier recadre :
  - un artisan ne fait pas de l'industriel,
  - meilleure formulation : "on a arrêté de réinventer la chaise, on a conçu un modèle de fabrication de chaises."
- Tu assumes que dans l'analogie Didier joue le rôle du "maître artisan" (même si pas maître absolu), et "l'élève" est l'équipe (le collectif décide de l'appropriation).

### 11.4 Mapping analogique exploré
- QA : test final / validation client (l'usage réel).
- Dépendances externes : éléments fournis par d'autres artisans/ateliers ; possibilité de montage à blanc/provisoire pour avancer.
- Goulot : avant = incertitude et contrôles fréquents ; après = validation/recette peut devenir le goulot.

### 11.5 Sensibilité "amateurisme"
- Didier exprime que "amateurisme" peut froisser.
- Alternatives proposées :
  - bricoleur,
  - fabricant,
  - menuisier appliqué,
  - ou formulation centrée sur le fait de "tester à la fin" plutôt que de juger les personnes.
- Pas de choix final tranché à ce stade.

---

## 12) Répartition des rôles Didier / Laure

### 12.1 Info nouvelle : Laure porte la continuité post-départ
- Laure est encore chez Alptis.
- Elle observe la suite de l'impact après ton départ.
- Elle a débloqué du budget pour des formations.
- Organisation continue vers un template produit.
- Estimation donnée : en ~1 semaine, capacité de déployer un parcours "exploitable à 70%" (hors services externes).

### 12.2 Répartition naturelle des rôles
- La complémentarité des profils dessine une répartition logique :
  - Didier : impulsion craft, structuration, démonstration des pivots techniques.
  - Laure : ancrage organisationnel, continuité et résultats post-départ.
- Cette répartition est une proposition de départ — à affiner pour équilibrer la présentation en duo.

---

## 13) Livrables produits pendant la conversation (capitalisation)
- Création/mises à jour du journal `REX_Lyon_Craft_Journal.md` (+ v2).
- Document d'avancement pour Laure (markdown puis PDF), puis version plus verbeuse.
- Synthèses PDF :
  - version structurée,
  - version narrative & stratégique.

---

## 14) Décisions / formulations à retenir (liste consolidée)

### 14.1 Thèses / formules structurantes
- **"Pour aller plus vite, il faut apprendre à livrer sûr."**
- **"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."**
- **"Le goulot s'est déplacé : du développement vers la recette/validation."**

### 14.2 Conclusion assumée
- **"Développer est un métier. Être artisan développeur en est un autre."**

### 14.3 Pivot complet (acte 3) — éléments incontournables
- Capture de l'intention (tests).
- Structure de code (découplage, lisibilité, refacto, patterns).
- Autonomie vis-à-vis des dépendances (simulation/mocks configurables).
- Rapprochement métier/DSI (co-conception pour faisabilité et time-to-market).

---

## 15) Points ouverts / à trancher plus tard
- Choix final du vocabulaire d'ouverture (éviter "amateur" sans édulcorer).
- Placement exact des punchlines et du niveau de provocation (ton, silence, posture).
- Découpage final en diapos + notes orales associées (ce document est une base de trace, pas encore un plan slide-by-slide).
- Arbitrage public vs interne : quels détails/mesures/chiffres peuvent être cités publiquement.

---

## 16) Comment utiliser ce document pour construire talk + slides + discours

1. **Surligner** :
   - phrases fortes,
   - anecdotes "ah OK",
   - pivots,
   - contraintes / limites (pour crédibilité).

2. **Transformer en plan de talk** :
   - ouverture (analogie),
   - acte 1 / acte 2 / acte 3,
   - conclusion (punchline).

3. **Décliner en support** :
   - 1 idée / slide,
   - notes orales associées.

4. **Dériver une version "alignment Laure"** :
   - ce qu'elle dit, ce que Didier dit, et les transitions.
