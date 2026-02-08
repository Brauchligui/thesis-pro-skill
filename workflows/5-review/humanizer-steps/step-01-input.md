# Étape 1 — Collecte du texte et du contexte

## Objectif
Récupérer le texte à humaniser et comprendre son contexte pour calibrer les transformations.

## Instructions pour l'agent

### 1. Demander le texte
Demandez à l'utilisateur de fournir le texte à humaniser. Accepter :
- Un copier-coller direct dans le chat
- Une référence à un fichier existant (chemin relatif ou absolu)
- Une référence à une section de la thèse par nom (ex: "l'introduction du chapitre III")

### 2. Collecter le contexte
Posez les questions suivantes (une par une, pas un formulaire) :

**a) Type de contenu**
- De quelle section de la thèse s'agit-il ? (introduction, revue de littérature, méthodologie, résultats, discussion, conclusion)
- Ou est-ce un texte hors-thèse ? (article, résumé, abstract)

**b) Audience cible**
- Qui va lire ce texte ? (jury académique, professionnels du secteur, public large)

**c) Registre souhaité**
Proposez ces options :
1. **Académique soutenu** — Formel, précis, conventions académiques respectées
2. **Académique accessible** — Rigoureux mais lisible, moins jargonnant
3. **Professionnel** — Ton expert mais direct, orienté praticien
4. **Conversationnel éduqué** — Comme si l'auteur expliquait à un collègue intelligent

**d) Priorité**
Qu'est-ce qui compte le plus pour l'utilisateur ?
1. Que ça sonne naturel / humain
2. Que ça reflète MA voix personnelle
3. Que ça passe les détecteurs IA
4. Les trois à parts égales

### 3. Confirmer la compréhension
Résumez en 2-3 phrases ce que vous avez compris de la demande avant de passer à l'étape suivante.

## Variables à transmettre aux étapes suivantes
- `{text_input}` : le texte brut à traiter
- `{section_type}` : type de section
- `{target_audience}` : audience cible
- `{target_register}` : registre choisi (1-4)
- `{priority}` : priorité principale
- `{word_count}` : nombre de mots du texte original
