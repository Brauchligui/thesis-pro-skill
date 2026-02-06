# Analyse Sectorielle - Étape 2: Analyse Macro (PESTEL)

## VOTRE TÂCHE:

Conduire une analyse PESTEL du secteur via recherche web.

## SÉQUENCE:

### 1. Lancer les Recherches

"Je vais conduire une **analyse PESTEL** pour le secteur **{{sector}}** en **{{geography}}**.

**Recherches en cours...**"

### 2. Recherches Parallèles

```
Recherche web: "{{sector}} {{geography}} political factors regulation"
Recherche web: "{{sector}} economic outlook growth"
Recherche web: "{{sector}} social trends consumer behavior"
Recherche web: "{{sector}} technology innovation digital"
Recherche web: "{{sector}} environmental sustainability ESG"
Recherche web: "{{sector}} legal compliance regulations"
```

### 3. Documenter l'Analyse PESTEL

```markdown
## Analyse PESTEL: {{sector}}

### P - Politique
**Facteurs identifiés:**
- [Facteur 1]: [Impact sur le secteur]
- [Facteur 2]: [Impact]

**Sources:** [URLs]

### E - Économique
**Indicateurs clés:**
- Taille du marché: [X] Mds €
- Croissance: [X]% CAGR
- Tendance: [Croissance/Stagnation/Déclin]

**Facteurs économiques:**
- [Facteur 1]
- [Facteur 2]

### S - Sociologique
**Tendances sociétales:**
- [Tendance 1]
- [Tendance 2]

**Évolutions comportementales:**
- [Évolution 1]

### T - Technologique
**Innovations majeures:**
- [Innovation 1]
- [Innovation 2]

**Niveau de digitalisation:** [Évaluation]

### E - Écologique
**Enjeux environnementaux:**
- [Enjeu 1]
- [Enjeu 2]

**Initiatives RSE/ESG:** [Description]

### L - Légal
**Cadre réglementaire:**
- [Réglementation 1]
- [Réglementation 2]

**Évolutions réglementaires attendues:**
- [Évolution 1]
```

### 4. Continuer

"[C] Continuer — Analyse concurrentielle (Porter)"

#### Si 'C':
- Charger: `./step-03-porter.md`
