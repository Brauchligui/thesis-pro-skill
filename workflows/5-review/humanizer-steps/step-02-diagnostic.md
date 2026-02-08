# Étape 2 — Diagnostic : Marqueurs IA et analyse stylistique

## Objectif
Identifier précisément ce qui rend le texte "robotique" ou détectable comme généré par IA, pour cibler les transformations.

## Instructions pour l'agent

### 1. Analyse des marqueurs IA typiques
Examinez le texte pour chacun de ces patterns. Pour chaque catégorie, attribuez un score de 0 (absent) à 3 (omniprésent) :

#### A. Structure syntaxique
- [ ] **Monotonie structurelle** : phrases qui suivent toujours le même schéma (Sujet-Verbe-Complément)
- [ ] **Longueur uniforme** : phrases de longueur quasi-identique (faible "burstiness")
- [ ] **Parallélisme excessif** : constructions symétriques répétées ("D'une part... D'autre part...", listes de 3 systématiques)

#### B. Vocabulaire et transitions
- [ ] **Connecteurs surexploités** : "De plus", "En outre", "Par ailleurs", "Il est important de noter", "Il convient de souligner"
- [ ] **Hedging mécanique** : "Il semble que", "On pourrait argumenter que", "Il est à noter que"
- [ ] **Adverbes de remplissage** : "fondamentalement", "essentiellement", "indéniablement", "incontestablement"
- [ ] **Vocabulaire LLM signature** : "crucial", "landscape" (paysage), "delve", "navigate", "foster", "leverage", "comprehensive"

#### C. Ton et posture
- [ ] **Neutralité excessive** : aucune prise de position, tout est nuancé de manière mécanique
- [ ] **Conclusions prévisibles** : chaque paragraphe se termine par une synthèse qui reformule le début
- [ ] **Absence de voix** : aucune marque personnelle, aucun "je", aucune anecdote ou expérience
- [ ] **Politesse artificielle** : formulations trop policées qui sonnent comme un assistant

#### D. Organisation
- [ ] **Listes à puces systématiques** : abus de bullet points là où de la prose suffirait
- [ ] **Sous-titres excessifs** : fragmentation artificielle du texte
- [ ] **Symétrie forcée** : arguments "pour" et "contre" toujours parfaitement équilibrés

### 2. Calcul du score de naturalité
Additionnez les scores (0-3) de chaque item coché.
- **0-8** : Texte plutôt naturel, ajustements légers nécessaires
- **9-20** : Texte mixte, humanisation modérée requise
- **21-36** : Texte très "IA", refonte stylistique profonde nécessaire
- **37+** : Réécriture quasi-complète recommandée

### 3. Présentation du diagnostic
Présentez à l'utilisateur :
1. Le **score global** avec l'interprétation
2. Les **3 problèmes les plus flagrants** avec des exemples tirés du texte (citations exactes)
3. Les **points forts** à conserver (il y en a toujours)
4. Une **recommandation** : ajustements ciblés vs refonte profonde

### 4. Validation
Demandez à l'utilisateur s'il est d'accord avec le diagnostic et s'il veut ajuster les priorités avant de continuer.

## Exemple de présentation du diagnostic

```
DIAGNOSTIC HUMANIZER
Score de naturalité : 24/48 — Texte mixte

Les 3 alertes principales :
1. TRANSITIONS MÉCANIQUES (score 3/3)
   → "De plus, il convient de souligner que..." (ligne 12)
   → "Par ailleurs, il est important de noter..." (ligne 28)

2. MONOTONIE SYNTAXIQUE (score 3/3)
   → 8 phrases consécutives de 20-25 mots en structure S-V-C

3. ABSENCE DE VOIX (score 2/3)
   → Aucun "je" ou marqueur personnel sur 500 mots
   → Ton uniformément détaché

Points forts à conserver :
- Argumentation logique solide
- Références bien intégrées
- Vocabulaire technique précis

Recommandation : Humanisation modérée — garder la structure,
transformer les transitions et injecter de la voix.
```
