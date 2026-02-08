# Humanizer - Dé-robotiser et personnaliser le texte

## Objectif
Transformer un texte rédigé par IA ou trop mécaniquement académique en un texte authentiquement humain, portant la voix personnelle de l'auteur, adapté au registre souhaité, et résistant aux détecteurs IA.

## Pré-requis
- Un texte à humaniser (collé par l'utilisateur ou référence à une section)
- Le profil de voix de l'auteur (créé à la première utilisation, réutilisable ensuite)

## Déroulement du workflow

Ce workflow se déroule en **6 étapes séquentielles**. Chaque étape doit être complétée avant de passer à la suivante. Guidez l'utilisateur à travers chacune.

### Étapes

| # | Fichier | Étape | Description |
|---|---------|-------|-------------|
| 1 | `humanizer-steps/step-01-input.md` | Collecte | Récupérer le texte et comprendre le contexte |
| 2 | `humanizer-steps/step-02-diagnostic.md` | Diagnostic | Identifier les marqueurs IA et les faiblesses stylistiques |
| 3 | `humanizer-steps/step-03-voice-profile.md` | Profil de voix | Charger ou créer le profil stylistique de l'auteur |
| 4 | `humanizer-steps/step-04-humanize.md` | Humanisation | Appliquer les transformations |
| 5 | `humanizer-steps/step-05-ai-audit.md` | Audit anti-IA | Vérifier qu'aucun pattern détectable ne subsiste |
| 6 | `humanizer-steps/step-06-output.md` | Livraison | Présenter le résultat et sauvegarder |

## Instructions pour l'agent

1. Chargez et exécutez chaque étape dans l'ordre
2. À chaque transition d'étape, résumez brièvement ce qui a été fait et annoncez l'étape suivante
3. Si l'utilisateur veut sauter une étape (ex: le profil de voix existe déjà), adaptez-vous
4. Restez dans le persona Dr. Alex tout au long du processus
5. Sauvegardez le résultat final dans `{output_folder}/humanized/` avec un nom descriptif
