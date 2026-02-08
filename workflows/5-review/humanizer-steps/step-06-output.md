# Étape 6 — Livraison et sauvegarde

## Objectif
Présenter le résultat final avec une comparaison avant/après, sauvegarder le texte humanisé, et fournir des conseils pour la suite.

## Instructions pour l'agent

### 1. Comparaison avant/après

Présentez une vue synthétique des transformations :

```
RÉSUMÉ DE L'HUMANISATION

Texte original : {word_count} mots
Texte humanisé : {new_word_count} mots
Variation : +/- X%

Registre : {target_register}
Score diagnostic initial : XX/48 (texte très IA)
Score audit final : X/10 (confiance humanité)

Principales transformations :
1. [description de la transformation la plus impactante]
2. [...]
3. [...]
4. [...]
5. [...]
```

### 2. Extraits comparatifs
Choisissez **2-3 passages représentatifs** et montrez le avant/après côte à côte :

```
AVANT :
"De plus, il convient de souligner que les biais cognitifs jouent un rôle
fondamental dans les décisions de santé publique. En effet, ces mécanismes
psychologiques influencent de manière significative les comportements..."

APRÈS :
"Les biais cognitifs pèsent lourd dans les décisions de santé publique —
plus qu'on ne le croit. Ce sont ces raccourcis mentaux, souvent invisibles,
qui orientent nos choix bien avant que la rationalité n'entre en jeu."
```

### 3. Sauvegarde

Sauvegardez le texte humanisé dans :
`{output_folder}/humanized/{section_type}-humanized-{date}.md`

Le fichier sauvegardé doit contenir :
- Un en-tête avec les métadonnées (date, section, registre, scores)
- Le texte humanisé complet
- Pas les commentaires d'analyse (texte prêt à intégrer)

Format de l'en-tête :
```yaml
---
source: "[section originale]"
date: YYYY-MM-DD
register: "[registre choisi]"
diagnostic_score: XX/48
audit_score: X/10
voice_profile: true/false
---
```

### 4. Conseils pour la suite

Proposez à l'utilisateur :

**Pour ce texte :**
- "Relisez-le à voix haute — c'est le meilleur test d'authenticité. Si vous butez sur une phrase, c'est qu'elle n'est pas naturelle."
- "Laissez reposer quelques heures puis relisez. Marquez ce qui ne vous ressemble pas."

**Pour les prochaines sessions :**
- "Votre profil de voix est sauvegardé. Les prochaines humanisations seront plus rapides."
- "Si vous rédigez d'abord un brouillon personnel (même très approximatif), l'humanisation sera plus authentique qu'à partir d'un texte 100% IA."

**Proposition de suite :**
- Souhaitez-vous humaniser une autre section ?
- Souhaitez-vous passer le texte en revue de cohérence ([RV] Review) ?
- Souhaitez-vous retourner au menu principal ?

### 5. Retour au menu
Après la réponse de l'utilisateur, redirigez vers l'action choisie ou réaffichez le menu principal.
