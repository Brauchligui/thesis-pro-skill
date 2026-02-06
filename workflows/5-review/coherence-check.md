# 🔍 Workflow: Vérification de Cohérence et Style Académique

## Objectif
Analyser une section ou l'ensemble de la thèse pour vérifier la cohérence argumentative, la qualité du style académique et la conformité aux standards.

---

## Instructions pour l'Agent

### Étape 1: Périmètre de la révision

Demander à l'utilisateur:
> "Que souhaitez-vous que je révise ?
>
> 1. **Une section spécifique** (introduction, chapitre, conclusion...)
> 2. **L'articulation entre sections** (transitions, fil rouge)
> 3. **Le style académique** d'un passage
> 4. **La cohérence globale** de la thèse
> 5. **Vérification pré-soumission** (check-list complète)"

Demander de partager le texte à réviser.

---

### Étape 2: Grilles d'analyse

#### 2a. Cohérence argumentative

| Critère | ✓ | Observations |
|---------|---|--------------|
| **Fil rouge visible** | | La problématique guide-t-elle tout le texte ? |
| **Progression logique** | | Chaque partie découle de la précédente ? |
| **Pas de contradictions** | | Les affirmations sont-elles cohérentes ? |
| **Conclusions justifiées** | | Les conclusions découlent-elles des résultats ? |
| **Transitions fluides** | | Les liens entre parties sont-ils explicites ? |

#### 2b. Style académique

| Critère | ✓ | Observations |
|---------|---|--------------|
| **Objectivité** | | Évite-t-on les opinions non étayées ? |
| **Précision** | | Le vocabulaire est-il exact ? |
| **Nuance** | | Évite-t-on les généralisations ? |
| **Citations appropriées** | | Chaque affirmation est-elle sourcée ? |
| **Clarté** | | Les phrases sont-elles compréhensibles ? |
| **Concision** | | Pas de verbiage inutile ? |

#### 2c. Structure et forme

| Critère | ✓ | Observations |
|---------|---|--------------|
| **Paragraphes structurés** | | 1 idée = 1 paragraphe ? |
| **Titres informatifs** | | Les titres reflètent-ils le contenu ? |
| **Cohérence typographique** | | Mêmes conventions partout ? |
| **Figures/tableaux référencés** | | Cités et numérotés correctement ? |
| **Annexes pertinentes** | | Tout ce qui doit y être y est ? |

---

### Étape 3: Analyse détaillée

#### Pour chaque problème identifié, fournir:

```markdown
### Problème [N]
**Type**: [Cohérence / Style / Structure / Citation]
**Localisation**: [Section, paragraphe approximatif]
**Description**: [Ce qui pose problème]
**Suggestion**: [Comment améliorer]
**Priorité**: [Haute / Moyenne / Basse]
```

#### Catégoriser les retours:
- 🔴 **Critique**: À corriger absolument
- 🟡 **Important**: Améliorerait significativement la qualité
- 🟢 **Suggestion**: Pour aller vers l'excellence

---

### Étape 4: Points de vigilance spécifiques

#### Vérifier l'introduction:
- [ ] Accroche engageante
- [ ] Problématique clairement énoncée
- [ ] Plan annoncé fidèlement suivi

#### Vérifier la conclusion:
- [ ] Répond explicitement à la problématique
- [ ] Ne contient pas de nouvelles informations
- [ ] Ouvre des perspectives

#### Vérifier la méthodologie:
- [ ] Tous les choix sont justifiés
- [ ] Les limites sont reconnues honnêtement

#### Vérifier les résultats:
- [ ] Présentation séparée de l'interprétation
- [ ] Données présentées clairement

#### Vérifier la discussion:
- [ ] Lien avec la littérature existante
- [ ] Contributions clairement articulées

---

### Étape 5: Cohérence terminologique

Vérifier que:
- Les termes clés sont définis à leur première utilisation
- Les mêmes concepts utilisent les mêmes termes partout
- Les acronymes sont développés à la première occurrence
- Le registre de langue est constant

---

### Étape 6: Check-list pré-soumission

Si révision finale demandée:

#### Contenu
- [ ] Page de titre conforme aux exigences
- [ ] Résumé + mots-clés (FR et EN)
- [ ] Remerciements (si souhaité)
- [ ] Table des matières à jour
- [ ] Liste des figures et tableaux
- [ ] Numérotation des pages correcte
- [ ] Bibliographie complète et formatée
- [ ] Annexes référencées dans le texte

#### Forme
- [ ] Police et taille conformes
- [ ] Marges respectées
- [ ] Interligne correct
- [ ] En-têtes et pieds de page
- [ ] Pas de pages blanches non voulues
- [ ] Qualité des images/graphiques

#### Dernières vérifications
- [ ] Relecture orthographique finale
- [ ] Vérification des hyperliens (si version numérique)
- [ ] Test d'impression (si version papier)

---

### Étape 7: Rapport de révision

```markdown
# Rapport de Révision - [Section/Document]
Date: [Date]
Réviseur: Dr. Alex (Thesis Pro Assistant)

---

## Résumé
[Appréciation générale en 3-4 phrases]

## Points forts
- [Force 1]
- [Force 2]
- [Force 3]

## Points à améliorer

### 🔴 Critiques (à corriger)
1. [Problème] → [Suggestion]
2. ...

### 🟡 Importants (recommandés)
1. [Problème] → [Suggestion]
2. ...

### 🟢 Suggestions (optionnels)
1. [Amélioration possible]
2. ...

## Prochaines étapes recommandées
1. [Action prioritaire]
2. [Action secondaire]
3. ...

---

*Ce rapport vise à améliorer la qualité du travail. Les points soulevés sont des suggestions d'amélioration.*
```

Sauvegarder dans: `{output_folder}/5-review/revision-report-[date].md`

---

## Conseils pour l'Agent
- Être constructif: toujours proposer des solutions
- Commencer par les points positifs
- Ne pas submerger: prioriser les retours
- Expliquer le "pourquoi" des suggestions
- Rappeler que la perfection n'existe pas, viser l'excellence accessible
- Encourager: arriver à la révision signifie que le gros du travail est fait !
