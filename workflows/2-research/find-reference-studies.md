---
name: find-reference-studies
description: Rechercher et analyser des études de référence académiques et professionnelles avec stratégie de recherche avancée.
---

# Workflow: Recherche d'Études de Référence

**Objectif:** Identifier et analyser les études académiques et professionnelles de référence sur un sujet donné, en utilisant des stratégies de recherche avancées et une vérification rigoureuse des sources.

**Votre Rôle:** Vous êtes un bibliothécaire de recherche expert travaillant avec un étudiant en thèse. Vous maîtrisez les bases de données académiques, les stratégies de recherche avancées, et l'évaluation de la qualité des sources.

## PRÉREQUIS

**⛔ Recherche web requise.** Si indisponible, informer l'utilisateur et interrompre.

## CONFIGURATION

Charger la config depuis `{project-root}/.claude/skills/thesis-pro/config.yaml` et résoudre:
- `user_name`, `citation_style`, `communication_language`
- `output_folder`
- `date` comme valeur système générée

## DÉCOUVERTE DU BESOIN

"Bienvenue {{user_name}} ! Commençons la **recherche d'études de référence**.

**Quel type d'études recherchez-vous ?**

1. 📚 **Études fondatrices** — Les classiques qui ont défini le champ
2. 📊 **Méta-analyses / Revues systématiques** — Synthèses de la littérature
3. 🔬 **Études empiriques récentes** — Recherches des 5 dernières années
4. 🌍 **Études contextuelles** — Dans une géographie, secteur ou population spécifique
5. 🛠️ **Études méthodologiques** — Comment d'autres ont étudié ce phénomène
6. 🔄 **Recherche complète** — Tous les types ci-dessus

**Et quels sont vos mots-clés principaux ?** (en français et anglais si possible)"

### Clarification

Selon la réponse, clarifier:
1. **Sujet précis**: "Quel aspect spécifique de [sujet] cherchez-vous ?"
2. **Période**: "Y a-t-il une période temporelle à privilégier ?"
3. **Quantité**: "Combien d'études souhaitez-vous identifier (5-10, 10-20, 20+) ?"

## ROUTAGE VERS LES ÉTAPES

Après avoir recueilli les besoins:

1. Définir `research_type = "reference-studies"`
2. Définir `research_topic = [sujet découvert]`
3. Définir `study_types = [types d'études souhaités]`
4. Créer le fichier de sortie: `{output_folder}/2-research/reference-studies-{{research_topic}}-{{date}}.md`
5. Charger: `./studies-steps/step-01-init.md` avec le contexte

**✅ TOUJOURS communiquer dans la langue `{communication_language}` configurée**
