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

### Base commune (à ajouter au début de chaque prompt)

```
Style : illustration en trait simple, type mini BD, peu de détails.
Palette chaude : indigo foncé (#0d1b2a), sable (#e6d5b8), or (#d4a03c).
Fond sombre. Pas de texte dans l'image.
Motifs géométriques africains/caraïbéens discrets en bordure.
Format 16:9.
```

### Slide 1 — L'atelier (avant)

```
[BASE COMMUNE]
Un atelier de menuiserie faiblement éclairé. Un artisan vient de
s'asseoir sur une chaise qu'il a fabriquée. La chaise craque sous lui.
Expression de surprise résignée. Outils dispersés sur l'établi.
Ambiance : routine, fatalité — pas de drame.
```

### Slide 10 — L'atelier (apprentissage)

```
[BASE COMMUNE]
Même atelier de menuiserie, un peu plus lumineux. Un maître artisan
montre une technique d'assemblage tenon-mortaise à un apprenti.
L'apprenti tient les outils avec hésitation mais concentration.
Les outils sont mieux rangés sur l'établi qu'avant.
Ambiance : transmission, effort, pas encore de maîtrise.
```

### Slide 14 — L'atelier (transformé)

```
[BASE COMMUNE]
Même atelier de menuiserie, bien éclairé et organisé. Sur l'établi,
un gabarit/patron de fabrication. L'artisan personnalise une chaise
avec confiance et précision. Plusieurs chaises terminées en
arrière-plan, chacune légèrement différente.
Ambiance : maîtrise, sérénité, fierté calme.
```
