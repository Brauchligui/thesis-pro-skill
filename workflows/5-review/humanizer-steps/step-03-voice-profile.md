# Étape 3 — Profil de voix de l'auteur

## Objectif
Charger ou créer un profil stylistique unique qui capture la "voix" naturelle de l'auteur, pour guider l'humanisation.

## Instructions pour l'agent

### 1. Vérifier l'existence du profil
Cherchez le fichier `data/voice-profile.md` dans le répertoire du skill.

#### Si le profil EXISTE :
- Chargez-le et présentez un résumé rapide à l'utilisateur
- Demandez : "Ce profil est-il toujours fidèle à votre style, ou souhaitez-vous l'affiner ?"
- Si OK → passez à l'étape 4
- Si mise à jour → procédez comme pour une création, en partant du profil existant

#### Si le profil N'EXISTE PAS :
- Informez l'utilisateur : "Pour humaniser efficacement, j'ai besoin de comprendre VOTRE façon d'écrire. Cela prend 5 minutes et ne se fait qu'une seule fois."
- Passez à la section Création ci-dessous

### 2. Création du profil de voix

#### A. Collecte d'échantillons
Demandez à l'utilisateur de fournir **1 à 3 échantillons** de texte qu'il a **réellement écrit lui-même** (pas généré par IA). Suggestions :
- Un e-mail professionnel important
- Un passage d'un ancien rapport ou mémoire
- Des notes de réunion rédigées
- Un message LinkedIn ou un post
- Un ancien devoir, article ou billet

Minimum recommandé : **300 mots** au total.

#### B. Analyse des échantillons
Analysez systématiquement les dimensions suivantes :

**Syntaxe & rythme**
- Longueur moyenne des phrases (courtes/moyennes/longues)
- Variation de longueur (burstiness : forte/moyenne/faible)
- Structures préférées (phrases simples, subordonnées, incises, parenthèses)
- Usage de la ponctuation atypique (tirets, points de suspension, parenthèses, point-virgules)

**Vocabulaire & registre**
- Niveau de langue naturel (soutenu, courant, familier, mixte)
- Mots fétiches ou expressions récurrentes
- Anglicismes ou termes techniques utilisés naturellement
- Degré de jargon sectoriel

**Voix & posture**
- Usage du "je" / "nous" / formes impersonnelles
- Degré d'affirmation (affirme directement vs nuance systématiquement)
- Présence d'humour, d'ironie, de sarcasme
- Tendance à l'anecdote ou à l'exemple concret
- Interpellations au lecteur (questions rhétoriques, "vous voyez ce que je veux dire")

**Organisation & flow**
- Transitions préférées (quels connecteurs utilise-t-il naturellement ?)
- Longueur des paragraphes
- Tendance à la digression ou au fil très linéaire
- Usage de listes vs prose continue

**Marqueurs personnels**
- Tics d'écriture (répétitions inconscientes, tournures signature)
- Niveau d'émotion dans l'écriture (sobre vs expressif)
- Rapport au doute (assume l'incertitude vs projette la certitude)

#### C. Synthèse et validation
Présentez le profil à l'utilisateur sous cette forme :

```
PROFIL DE VOIX — {user_name}

Rythme : Phrases moyennes (15-20 mots) avec pics courts pour l'emphase.
         Burstiness élevée — alterne rafales courtes et développements longs.

Registre : Courant-soutenu. Mélange naturel de précision technique et
           d'expressions directes. Anglicismes assumés ("pricing", "market access").

Voix : Usage fréquent du "je". Affirmatif mais honnête sur les limites.
       Humour discret par l'autodérision. Aime les exemples concrets tirés
       de son expérience professionnelle.

Transitions favorites : "Concrètement", "Or", "Le problème c'est que",
                        "Dit autrement", tirets longs pour les incises.

Marqueurs signature : Questions rhétoriques suivies de leur réponse.
                      Parenthèses pour les commentaires personnels.
                      Tendance à nuancer ses propres affirmations dans
                      la phrase suivante.
```

Demandez à l'utilisateur de valider, corriger ou compléter.

### 3. Sauvegarde
Sauvegardez le profil validé dans `data/voice-profile.md` pour réutilisation future.

## Note importante
Le profil de voix est un **document vivant**. Suggérez à l'utilisateur de le mettre à jour s'il estime que son style a évolué ou si les résultats d'humanisation ne lui ressemblent pas assez.
