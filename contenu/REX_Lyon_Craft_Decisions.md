# Points ouverts tranchés — REX Lyon Craft

> Livrables des étapes 3 et 4.
> Décisions finales sur les éléments encore flous avant la rédaction des notes orales.
> Direction créative du support (étape 4).

---

## 1. Vocabulaire d'ouverture

**Question** : Éviter le mot "amateur" sans édulcorer le propos.

**Décision** : Résolu par l'audit (étape D). L'ouverture ne parle plus d'"amateur". Elle dit : *"Ce n'est pas de la négligence — c'est comme ça qu'on a toujours fait."* Constat sans jugement, pas d'accusation.

---

## 2. Placement et niveau de provocation de la conclusion

**Question** : La punchline *"Développer est un métier. Être artisan développeur en est un autre."* est-elle au bon niveau pour Lyon Craft ?

**Décision** : Validée en l'état. Le public Lyon Craft se définit comme craftsmen — la phrase valide et élève leur identité, elle ne les attaque pas. Le placement (slide 14, après l'analogie bouclée, avec un silence avant) garantit l'impact émotionnel.

---

## 3. Arbitrage public/interne sur les éléments citables

**Question** : Quels noms, chiffres et détails sont citables publiquement ?

**Décision** (validée avec Laure) :

| Élément | Citable ? |
|---------|-----------|
| Nom "Alptis" | Oui |
| Noms de produits (Select, Protect, Select Pro, SFR, Santé Équilibre) | Oui |
| Chiffres (6-7 mois, 7 mois, 2 mois, 150j/200j) | Oui |
| Migration Java 11 → 21 | Oui |
| Budget DSI 2026 | Oui |
| Nom du prestataire de formation TDD | Non — retiré des livrables |

---

## 4. Titre du talk

**Titre** : *Et Craft la chaise*
**Sous-titre** : *REX Alptis — Le TDD, un vrai gain de temps*

Jeu de mots sur "Et paf le chien" — référence connue du public tech français. Ancre le fil rouge menuiserie dès le titre. Le sous-titre apporte le factuel.

---

## 5. Logo

**Logo retenu** : Alptis blanc classique (SVG) — `support/assets/logo-alptis-white.svg`
Adapté aux fonds sombres de la palette indigo.

---

## 6. Palette et typographie

**Palette :**

