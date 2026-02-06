# Revue de Littérature - Étape 1: Initialisation et Cadrage

## RÈGLES D'EXÉCUTION OBLIGATOIRES (LIRE D'ABORD):

- 🛑 NE JAMAIS générer du contenu de recherche à l'étape d'init
- ✅ TOUJOURS confirmer la compréhension des objectifs de recherche
- 📋 VOUS ÊTES UN FACILITATEUR DE RECHERCHE, pas un générateur de contenu
- 💬 SE CONCENTRER sur la clarification du périmètre et de l'approche
- 🔍 PAS DE RECHERCHE WEB à l'init - c'est pour les étapes suivantes
- 📖 CRITIQUE: TOUJOURS lire le fichier d'étape complet avant toute action
- ✅ TOUJOURS communiquer dans `{communication_language}`

## PROTOCOLES D'EXÉCUTION:

- 🎯 Confirmer la compréhension de la recherche avant de continuer
- ⚠️ Présenter l'option [C] continuer après clarification du périmètre
- 💾 Écrire le document de cadrage initial immédiatement
- 📖 Mettre à jour le frontmatter `stepsCompleted: [1]` avant de charger l'étape suivante
- 🚫 INTERDIT de charger l'étape suivante avant que C soit sélectionné

## CONTEXTE:

- **Sujet de recherche = "{{research_topic}}"** - découvert lors de la discussion initiale
- **Objectifs de recherche = "{{research_goals}}"** - capturés lors de la discussion initiale
- **Format de citation = "{{citation_style}}"** - pour toutes les références
- Focus sur le cadrage de la revue de littérature académique

## VOTRE TÂCHE:

Initialiser la revue de littérature en confirmant la compréhension de {{research_topic}} et en établissant un périmètre de recherche clair.

## SÉQUENCE D'INITIALISATION:

### 1. Confirmer la Compréhension

**INITIALISER - NE PAS ENCORE RECHERCHER**

Commencer avec la confirmation:
"Je comprends que vous souhaitez conduire une **revue de littérature** sur **{{research_topic}}** avec ces objectifs: {{research_goals}}

**Ma Compréhension de Vos Besoins:**

- **Sujet de recherche**: {{research_topic}}
- **Objectifs**: {{research_goals}}
- **Type de recherche**: Revue de Littérature Académique
- **Format de citation**: {{citation_style}}
- **Approche**: Analyse systématique avec vérification des sources

**Domaines que Nous Couvrirons:**

1. **Concepts fondamentaux** — Définitions, origines, évolution historique
2. **Théories et cadres conceptuels** — Modèles théoriques principaux
3. **État de l'art** — Recherches récentes et avancées
4. **Débats et controverses** — Points de tension dans la littérature
5. **Gaps identifiés** — Ce que la littérature n'a pas encore exploré
6. **Positionnement** — Comment votre recherche s'inscrit dans ce paysage

**Est-ce que cela capture bien ce que vous recherchez ?**"

### 2. Affiner le Périmètre

Recueillir les clarifications nécessaires:

#### Questions de Cadrage:
- "Y a-t-il des auteurs ou théories incontournables que vous connaissez déjà ?"
- "Devons-nous nous concentrer sur une période spécifique (ex: 10 dernières années) ?"
- "Y a-t-il des disciplines connexes à explorer (psychologie, économie, sociologie...) ?"
- "Préférez-vous des sources francophones, anglophones, ou les deux ?"

### 3. Définir les Mots-clés

Proposer une liste de mots-clés bilingues:

```markdown
## Mots-clés de Recherche

### Français
- [mot-clé principal 1]
- [mot-clé principal 2]
- [mot-clé combiné 1]

### English
- [keyword 1]
- [keyword 2]
- [combined keyword 1]

### Opérateurs de recherche suggérés
- "[concept 1]" AND "[concept 2]"
- "[concept]" AND "systematic review"
- "[concept]" AND "[contexte spécifique]"
```

### 4. Documenter le Cadrage Initial

**ÉCRIRE IMMÉDIATEMENT AU DOCUMENT**

Écrire le cadrage initial:

```markdown
# Revue de Littérature: {{research_topic}}

## Cadrage de la Recherche

### Compréhension Confirmée

**Sujet**: {{research_topic}}
**Objectifs**: {{research_goals}}
**Type**: Revue de Littérature Académique
**Format de citation**: {{citation_style}}
**Date**: {{date}}

### Périmètre de Recherche

**Domaines à couvrir:**
- Concepts fondamentaux et définitions
- Théories et cadres conceptuels
- État de l'art et recherches récentes
- Débats et controverses
- Gaps et opportunités de recherche

**Mots-clés:**
- FR: [liste]
- EN: [liste]

**Sources ciblées:**
- Bases académiques: Google Scholar, Cairn, PubMed, JSTOR
- Thèses: HAL, ProQuest
- Rapports: Organismes de référence du domaine

### Méthodologie

- Recherche systématique avec mots-clés bilingues
- Vérification des sources multiples
- Priorisation des sources peer-reviewed
- Citation au format {{citation_style}}

### Prochaines Étapes

1. ✅ Initialisation et cadrage (étape actuelle)
2. Recherche des concepts fondamentaux et définitions
3. Analyse des théories et cadres conceptuels
4. État de l'art et recherches récentes
5. Identification des gaps et positionnement
6. Synthèse et document final

**Statut**: Périmètre confirmé, prêt pour la recherche détaillée
```

### 5. Présenter l'Option de Continuation

"J'ai documenté notre compréhension et le cadrage initial pour la revue de littérature sur **{{research_topic}}**.

**Ce que j'ai établi:**
- Sujet et objectifs confirmés
- Domaines d'analyse définis
- Mots-clés bilingues préparés
- Méthodologie de recherche établie

**Statut du document:** Cadrage initial écrit pour votre révision

**Prêt à commencer la recherche des concepts fondamentaux ?**

[C] Continuer — Confirmer le périmètre et passer à la recherche des concepts
[M] Modifier — Suggérer des changements au périmètre avant de continuer"

### 6. Gérer la Réponse

#### Si 'C' (Continuer):
- Mettre à jour le frontmatter: `stepsCompleted: [1]`
- Ajouter une note de confirmation: "Périmètre confirmé par l'utilisateur le {{date}}"
- Charger: `./step-02-foundational-concepts.md`

#### Si 'M' (Modifier):
- Recueillir les changements de l'utilisateur
- Mettre à jour le document avec les modifications
- Re-présenter le périmètre mis à jour pour confirmation

## MÉTRIQUES DE SUCCÈS:

✅ Sujet et objectifs de recherche compris avec précision
✅ Périmètre de la revue clairement défini
✅ Mots-clés bilingues établis
✅ Document de cadrage initial écrit immédiatement
✅ Opportunité de révision donnée à l'utilisateur
✅ Option [C] présentée et gérée correctement

## MODES D'ÉCHEC:

❌ Ne pas confirmer la compréhension du sujet et des objectifs
❌ Générer du contenu de recherche au lieu de juste clarifier le périmètre
❌ Ne pas écrire le document de cadrage initial
❌ Ne pas donner l'opportunité de modifier le périmètre
❌ Continuer à l'étape suivante sans confirmation utilisateur

## ÉTAPE SUIVANTE:

Après confirmation utilisateur, charger `./step-02-foundational-concepts.md` pour commencer la recherche des concepts fondamentaux et définitions.
