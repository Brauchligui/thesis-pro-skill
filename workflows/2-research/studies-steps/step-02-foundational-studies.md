# Recherche d'Études - Étape 2: Études Fondatrices

## RÈGLES D'EXÉCUTION OBLIGATOIRES:

- 🛑 NE JAMAIS générer du contenu sans recherche web
- ✅ Rechercher les études FONDATRICES qui ont défini le champ
- 📋 VOUS ÊTES UN HISTORIEN DE LA RECHERCHE
- 🔍 RECHERCHE WEB REQUISE - trouver les classiques
- 📝 ÉCRIRE LES RÉSULTATS IMMÉDIATEMENT
- ✅ TOUJOURS communiquer dans `{communication_language}`

## VOTRE TÂCHE:

Identifier les études fondatrices et séminales sur {{research_topic}}.

## SÉQUENCE DE RECHERCHE:

### 1. Lancer la Recherche

"Je recherche maintenant les **études fondatrices** sur **{{research_topic}}**.

**Ce que je cherche:**
- Articles séminaux qui ont introduit les concepts clés
- Ouvrages de référence incontournables
- Études qui ont établi le paradigme de recherche
- Auteurs fondateurs du champ

**Je lance les recherches...**"

### 2. Exécution de Recherche Parallèle

```
Recherche web: "{{research_topic}} seminal paper foundational"
Recherche web: "{{research_topic}} original study pioneer"
Recherche web: "{{research_topic}} classic study landmark"
Recherche web: "{{research_topic}} first study introduced"
Recherche web: "who coined {{research_topic}} term origin"
```

### 3. Analyser les Résultats

Pour chaque étude fondatrice trouvée, documenter:

```markdown
## Études Fondatrices Identifiées

### Étude 1: [Titre]

**Référence complète ({{citation_style}}):**
[Citation formatée]

**Auteur(s):** [Nom(s)]
**Année:** [Année]
**Type:** Article / Livre / Chapitre

**Contribution fondatrice:**
[Ce que cette étude a introduit/établi]

**Nombre de citations:** [X] (Google Scholar)

**Pourquoi c'est fondateur:**
- [Raison 1]
- [Raison 2]

**Concepts clés introduits:**
- [Concept 1]
- [Concept 2]

**Citation clé:**
"[Citation importante de l'étude]"

**À citer pour:**
[Dans quelle partie de la thèse utiliser cette source]

---

### Étude 2: [Titre]
[Structure identique]

---

### Tableau Récapitulatif des Études Fondatrices

| Auteur | Année | Titre | Contribution | Citations |
|--------|-------|-------|--------------|-----------|
| [Nom] | [An] | [Titre court] | [Contribution] | [X] |
```

### 4. Présenter et Continuer

"J'ai identifié **[X] études fondatrices** sur {{research_topic}}.

**Résultats:**
- ✅ [X] articles séminaux identifiés
- ✅ Auteurs fondateurs documentés
- ✅ Citations clés extraites
- ✅ Tableau récapitulatif créé

[C] Continuer — Rechercher les méta-analyses et revues systématiques
[A] Approfondir — Explorer d'autres études fondatrices"

#### Si 'C':
- Mettre à jour: `stepsCompleted: [1, 2]`
- Charger: `./step-03-meta-analyses.md`

## ÉTAPE SUIVANTE:

Charger `./step-03-meta-analyses.md` pour rechercher les méta-analyses.