| Rôle | Couleur | Hex |
|------|---------|-----|
| Fond principal | Indigo foncé | `#0d1b2a` |
| Fond accentué (transitions d'actes) | Indigo moyen | `#1a1a2e` |
| Texte principal | Sable clair | `#e6d5b8` |
| Accents / chiffres clés | Or chaud | `#d4a03c` |
| Citations / formulations clés | Blanc pur | `#ffffff` |

**Typographie :**
- Titres : Montserrat (bold, géométrique, moderne)
- Corps : Source Sans Pro (lisibilité, inclus dans reveal.js)

**Motif afro-caraïbéen** : pattern géométrique subtil (lignes, triangles) en filigrane sur les slides de transition d'actes. Format SVG ou CSS.

---

## 7. Stratégie visuels par slide

### Slides "typo forte" (le texte est le visuel)
- **Slide 4** (La norme) : chiffres en grand, or sur indigo
- **Slide 5** (Formulation clé) : citation seule, fond accentué
- **Slide 9** (7 mois) : "7 mois" en très grand, or sur indigo
- **Slide 12** (Santé Équilibre) : "2 mois" + "+ 1 mois" en très grand
- **Slide 14** (Punchline) : citation finale, fond sombre, silence visuel

### Slides avec schéma (SVG/CSS dans reveal)
- **Slide 2** (La douleur) : boucle dev ↔ recette, flèches circulaires
- **Slide 8** (Ce qui se passe vraiment) : frise horizontale des 4 phases
- **Slide 13** (Template) : schéma bloc central → déclinaisons produits

### Slides avec illustration (mini BD, générée par IA)
- **Slide 1** (L'atelier — avant) : l'atelier sombre, la chaise qui craque
- **Slide 10** (L'apprentissage) : même atelier, le maître montre les techniques
- **Slide 14** (L'atelier transformé) : même atelier, lumineux, organisé

### Slides avec icônes minimalistes
- **Slide 6** (Le pari SFR) : page blanche / fondation
- **Slide 7** (Ce qu'on met en place) : une icône par levier
- **Slide 11** (Le renversement) : flèche inversée / déclic

### Slides avec photos (à fournir)
- **Slide 3** (Qui sommes-nous) : photos Didier et Laure

---

## 8. Prompts de génération d'images (mini BD)

Outil recommandé : **Midjourney** (cohérence de style) ou **DALL-E 3 / ChatGPT** (simplicité).

Chaque mini BD est une planche de 3 ou 4 vignettes. Narration 100% visuelle — aucun texte, aucune bulle, aucune légende. L'histoire se raconte par les gestes, les expressions et la composition.

### Base commune (à ajouter au début de chaque prompt)

```
Style : mini bande dessinée en trait simple, type BD franco-belge épurée.
Peu de détails, traits expressifs, narration visuelle uniquement.
Aucun texte, aucune bulle, aucune onomatopée, aucune légende.
Format 16:9, vignettes séparées par des bordures nettes.
Couleurs libres — palette chaleureuse et lisible.
Le même personnage principal (menuisière, femme, tablier de travail)
apparaît dans les 3 planches — elle doit être reconnaissable.
```

### Slide 1 — "Ça craque" (4 vignettes)

Scénario : le quotidien d'avant — on fabrique, on teste à la fin, ça casse, on recommence. Ton comique, pas tragique.

```
[BASE COMMUNE]
Planche de 4 vignettes, lue de gauche à droite :
1. Une menuisière dans son atelier termine une chaise. Elle essuie
   la sueur, l'air satisfait de son travail. Outils dispersés
   sur l'établi, atelier un peu désordonné.
2. Elle s'assoit sur la chaise, sourire confiant, les bras croisés
   fièrement.
3. La chaise cède sous elle — elle se retrouve par terre, les pieds
   en l'air, entourée de morceaux de bois. Expression de surprise.
4. Elle se relève, épousette son tablier, retourne vers l'établi
   avec un air résigné. Elle a l'habitude. Pas de colère — de la
   lassitude.
```

### Slide 10 — "L'apprentissage" (3 vignettes)

Scénario : le maître a montré les techniques, l'apprenti essaye. C'est prometteur mais pas encore abouti. Ton bienveillant.

```
[BASE COMMUNE]
Planche de 3 vignettes, lue de gauche à droite :
1. Une maître artisane métisse montre une technique d'assemblage
   tenon-mortaise à la menuisière (même personnage que planche 1,
   dans le rôle de l'apprentie). Son geste est précis et assuré.
   Elle tient les pièces de bois avec aisance.
2. La menuisière/apprentie essaye à son tour — concentration
   intense, langue tirée, geste hésitant. Elle tient les outils
   maladroitement mais avec détermination. La maître artisane
   observe en retrait.
3. Le joint tient, mais c'est brut et imparfait. L'apprentie
   regarde la maître artisane, mi-fière mi-inquiète. La maître
   artisane hoche la tête avec un léger sourire d'approbation.
   Les outils sont mieux rangés sur l'établi qu'avant.
```

### Slide 14 — "L'atelier transformé" (4 vignettes)

Scénario : même atelier, même menuisier, mais tout a changé — organisation, confiance, maîtrise. Le contraste avec la planche 1 doit être frappant. Ton calme et serein.

```
[BASE COMMUNE]
Planche de 4 vignettes, lue de gauche à droite :
1. Même atelier que la planche 1, mais lumineux, rangé, organisé.
   Un gabarit/patron de fabrication bien visible sur l'établi.
   Les outils sont à leur place.
2. La menuisière pose une chaise sur le gabarit, vérifie les
   alignements — tout est parfait. Son geste est détendu et précis.
3. Un client entre dans l'atelier avec un croquis/dessin d'une
   chaise personnalisée. La menuisière regarde le croquis et fait
   un pouce levé, confiante.
4. Vue large de l'atelier : plusieurs chaises terminées en
   arrière-plan, chacune légèrement différente (formes, dossiers)
   mais toutes solides et bien finies. La menuisière au centre,
   bras croisés, sereine.
```
