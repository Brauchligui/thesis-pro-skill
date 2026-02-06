# Recherche d'Études - Étape 3: Méta-Analyses et Revues Systématiques

## RÈGLES D'EXÉCUTION OBLIGATOIRES:

- 🛑 NE JAMAIS générer du contenu sans recherche web
- ✅ Rechercher les MÉTA-ANALYSES et REVUES SYSTÉMATIQUES
- 📋 Ces sources sont CRUCIALES car elles synthétisent la littérature
- 🔍 RECHERCHE WEB REQUISE
- 📝 ÉCRIRE LES RÉSULTATS IMMÉDIATEMENT
- ✅ TOUJOURS communiquer dans `{communication_language}`

## VOTRE TÂCHE:

Identifier les méta-analyses et revues systématiques sur {{research_topic}}.

## SÉQUENCE DE RECHERCHE:

### 1. Lancer la Recherche

"Je recherche maintenant les **méta-analyses et revues systématiques** sur **{{research_topic}}**.

**Pourquoi ces sources sont précieuses:**
- Elles synthétisent des dizaines/centaines d'études
- Elles offrent une vue d'ensemble du champ
- Elles identifient les résultats robustes vs inconsistants
- Elles pointent les gaps de recherche

**Je lance les recherches...**"

### 2. Exécution de Recherche Parallèle

```
Recherche web: "{{research_topic}} meta-analysis"
Recherche web: "{{research_topic}} systematic review"
Recherche web: "{{research_topic}} literature review comprehensive"
Recherche web: "{{research_topic}} revue systématique méta-analyse"
Recherche web: "{{research_topic}} state of the art review"
```

### 3. Analyser les Résultats

Pour chaque méta-analyse/revue trouvée:

```markdown
## Méta-Analyses et Revues Systématiques

### Méta-Analyse 1: [Titre]

**Référence complète ({{citation_style}}):**
[Citation formatée]

**Type:** Méta-analyse quantitative / Revue systématique / Revue narrative

**Périmètre:**
- Nombre d'études incluses: [X]
- Période couverte: [années]
- Bases de données consultées: [liste]
- Critères d'inclusion: [résumé]

**Questions de recherche:**
[Questions auxquelles la revue répond]

**Résultats principaux:**
1. [Résultat 1 avec taille d'effet si applicable]
2. [Résultat 2]
3. [Résultat 3]

**Conclusions des auteurs:**
"[Citation clé des conclusions]"

**Limites identifiées par les auteurs:**
- [Limite 1]
- [Limite 2]

**Recommandations pour recherches futures:**
- [Recommandation 1]
- [Recommandation 2]

**Pertinence pour votre thèse:**
[Comment cette revue informe votre recherche]

---

### Tableau des Méta-Analyses

| Auteur(s) | Année | Type | N études | Focus | Conclusion principale |
|-----------|-------|------|----------|-------|----------------------|
| [Nom] | [An] | Méta | [X] | [Focus] | [Conclusion] |
| [Nom] | [An] | Syst | [X] | [Focus] | [Conclusion] |

### Synthèse des Méta-Analyses

**Points de convergence:**
[Ce sur quoi les méta-analyses s'accordent]

**Points de divergence:**
[Résultats contradictoires entre revues]

**Gaps identifiés par les revues:**
[Ce que les revues identifient comme manquant]
```

### 4. Présenter et Continuer

"J'ai identifié **[X] méta-analyses et revues systématiques** sur {{research_topic}}.

**Résultats:**
- ✅ [X] revues systématiques identifiées
- ✅ Périmètres et conclusions documentés
- ✅ Gaps identifiés par les revues repérés
- ✅ Tableau récapitulatif créé

[C] Continuer — Rechercher les études empiriques récentes
[A] Approfondir — Explorer d'autres revues"

#### Si 'C':
- Mettre à jour: `stepsCompleted: [1, 2, 3]`
- Charger: `./step-04-recent-empirical.md`
