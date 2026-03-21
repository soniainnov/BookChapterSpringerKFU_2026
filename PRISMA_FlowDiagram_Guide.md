# PRISMA 2020 Flow Diagram — Guide de création manuelle

**Chapitre :** A Systematic Review of IoT-Enabled Smart Agriculture for Food Security and Sustainable Development
**Référence dans le texte :** Fig. 1
**Standard :** PRISMA 2020 (Page et al., 2021)

---

## Structure du diagramme (4 étapes)

Le diagramme PRISMA 2020 se lit de haut en bas et comporte **2 colonnes** :
- Colonne gauche : **Identification via bases de données**
- Colonne droite : **Identification via autres sources** (citation tracking)

Puis les étapes fusionnent en une colonne centrale pour Screening → Eligibility → Included.

---

## Contenu exact de chaque boîte

### ── ÉTAPE 1 : IDENTIFICATION ──────────────────────────────────

#### Boîte 1A (colonne gauche)
```
Records identified from databases
(IEEE Xplore, Scopus, Web of Science,
ACM Digital Library, Google Scholar)

n = 1,247
```

#### Boîte 1B (colonne droite)
```
Records identified through
manual backward citation tracking
of highly cited reviews

n = 34
```

#### Boîte 1C — Doublons supprimés (entre 1A+1B et Screening)
```
Duplicate records removed

n = 312
```

---

### ── ÉTAPE 2 : SCREENING ────────────────────────────────────────

#### Boîte 2A — Entrée du Screening
```
Records screened
(title and abstract)

n = 969
```

#### Boîte 2B — Exclus (à droite, flèche vers la droite)
```
Records excluded
(irrelevant to review scope)

n = 743
```

---

### ── ÉTAPE 3 : ELIGIBILITY ──────────────────────────────────────

#### Boîte 3A — Texte intégral évalué
```
Full-text articles assessed
for eligibility

n = 226
```

#### Boîte 3B — Exclus avec raisons (à droite, flèche vers la droite)
```
Full-text articles excluded  n = 139

Reasons:
  • Insufficient IoT content         n = 47
  • No developing country context    n = 52
  • Purely theoretical (no application) n = 28
  • Non-English language             n = 12
```

---

### ── ÉTAPE 4 : INCLUDED ─────────────────────────────────────────

#### Boîte 4A — Corpus final
```
Studies included in
qualitative synthesis

n = 87
```

---

## Flux des flèches

```
[1A: n=1,247]  [1B: n=34]
      │               │
      └───────┬────────┘
              ▼
   [Duplicates removed: n=312]
              │
              ▼
   [2A: Screened n=969] ──────► [2B: Excluded n=743]
              │
              ▼
   [3A: Full-text n=226] ──────► [3B: Excluded n=139
              │                    • IoT insuffisant: 47
              │                    • Pas pays dev.: 52
              │                    • Théorique: 28
              │                    • Non-anglais: 12]
              ▼
   [4A: Included n=87]
```

---

## Recommandations pour la création

### Outils recommandés
| Outil | Lien | Gratuit |
|-------|------|---------|
| **PRISMA Flow Diagram Generator** (officiel) | https://www.prisma-statement.org/prismastatement/flowdiagram | ✅ |
| draw.io / diagrams.net | https://app.diagrams.net | ✅ |
| Lucidchart | https://www.lucidchart.com | freemium |
| PowerPoint / Word SmartArt | — | ✅ (si Office dispo) |

### Outil le plus rapide : PRISMA Flow Diagram Generator officiel
1. Aller sur https://www.prisma-statement.org/prismastatement/flowdiagram
2. Sélectionner **PRISMA 2020**
3. Remplir les champs avec les chiffres ci-dessus
4. Exporter en **PNG haute résolution** ou **SVG**
5. Insérer dans le fichier Word comme figure

---

## Format pour insertion dans le document Word

- **Légende sous la figure :** `Fig. 1. PRISMA 2020 flow diagram of the study selection process.`
- **Style Word à utiliser :** `figurecaption`
- **Résolution minimale :** 300 DPI (requis Springer)
- **Format accepté :** EPS, PDF, TIFF, PNG (Springer préfère EPS ou PDF vectoriel)
- **Ne pas utiliser** d'image générée par IA (politique Springer)

---

## Chiffres de cohérence à vérifier

| Calcul | Résultat attendu |
|--------|-----------------|
| 1,247 + 34 = | **1,281** records total identifiés |
| 1,281 − 312 = | **969** records screened ✅ |
| 969 − 743 = | **226** full-text évalués ✅ |
| 226 − 139 = | **87** études incluses ✅ |
| 47 + 52 + 28 + 12 = | **139** exclusions eligibility ✅ |

Tous les chiffres sont cohérents.
