# 🧠 Workflow: Brainstorm - Explorer ou Affiner la Problématique

## Objectif
Aider l'étudiant à transformer une idée vague en problématique de recherche claire et pertinente, ou à affiner une problématique existante, en utilisant des techniques de brainstorming diversifiées.

---

## Instructions pour l'Agent

### Configuration
- **Techniques disponibles**: `{project-root}/.claude/skills/thesis-pro/data/brainstorming-techniques.csv`
- **Objectif quantitatif**: Viser 20-50 pistes avant de converger
- **Anti-biais**: Changer de catégorie de technique toutes les 10 idées

---

## PHASE 1: ÉVALUATION DU POINT DE DÉPART

Demander à l'utilisateur:
> "Où en êtes-vous avec votre sujet de thèse ?
>
> 1. 💭 **Idée vague** — J'ai un domaine d'intérêt mais pas de sujet précis
> 2. 🎯 **Sujet défini** — J'ai un sujet mais pas encore de problématique
> 3. 🔍 **Problématique à affiner** — J'ai une problématique mais je veux l'améliorer
> 4. ⚔️ **Challenge** — Je veux stress-tester ma problématique existante"

Adapter la suite en fonction de la réponse.

---

## PHASE 2: CHOIX DE L'APPROCHE

Proposer à l'utilisateur:
> "Comment voulez-vous procéder ?
>
> 1. 🎲 **Exploration libre** — Je vous guide à travers plusieurs techniques
> 2. 🎯 **Technique spécifique** — Choisir une technique dans le catalogue
> 3. 🤖 **Recommandation IA** — Je choisis les techniques les plus adaptées à votre situation
> 4. 🌀 **Flow progressif** — On commence doucement et on intensifie"

---

## PHASE 3: CATALOGUE DES TECHNIQUES

### Catégories disponibles

Charger et présenter les techniques depuis le CSV:

#### 🤝 Collaboratives
Pour enrichir par itérations successives.

#### 🎨 Créatives
Pour sortir des sentiers battus et faire des connexions inattendues.

#### 🔬 Profondes (Deep Thinking)
Pour creuser en profondeur et trouver les causes racines.

#### 🪞 Introspectives
Pour explorer vos motivations et dépasser vos blocages.

#### 📐 Structurées
Pour une exploration méthodique et systématique.

#### 🎭 Théâtrales
Pour adopter d'autres perspectives par le jeu de rôle.

#### 🌪️ Wild Cards
Pour casser les codes et provoquer des ruptures.

#### 🌿 Biomimétiques
Pour s'inspirer de la nature et des systèmes vivants.

#### 🌍 Culturelles
Pour puiser dans la sagesse collective et les traditions.

---

## PHASE 4: EXÉCUTION DES TECHNIQUES

### Protocole d'exécution

Pour chaque technique choisie:

1. **Introduire** la technique et son objectif
2. **Expliquer** comment elle s'applique au contexte thèse
3. **Guider** l'utilisateur à travers les prompts spécifiques
4. **Capturer** toutes les idées générées (sans jugement)
5. **Transition** vers la technique suivante si applicable

### Techniques prioritaires pour une thèse

#### Pour trouver un sujet (si idée vague)

**1. Values Archaeology** (Introspective)
> "Creusons ce qui vous anime vraiment...
> - Dans votre expérience professionnelle, quel problème vous frustre le plus ?
> - Quelle injustice ou inefficacité vous met en colère ?
> - Si vous pouviez changer UNE chose dans votre domaine, ce serait quoi ?"

**2. Role Playing** (Collaborative)
> "Mettons-nous dans la peau de différents acteurs...
> - Comment un [patient/client/utilisateur] vit-il ce problème ?
> - Qu'est-ce qu'un [dirigeant/décideur] aimerait comprendre ?
> - Que dirait un [chercheur/expert] qui étudie ce domaine ?"

**3. Cross-Pollination** (Créative)
> "Regardons ce qui se fait ailleurs...
> - Comment ce problème est-il résolu dans d'autres industries ?
> - Quelles solutions existent dans d'autres pays ?
> - Que ferait une startup face à ce défi ?"

#### Pour affiner une problématique

**1. Five Whys** (Profonde)
> "Creusons les causes...
> Pourquoi [problème initial] ? → Réponse → Pourquoi ? → ... (5 fois)"

**2. Assumption Reversal** (Profonde)
> "Questionnons les évidences...
> - Qu'est-ce qu'on tient pour acquis dans ce domaine ?
> - Et si le contraire était vrai ?
> - Quelles hypothèses n'ont jamais été testées ?"

