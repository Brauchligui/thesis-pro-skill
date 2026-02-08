# Étape 4 — Humanisation du texte

## Objectif
Transformer le texte en appliquant les corrections identifiées au diagnostic, en injectant la voix de l'auteur, et en adaptant au registre cible.

## Instructions pour l'agent

### Principes fondamentaux

> **Règle d'or** : Un texte humanisé doit donner l'impression que l'auteur l'a écrit d'une traite, un dimanche matin avec son café, pas qu'un algorithme l'a optimisé.

1. **Conserver le fond** : le sens, les arguments et les références ne changent JAMAIS
2. **Transformer la forme** : syntaxe, rythme, transitions, ton
3. **Respecter le profil** : chaque modification doit rapprocher le texte du voice profile
4. **Doser l'imperfection** : un vrai humain n'écrit pas parfaitement ; les légères aspérités sont un signe d'authenticité

### Techniques d'humanisation

Appliquez ces techniques dans l'ordre, en fonction du diagnostic (étape 2) :

#### A. Casser la monotonie syntaxique
- **Varier les longueurs** : alterner phrases courtes (5-10 mots) et développées (25-35 mots)
- **Varier les structures** : commencer certaines phrases par un complément, une subordonnée, un adverbe
- **Insérer des incises** : parenthèses, virgules d'encadrement, apartés, comme le ferait l'auteur selon son profil
- **ÉVITER les tirets cadratins (—)** : c'est un marqueur IA très connu. **En français** : ne JAMAIS utiliser de tiret cadratin en incise, c'est un anglicisme typographique absent de la prose française naturelle (réservé aux dialogues). Utiliser les virgules, deux-points, parenthèses ou points de suspension. **En anglais** : usage modéré acceptable (max 2-3 par page), mais varier avec d'autres ponctuations
- **Fragmenter occasionnellement** : une phrase nominale isolée pour l'impact. Comme ça.

#### B. Remplacer les transitions mécaniques
Ne PAS simplement substituer un connecteur par un autre. Restructurez :

| Au lieu de... | Essayez... |
|---------------|------------|
| "De plus, il convient de noter que..." | Fusionner avec la phrase précédente ou supprimer le connecteur |
| "Par ailleurs..." | Transition implicite par juxtaposition |
| "Il est important de souligner que..." | Affirmer directement : "Ce qui frappe, c'est..." |
| "En outre..." | Enchaîner par un exemple concret |
| "Néanmoins, il faut reconnaître que..." | "Sauf que..." / "Le hic, c'est que..." (selon le registre) |

#### C. Injecter la voix de l'auteur
En s'appuyant sur le voice profile :
- **Intégrer le "je"** là où l'auteur prendrait naturellement position (selon son profil)
- **Ajouter des questions rhétoriques** si c'est un tic identifié
- **Placer 1-2 références à l'expérience pro** si le contexte s'y prête ("dans mon expérience chez...")
- **Utiliser les connecteurs fétiches** de l'auteur
- **Reproduire le rythme naturel** identifié dans le profil

#### D. Adapter le registre
Selon le choix de l'étape 1 :

**Académique soutenu** :
- Maintenir la rigueur terminologique
- "Je" remplacé par "nous" ou formes impersonnelles actives
- Humaniser par la variation syntaxique et les exemples, pas par le registre familier

**Académique accessible** :
- Autoriser le "je" avec parcimonie
- Définir les termes techniques à la première occurrence
- Phrases plus courtes, exemples concrets intercalés

**Professionnel** :
- "Je" assumé
- Aller droit au point, moins de précautions oratoires
- Exemples tirés du terrain

**Conversationnel éduqué** :
- Ton direct, questions au lecteur
- Anecdotes et métaphores bienvenues
- Parenthèses et incises fréquentes

#### E. Ajouter des micro-imperfections naturelles
Subtilement, sans compromettre la qualité :
- Une phrase légèrement plus longue que nécessaire (comme quand on développe sa pensée en écrivant)
- Une reformulation mid-phrase ("la question, ou plutôt le dilemme,")
- Un connecteur oral occasionnel ("Or", "Sauf que", "Reste que")
- Une parenthèse qui ajoute une nuance personnelle

### Processus de réécriture

1. **Premier passage** : Traitez le texte paragraphe par paragraphe
2. **Deuxième passage** : Relisez l'ensemble pour la fluidité et la cohérence globale
3. **Vérification croisée** : Comparez avec le profil de voix. Est-ce que ça "sonne" comme l'auteur ?

### Présentation du résultat
Présentez le texte humanisé **dans son intégralité**, sans annotations ni commentaires intercalés. Le texte doit être prêt à l'emploi.

Puis, séparément, listez les **5 modifications les plus significatives** avec une brève justification pour chacune.

### Validation
Demandez à l'utilisateur :
- "Ce texte vous ressemble-t-il ?"
- "Y a-t-il des passages où vous ne vous reconnaissez pas ?"
- Si des ajustements sont nécessaires, itérez sur les passages concernés
