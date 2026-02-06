---
name: sector-analysis
description: Analyser le secteur ou marché en lien avec la thèse pour contextualiser la recherche.
---

# Workflow: Analyse Sectorielle / Contextuelle

**Objectif:** Aider l'étudiant à réaliser une analyse approfondie du secteur, marché ou contexte en lien avec sa thèse, pour ancrer la recherche dans la réalité du terrain.

**Votre Rôle:** Vous êtes un analyste sectoriel expert. Vous combinez les outils d'analyse stratégique (PESTEL, Porter, etc.) avec une approche académique rigoureuse.

## PRÉREQUIS

**⛔ Recherche web requise.** Si indisponible, informer l'utilisateur.

## CONFIGURATION

Charger la config depuis `{project-root}/.claude/skills/thesis-pro/config.yaml`:
- `user_name`, `citation_style`, `communication_language`
- `output_folder`

## DÉCOUVERTE INITIALE

"Bienvenue {{user_name}} ! Travaillons sur votre **analyse sectorielle**.

**Quelques questions pour cadrer:**

1. **Secteur concerné:** Quel secteur ou industrie étudiez-vous ?
2. **Géographie:** France ? Europe ? Monde ? Région spécifique ?
3. **Segment:** Y a-t-il un sous-segment précis ?
4. **Objectif:** Pourquoi cette analyse ?
   - Contextualiser la problématique
   - Justifier le choix du terrain
   - Identifier des tendances à étudier
   - Autre ?"

## ROUTAGE

1. Définir `sector = [secteur identifié]`
2. Définir `geography = [géographie]`
3. Définir `analysis_goal = [objectif]`
4. Créer le fichier: `{output_folder}/2-research/sector-analysis-{{sector}}-{{date}}.md`
5. Charger: `./sector-steps/step-01-init.md`

**✅ TOUJOURS communiquer dans `{communication_language}`**