**3. Question Storming** (Profonde)
> "Générons UNIQUEMENT des questions pendant 5 minutes...
> - Pas de réponses autorisées
> - Toutes les questions sont bonnes
> - Plus c'est naïf, mieux c'est"

#### Pour challenger une problématique

**1. Reverse Brainstorming / Anti-Solution** (Wild)
> "Comment pourrait-on rendre cette recherche inutile ?
> - Qu'est-ce qui invaliderait vos conclusions ?
> - Quelles critiques un jury sévère ferait-il ?
> - Où sont les failles logiques ?"

**2. Alien Anthropologist** (Théâtrale)
> "Vous êtes un chercheur martien qui découvre ce sujet...
> - Qu'est-ce qui vous semble absurde dans les pratiques actuelles ?
> - Quelles questions évidentes personne ne pose ?
> - Pourquoi les humains font-ils ainsi ?"

**3. Constraint Mapping** (Profonde)
> "Cartographions toutes les limites...
> - Contraintes théoriques : que dit (ou ne dit pas) la littérature ?
> - Contraintes pratiques : accès au terrain, temps, ressources ?
> - Contraintes éthiques : que ne pouvez-vous PAS faire ?"

---

## PHASE 5: CONVERGENCE

### Critères FINER pour évaluer les pistes

| Critère | Question | ✓/✗ |
|---------|----------|-----|
| **F**easible | Est-ce réalisable dans le temps et avec les ressources disponibles ? | |
| **I**nteresting | Est-ce intéressant pour vous ET pour la communauté ? | |
| **N**ovel | Apporte-t-il quelque chose de nouveau ? | |
| **E**thical | Peut-il être étudié éthiquement ? | |
| **R**elevant | A-t-il des implications pratiques réelles ? | |

### Formulation de la problématique

Templates de formulation:
- "Dans quelle mesure [X] influence-t-il [Y] dans le contexte de [Z] ?"
- "Comment [les acteurs] peuvent-ils [action] pour [objectif] malgré [contrainte] ?"
- "Quels sont les facteurs déterminants de [phénomène] dans [contexte] ?"
- "En quoi [nouveau phénomène] remet-il en question [théorie établie] ?"

### Test de la problématique
1. Pouvez-vous l'expliquer en 30 secondes à un non-initié ?
2. La réponse peut-elle être nuancée (pas juste oui/non) ?
3. Avez-vous accès aux données/terrain nécessaires ?
4. Est-ce aligné avec vos objectifs de carrière ?

---

## PHASE 6: DOCUMENTATION

### Livrable: Brief de Problématique

```markdown
# Brief de Problématique
Date: [Date]
Session de brainstorming: [Durée]

## Techniques utilisées
- [Technique 1]: [Ce qui en est ressorti]
- [Technique 2]: [Ce qui en est ressorti]

## Idées générées (toutes)
1. [Idée 1]
2. [Idée 2]
... [Liste complète]

## Top 3 des pistes retenues
1. **[Piste principale]**
   - Pourquoi: ...
   - Faisabilité: ...

2. **[Piste alternative 1]**
   - Pourquoi: ...

3. **[Piste alternative 2]**
   - Pourquoi: ...

## Problématique formulée
> [Formulation finale]

## Sous-questions de recherche
1. ...
2. ...
3. ...

## Mots-clés pour la recherche
- FR: [mots-clés français]
- EN: [mots-clés anglais]

## Prochaines étapes
- [ ] Valider avec le directeur de thèse
- [ ] Faire une première recherche bibliographique
- [ ] Affiner si nécessaire
```

Sauvegarder dans: `{output_folder}/1-ideation/brainstorm-session-[date].md`

---

## Conseils pour l'Agent

### Posture
- **Facilitateur**, pas directeur : guider par des questions
- **Bienveillant** : toutes les idées sont bonnes en phase divergente
- **Provocateur** : pousser au-delà des premières idées (les meilleures viennent après les 20 premières)
- **Patient** : le silence est productif, laisser le temps de réfléchir

### Anti-patterns à éviter
- Ne pas juger les idées trop tôt
- Ne pas converger avant d'avoir suffisamment divergé
- Ne pas laisser l'utilisateur s'autocensurer
- Ne pas imposer sa propre vision du sujet

### Signaux positifs
- "Je n'avais jamais pensé à ça comme ça"
- "C'est évident mais personne ne le dit"
- "Ça me fait peur mais c'est intéressant"
- Énergie et enthousiasme qui montent
