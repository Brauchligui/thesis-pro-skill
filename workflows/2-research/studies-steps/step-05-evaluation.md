# Recherche d'Études - Étape 5: Évaluation et Sélection

## RÈGLES D'EXÉCUTION OBLIGATOIRES:

- 🛑 NE PAS ajouter de nouvelles études à cette étape
- ✅ ÉVALUER la qualité des études identifiées
- 📋 Appliquer des critères de qualité rigoureux
- 🔍 Identifier les études les plus pertinentes pour la thèse
- 📝 CRÉER une sélection priorisée
- ✅ TOUJOURS communiquer dans `{communication_language}`

## VOTRE TÂCHE:

Évaluer la qualité des études identifiées et créer une sélection priorisée.

## SÉQUENCE D'ÉVALUATION:

### 1. Présenter les Critères d'Évaluation

"Je vais maintenant **évaluer la qualité** des études identifiées sur **{{research_topic}}**.

**Critères d'Évaluation:**

| Critère | Description | Poids |
|---------|-------------|-------|
| **Crédibilité** | Journal peer-reviewed, auteur reconnu | ⭐⭐⭐ |
| **Rigueur** | Méthodologie claire et solide | ⭐⭐⭐ |
| **Pertinence** | Alignement avec votre recherche | ⭐⭐⭐ |
| **Actualité** | Date de publication | ⭐⭐ |
| **Impact** | Nombre de citations | ⭐⭐ |
| **Accessibilité** | Disponibilité du texte intégral | ⭐ |"

### 2. Évaluer Chaque Étude

```markdown
## Évaluation des Études

### Grille d'Évaluation

| Étude | Crédibilité | Rigueur | Pertinence | Actualité | Impact | Score |
|-------|-------------|---------|------------|-----------|--------|-------|
| [Étude 1] | 5/5 | 4/5 | 5/5 | 3/5 | 5/5 | 22/25 |
| [Étude 2] | 4/5 | 5/5 | 4/5 | 5/5 | 3/5 | 21/25 |
| [Étude 3] | 5/5 | 4/5 | 3/5 | 4/5 | 4/5 | 20/25 |

### Alertes Qualité

**Études à utiliser avec précaution:**
- [Étude X]: [Raison - ex: échantillon petit, biais potentiel]

**Journaux prédateurs détectés:**
- [Si applicable]

### Sélection Finale

#### Études Incontournables (Score ≥ 20)
1. [Étude] — [Justification courte]
2. [Étude] — [Justification]

#### Études Recommandées (Score 15-19)
1. [Étude] — [Justification]
2. [Étude] — [Justification]

#### Études Complémentaires (Score < 15)
1. [Étude] — [Usage limité recommandé]

### Classification par Usage

**Pour la définition des concepts:**
- [Étude 1], [Étude 2]

**Pour le cadre théorique:**
- [Étude 3], [Étude 4]

**Pour la méthodologie:**
- [Étude 5]

**Pour la discussion des résultats:**
- [Étude 6], [Étude 7]
```

### 3. Présenter et Continuer

"J'ai **évalué [X] études** sur {{research_topic}}.

**Résultats:**
- ✅ [X] études incontournables identifiées
- ✅ [X] études recommandées
- ✅ Classification par usage créée
- ✅ Alertes qualité documentées

[C] Continuer — Créer les fiches de lecture synthétiques
[R] Réviser — Revoir l'évaluation de certaines études"

#### Si 'C':
- Mettre à jour: `stepsCompleted: [1, 2, 3, 4, 5]`
- Charger: `./step-06-synthesis.md`
