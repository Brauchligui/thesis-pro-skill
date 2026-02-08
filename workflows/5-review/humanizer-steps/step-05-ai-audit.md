# Étape 5 — Audit anti-détection IA

## Objectif
Vérifier que le texte humanisé ne contient plus de patterns détectables par les outils anti-IA (GPTZero, Originality.ai, Turnitin AI, ZeroGPT, etc.) et recommander les derniers ajustements si nécessaire.

## Instructions pour l'agent

### Contexte important
> Les détecteurs IA ne sont pas fiables à 100%. Ils produisent des faux positifs et des faux négatifs. L'objectif n'est pas de "tromper" un outil, mais de s'assurer que le texte est **authentiquement humain dans sa forme**, ce qui naturellement le rend indétectable.

### 1. Checklist des patterns détectables

Relisez le texte humanisé et vérifiez l'absence des marqueurs suivants :

#### Perplexité (diversité lexicale)
- [ ] Le vocabulaire est-il suffisamment varié ? (pas de répétition du même mot dans un rayon de 3 phrases)
- [ ] Y a-t-il des choix lexicaux surprenants/originaux ? (un humain choisit parfois un mot inattendu)
- [ ] Les synonymes sont-ils utilisés naturellement, pas de manière forcée ?

#### Burstiness (variation de complexité)
- [ ] Les phrases varient-elles significativement en longueur ? (écart-type > 8 mots)
- [ ] Y a-t-il un mélange de phrases simples et complexes ?
- [ ] Le rythme change-t-il entre les paragraphes ? (un paragraphe dense suivi d'un plus aéré)

#### Patterns structurels
- [ ] Pas de structure "topic sentence → développement → conclusion" systématique dans chaque paragraphe
- [ ] Pas de parallélisme parfait entre sections
- [ ] Les transitions sont variées et certaines sont implicites
- [ ] Le texte ne suit pas un schéma prévisible

#### Marqueurs lexicaux IA connus
Vérifiez l'absence de ces termes/tournures (sauf s'ils sont naturels dans le contexte) :
- FR : "il convient de", "force est de constater", "il est primordial", "de manière significative", "dans ce contexte", "il est à noter que"
- EN (si sections bilingues) : "delve", "leverage", "foster", "comprehensive", "landscape", "navigate", "crucial", "moreover", "furthermore"

#### Marqueurs typographiques et stylistiques IA
- [ ] **Tirets cadratins (—)** : compter les occurrences.
  - **En français** : AUCUN tiret cadratin en incise n'est normal. Le français utilise les virgules, parenthèses, deux-points ou points de suspension. Le tiret cadratin est réservé aux dialogues. Tout usage en incise est un anglicisme typographique hérité de l'entraînement LLM sur du texte anglais. Remplacer systématiquement.
  - **En anglais** : l'em-dash est un outil naturel de la prose. Seule la surutilisation est suspecte (plus de 5 par page). Varier avec des virgules ou parenthèses pour ne pas créer de pattern répétitif
- [ ] **Paires adverbe+adjectif en série** : 3+ paires alignées du type "étrangement X, fondamentalement Y, profondément Z" est un pattern IA flagrant
- [ ] **Listes de 3 systématiques** : vérifier que le texte ne retombe pas dans les triades à chaque énumération

#### Cohérence humaine
- [ ] Le texte contient-il au moins une marque personnelle par page ?
- [ ] Y a-t-il des moments de "pensée à voix haute" (reformulations, nuances ajoutées) ?
- [ ] Le niveau de certitude varie-t-il naturellement ? (pas systématiquement nuancé)

### 2. Scoring final

Attribuez un score de confiance :

| Score | Interprétation |
|-------|----------------|
| **9-10** | Indiscernable d'un texte humain. Prêt. |
| **7-8** | Très bon. 1-2 ajustements mineurs recommandés. |
| **5-6** | Correct mais quelques patterns résiduels. Retouches ciblées nécessaires. |
| **< 5** | Insuffisant. Retour à l'étape 4 pour des passages spécifiques. |

### 3. Rapport d'audit

Présentez le rapport sous cette forme :

```
AUDIT ANTI-DÉTECTION IA
Score de confiance : X/10

Perplexité : ✅ Bonne / ⚠️ À améliorer
Burstiness : ✅ Bonne / ⚠️ À améliorer
Patterns structurels : ✅ Absents / ⚠️ Résiduels
Marqueurs lexicaux : ✅ Nettoyés / ⚠️ Restants
Cohérence humaine : ✅ Présente / ⚠️ Insuffisante

Passages à risque :
→ [citation du passage] — Raison : [explication]
→ ...

Recommandations :
1. ...
2. ...
```

### 4. Corrections si nécessaire
Si le score est < 7 :
- Identifiez les passages problématiques précis
- Proposez des reformulations ciblées
- Appliquez les corrections et re-scorez

### 5. Rappel éthique
Informez l'utilisateur :
> "Cet audit vérifie que votre texte reflète authentiquement votre pensée et votre style. L'objectif est l'authenticité, pas la dissimulation. Un texte véritablement pensé et retravaillé par son auteur n'a rien à cacher."
