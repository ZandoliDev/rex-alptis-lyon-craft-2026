# Plan d'action — REX Lyon Craft

> Document de référence partagé entre toutes les conversations du projet.  
> Chaque étape produit un livrable `.md` à ajouter au projet avant de passer à la suivante.

---

## Contexte clé à ne jamais perdre de vue

- **Format** : Talk REX en duo (Didier + Laure) — public Lyon Craft (initié craft)
- **Angle** : Pas "comment faire du craft" mais "comment convaincre" et "quel impact organisationnel"
- **Chiffres structurants** :
  - Avant : 1 produit = 6 à 7 mois / équipe de 4 à 5 personnes (PO, SA, 3 dev)
  - Produit 1 (craft from scratch) : 7 mois
  - Produit 2 (duplication craft) : 2 mois
- **Thèses retenues** :
  - *"Pour aller plus vite, il faut apprendre à livrer sûr."*
  - *"Quand le changement devient maîtrisé, l'industrialisation devient rationnelle."*
  - *"Le goulot s'est déplacé : du développement vers la recette/validation."*
- **Conclusion assumée** : *"Développer est un métier. Être artisan développeur en est un autre."*
- **Fil rouge** : analogie menuiserie (ouvre, traverse et ferme le talk)
- **Positionnement duo** : Didier = impulsion craft / structuration / démonstration. Laure = contexte / continuité / stratégie post-départ.

---

## Structure narrative du talk (3 actes)

| Acte | Titre provisoire | Idée centrale | Chiffre clé |
|------|-----------------|---------------|-------------|
| 0 | Ouverture | Analogie menuiserie — l'atelier avant | — |
| 1 | L'héritage | Travailler sur un existant sans filet | 6-7 mois / produit |
| 2 | L'expérimentation | Repartir de zéro avec le craft | 7 mois (produit 1) |
| 3 | L'industrialisation | Quand maîtrise = levier | 2 mois (produit 2) |
| 4 | Conclusion | Punchline + analogie de fermeture | — |

---

## Étapes de travail

### Étape 1 — Intégrer les chiffres dans la trame narrative
**Objectif** : Positionner les durées (6-7 mois → 6 mois → 2 mois) comme fil rouge visible de la narration. Qualifier chaque chiffre (contexte, équipe, périmètre) pour qu'il soit indiscutable en salle.  
**Livrable** : `REX_Lyon_Craft_Trame_Narrative.md`  
**Statut** : ✅ Fait

---

### Étape 2 — Plan slide-by-slide
**Objectif** : Produire le squelette complet du talk : titre de chaque slide, idée centrale, donnée ou anecdote associée, répartition Didier / Laure.  
**Dépend de** : Étape 1  
**Livrable** : `REX_Lyon_Craft_Plan_Slides.md`  
**Statut** : ✅ Fait

---

### Étape 3 — Trancher les points ouverts
**Objectif** : Décisions finales sur les éléments encore flous.
- Vocabulaire d'ouverture (éviter "amateur" sans édulcorer)
- Placement et niveau de provocation de la conclusion
- Arbitrage public/interne sur les chiffres et détails citables

**Dépend de** : Étape 2  
**Livrable** : `REX_Lyon_Craft_Decisions.md`
**Statut** : ✅ Fait

---

### Étape 4 — Direction créative du support
**Objectif** : Définir l'identité visuelle et le titre du talk avant de produire le support final.
- Titre du talk : trouver une accroche qui intrigue, donne envie — pas un titre descriptif
- Logo Alptis : récupérer et intégrer
- Visuels : stratégie images (photos, illustrations, créations) pour chaque slide
- Palette et typo : affiner l'identité indigo–sable, motif afro-caraïbéen discret

**Dépend de** : Étape 3
**Livrable** : décisions intégrées dans `REX_Lyon_Craft_Decisions.md`
**Statut** : 🔲 À faire

---

### Étape 5 — Notes speaker par slide
**Objectif** : Pour chaque slide, lister les points à dire à l'oral (aide-mémoire, pas un script). Indiquer qui parle et les transitions Didier ↔ Laure.
**Dépend de** : Étapes 2 et 3
**Livrable** : `REX_Lyon_Craft_Notes_Speaker.md`
**Statut** : 🔲 À faire

---

### Étape 6 — Support de présentation
**Objectif** : Créer le support visuel final (reveal-md → HTML autoporté, déployé via GitHub Pages).
- Contenu adapté à la projection : mots-clés, chiffres, citations — pas de paragraphes
- Notes speaker (étape 5)
- Identité visuelle et titre définis à l'étape 4
- Visuels intégrés

**Dépend de** : Étapes 4, 5
**Livrable** : `support/REX_Lyon_Craft.md` (source) + `support/dist/` (HTML autoporté)
**Statut** : 🚧 V1 brute en place, à refaire

---

## Livrables produits (à mettre à jour au fil des conversations)

| Fichier | Description | Statut |
|---------|-------------|--------|
| `REX_Lyon_Craft_Compte_Rendu.md` | Trace complète de la conversation initiale (ChatGPT) | ✅ Disponible dans le projet |
| `REX_Lyon_Craft_Plan_Action.md` | Ce document | ✅ Disponible dans le projet |
| `REX_Lyon_Craft_Trame_Narrative.md` | Trame avec chiffres intégrés | ✅ Disponible dans le projet |
| `REX_Lyon_Craft_Plan_Slides.md` | Plan slide-by-slide | ✅ Disponible dans le projet |
| `REX_Lyon_Craft_Decisions.md` | Points ouverts tranchés | ✅ Disponible dans le projet |
| `REX_Lyon_Craft_Notes_Speaker.md` | Notes speaker par slide | 🔲 |
| `support/REX_Lyon_Craft.md` | Support reveal-md (source) | 🚧 V1 brute |
| `support/dist/` | HTML autoporté (GitHub Pages) | 🚧 V1 brute |
