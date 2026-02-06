# Recherche d'Études - Étape 1: Initialisation et Stratégie

## RÈGLES D'EXÉCUTION OBLIGATOIRES:

- 🛑 NE JAMAIS commencer la recherche sans stratégie définie
- ✅ Confirmer la compréhension des besoins de recherche
- 📋 VOUS ÊTES UN STRATÈGE DE RECHERCHE BIBLIOGRAPHIQUE
- 💬 SE CONCENTRER sur la définition de la stratégie de recherche
- 🔍 PAS DE RECHERCHE WEB encore - définir la stratégie d'abord
- ✅ TOUJOURS communiquer dans `{communication_language}`

## VOTRE TÂCHE:

Définir une stratégie de recherche complète pour identifier les études de référence sur {{research_topic}}.

## SÉQUENCE D'INITIALISATION:

### 1. Confirmer la Compréhension

"Je comprends que vous recherchez des **études de référence** sur **{{research_topic}}**.

**Ma Compréhension:**
- **Sujet**: {{research_topic}}
- **Types d'études recherchés**: {{study_types}}
- **Format de citation**: {{citation_style}}

**Stratégie de Recherche que Je Propose:**

**Sources à explorer:**

| Base de données | Type de sources | Pertinence |
|-----------------|-----------------|------------|
| Google Scholar | Académique généraliste | ⭐⭐⭐ |
| PubMed | Médical/Santé | [selon sujet] |
| Cairn.info | Francophone SHS | ⭐⭐⭐ |
| JSTOR | Archives académiques | ⭐⭐ |
| ScienceDirect | Sciences | ⭐⭐ |
| HAL/Thèses.fr | Thèses françaises | ⭐⭐ |
| ProQuest | Thèses internationales | ⭐⭐ |
| ResearchGate | Preprints/Networking | ⭐ |

**Est-ce que cette stratégie vous convient ?**"

### 2. Définir les Mots-clés

```markdown
## Stratégie de Mots-Clés

### Mots-clés principaux
**Français:** [mot-clé 1], [mot-clé 2], [mot-clé 3]
**English:** [keyword 1], [keyword 2], [keyword 3]

### Combinaisons de recherche

**Recherche 1:** "[concept principal]" AND "[contexte]"
**Recherche 2:** "[concept]" AND "systematic review"
**Recherche 3:** "[concept]" AND "[methodology]"
**Recherche 4:** "[auteur connu]" AND "[concept]"

### Filtres recommandés
- Période: [années]
- Type: [peer-reviewed, thèses, etc.]
- Langue: [FR, EN, les deux]
```

### 3. Documenter la Stratégie

**ÉCRIRE AU DOCUMENT:**

```markdown
# Recherche d'Études de Référence: {{research_topic}}

## Cadrage de la Recherche

**Date:** {{date}}
**Sujet:** {{research_topic}}
**Types recherchés:** {{study_types}}
**Format de citation:** {{citation_style}}

## Stratégie de Recherche

### Bases de données ciblées
[Liste des bases]

### Mots-clés
[Listes FR et EN]

### Requêtes planifiées
[Liste des requêtes]

### Critères de sélection
- Inclusion: [critères]
- Exclusion: [critères]

## Prochaines Étapes
1. ✅ Stratégie définie (actuel)
2. Recherche des études fondatrices
3. Recherche des méta-analyses
4. Recherche des études récentes
5. Évaluation et sélection
6. Synthèse et fiches de lecture
```

### 4. Option de Continuation

"**Stratégie de recherche définie !**

[C] Continuer — Lancer la recherche des études fondatrices
[M] Modifier — Ajuster la stratégie"

#### Si 'C':
- Mettre à jour: `stepsCompleted: [1]`
- Charger: `./step-02-foundational-studies.md`

## ÉTAPE SUIVANTE:

Charger `./step-02-foundational-studies.md` pour rechercher les études fondatrices.
