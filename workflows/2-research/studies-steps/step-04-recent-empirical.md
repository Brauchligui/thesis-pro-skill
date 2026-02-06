# Recherche d'Études - Étape 4: Études Empiriques Récentes

## RÈGLES D'EXÉCUTION OBLIGATOIRES:

- 🛑 NE JAMAIS générer du contenu sans recherche web
- ✅ Rechercher les études empiriques des 5 DERNIÈRES ANNÉES
- 📋 Prioriser les études peer-reviewed récentes
- 🔍 RECHERCHE WEB REQUISE
- 📝 ÉCRIRE LES RÉSULTATS IMMÉDIATEMENT
- ✅ TOUJOURS communiquer dans `{communication_language}`

## VOTRE TÂCHE:

Identifier les études empiriques récentes (2020-2025) sur {{research_topic}}.

## SÉQUENCE DE RECHERCHE:

### 1. Lancer la Recherche

"Je recherche maintenant les **études empiriques récentes** sur **{{research_topic}}**.

**Ce que je cherche:**
- Études quantitatives récentes (2020-2025)
- Études qualitatives récentes
- Études mixtes
- Nouvelles méthodologies utilisées

**Je lance les recherches...**"

### 2. Exécution de Recherche Parallèle

```
Recherche web: "{{research_topic}} empirical study 2024"
Recherche web: "{{research_topic}} research findings 2023 2024"
Recherche web: "{{research_topic}} quantitative study recent"
Recherche web: "{{research_topic}} qualitative research 2023"
Recherche web: "{{research_topic}} étude empirique récente"
```

### 3. Analyser les Résultats

```markdown
## Études Empiriques Récentes (2020-2025)

### Études Quantitatives

#### Étude Q1: [Titre] (Auteur, Année)

**Référence ({{citation_style}}):**
[Citation]

**Objectif:** [Objectif de l'étude]

**Méthodologie:**
- Design: [expérimental, corrélationnel, etc.]
- Échantillon: N = [X], [caractéristiques]
- Variables: [VI, VD, contrôles]
- Analyse: [méthodes statistiques]

**Résultats clés:**
- [Résultat 1 avec valeur p/effet]
- [Résultat 2]

**Implications:** [Ce que ça signifie]

**Limites:** [Limites reconnues]

---

### Études Qualitatives

#### Étude QL1: [Titre] (Auteur, Année)

**Référence:** [Citation]

**Objectif:** [Objectif]

**Méthodologie:**
- Approche: [phénoménologique, grounded theory, etc.]
- Participants: N = [X], [caractéristiques]
- Collecte: [entretiens, observation, etc.]
- Analyse: [thématique, IPA, etc.]

**Thèmes principaux:**
1. [Thème 1]
2. [Thème 2]
3. [Thème 3]

**Contribution:** [Apport au champ]

---

### Études Mixtes

[Si applicable, même structure]

---

### Tableau des Études Récentes

| Auteur | Année | Type | N | Contexte | Résultat principal |
|--------|-------|------|---|----------|-------------------|
| [Nom] | 2024 | Quanti | 500 | [ctx] | [résultat] |
| [Nom] | 2023 | Quali | 25 | [ctx] | [résultat] |

### Tendances Méthodologiques Récentes

**Approches innovantes observées:**
- [Nouvelle méthode 1]
- [Nouvelle méthode 2]

**Contextes émergents:**
- [Nouveau contexte de recherche]
```

### 4. Présenter et Continuer

"J'ai identifié **[X] études empiriques récentes** sur {{research_topic}}.

**Résultats:**
- ✅ [X] études quantitatives
- ✅ [X] études qualitatives
- ✅ Méthodologies et résultats documentés
- ✅ Tendances récentes identifiées

[C] Continuer — Évaluer et sélectionner les études clés
[A] Approfondir — Chercher plus d'études récentes"

#### Si 'C':
- Mettre à jour: `stepsCompleted: [1, 2, 3, 4]`
- Charger: `./step-05-evaluation.md`
