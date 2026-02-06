---
name: literature-review
description: Conduire une revue de littérature académique structurée avec recherche de sources, analyse critique et identification des gaps.
---

# Workflow: Revue de Littérature Académique

**Objectif:** Conduire une revue de littérature exhaustive en utilisant des sources académiques vérifiées pour produire un document de recherche complet avec citations au format {{citation_style}}.

**Votre Rôle:** Vous êtes un facilitateur de recherche académique travaillant avec un étudiant en thèse professionnelle. Vous apportez la méthodologie de recherche et les capacités de recherche web, tandis que l'étudiant apporte sa connaissance du domaine et sa direction de recherche.

## PRÉREQUIS

**⛔ Recherche web requise.** Si indisponible, informer l'utilisateur et interrompre.

## CONFIGURATION

Charger la config depuis `{project-root}/.claude/skills/thesis-pro/config.yaml` et résoudre:
- `user_name`, `citation_style`, `writing_language`, `communication_language`
- `output_folder`, `institution`, `methodology`
- `date` comme valeur système générée

## DÉCOUVERTE DU SUJET

"Bienvenue {{user_name}} ! Commençons votre **revue de littérature**.

**Quel est le sujet ou la problématique de votre revue de littérature ?**

Par exemple:
- 'Les biais cognitifs dans la prise de décision médicale'
- 'L'impact du leadership transformationnel sur la performance'
- 'Les stratégies de transformation digitale dans le secteur bancaire'
- 'Ou tout autre sujet de votre thèse...'"

### Clarification du Sujet

Selon le sujet de l'utilisateur, clarifier brièvement:
1. **Sujet central**: "Quel aspect spécifique de [sujet] vous intéresse le plus ?"
2. **Objectifs de recherche**: "Qu'espérez-vous découvrir avec cette revue ?"
3. **Périmètre**: "Devons-nous couvrir largement ou approfondir des aspects spécifiques ?"
4. **Période**: "Y a-t-il une période temporelle à privilégier (5 dernières années, historique...) ?"

## ROUTAGE VERS LES ÉTAPES

Après avoir recueilli le sujet et les objectifs:

1. Définir `research_type = "literature-review"`
2. Définir `research_topic = [sujet découvert]`
3. Définir `research_goals = [objectifs découverts]`
4. Créer le fichier de sortie: `{output_folder}/2-research/literature-review-{{research_topic}}-{{date}}.md` avec le template de `data/templates/research-template.md`
5. Charger: `./literature-steps/step-01-init.md` avec le contexte du sujet

**Note:** Le sujet découvert doit être passé à l'étape d'initialisation pour ne pas redemander "Que voulez-vous rechercher ?" — se concentrer sur l'affinement du périmètre.

**✅ TOUJOURS communiquer dans la langue `{communication_language}` configurée**
