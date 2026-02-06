# 📖 Workflow: Gestion de la Bibliographie

## Objectif
Aider l'étudiant à organiser, formater et gérer ses sources bibliographiques de manière rigoureuse.

---

## Instructions pour l'Agent

### Étape 1: État des lieux

Demander à l'utilisateur:
> "Où en êtes-vous avec votre bibliographie ?
>
> 1. Je n'ai pas encore commencé à organiser mes sources
> 2. J'ai des sources en vrac que je veux organiser
> 3. J'ai une bibliographie mais je veux vérifier le formatage
> 4. Je veux ajouter de nouvelles sources
> 5. Je veux convertir ma bibliographie dans un autre format"

Rappeler le format choisi: **{citation_style}**

---

### Étape 2: Organisation des sources

#### Catégorisation recommandée

```markdown
## Bibliographie

### Sources académiques
#### Articles de revues à comité de lecture
#### Ouvrages et chapitres d'ouvrages
#### Thèses et mémoires
#### Working papers et conférences

### Sources professionnelles
#### Rapports sectoriels et études
#### Publications d'organisations
#### Articles de presse spécialisée

### Sources institutionnelles
#### Textes législatifs et réglementaires
#### Rapports publics
#### Statistiques officielles

### Sources web (avec précaution)
#### Sites d'organisations reconnues
#### Bases de données en ligne
```

---

### Étape 3: Vérification du formatage

#### Charger le guide de style approprié
Lire: `data/citation-styles/{citation_style}.md`

#### Checklist de formatage

| Élément | Vérifié | Commentaire |
|---------|---------|-------------|
| Ordre alphabétique (si applicable) | ⬜ | |
| Cohérence du format | ⬜ | Toutes les entrées suivent le même modèle |
| Noms d'auteurs | ⬜ | Format identique partout |
| Italiques correctement placés | ⬜ | Titres de livres/revues |
| Ponctuation | ⬜ | Points, virgules aux bons endroits |
| DOI ou URL | ⬜ | Présents pour les sources en ligne |
| Dates d'accès | ⬜ | Pour les sources web |
| Pas de doublons | ⬜ | |

---

### Étape 4: Formatage d'une source

Si l'utilisateur fournit une source à formater:

1. Identifier le type de source (livre, article, site web, etc.)
2. Extraire les métadonnées nécessaires
3. Appliquer le format `{citation_style}`
4. Retourner la référence formatée

**Template de demande:**
> "Pour formater cette source, j'ai besoin de:
> - Type (livre, article, site web...)
> - Auteur(s)
> - Titre
> - Année
> - [Autres champs selon le type]"

---

### Étape 5: Outils recommandés

Informer l'utilisateur des outils de gestion bibliographique:

| Outil | Gratuit | Points forts |
|-------|---------|--------------|
| **Zotero** | ✅ | Open source, plugins Word/Google Docs |
| **Mendeley** | ✅ | Bon pour PDF, réseau social |
| **EndNote** | ❌ | Puissant, standard institutionnel |
| **Citavi** | ❌ | Allemand, très complet |

**Pour le style {citation_style}:**
- S'assurer que le style est installé dans l'outil
- Vérifier la sortie (parfois des erreurs)

---

### Étape 6: Détection de problèmes courants

#### Erreurs fréquentes à vérifier:
- **"et al." mal utilisé**: Vérifier le seuil selon le style
- **Majuscules incohérentes**: Titre en majuscule ou minuscule ?
- **Abréviations de journaux**: Selon le style
- **Sources secondaires**: Citer l'original si possible
- **Auto-citations excessives**: Équilibre nécessaire

---

### Étape 7: Cohérence citations ↔ bibliographie

Vérifier:
- Chaque citation dans le texte a une entrée en bibliographie
- Chaque entrée en bibliographie est citée dans le texte
- Les années correspondent

> "Voulez-vous que je vérifie la cohérence entre vos citations et votre bibliographie ? Si oui, partagez-moi les deux."

---

### Étape 8: Livrable

Si l'utilisateur le souhaite, créer ou mettre à jour:

```markdown
# Bibliographie - [Titre de la thèse]
Format: {citation_style}
Dernière mise à jour: [Date]

---

## Articles de revues à comité de lecture

[Entrées formatées]

## Ouvrages

[Entrées formatées]

## Rapports et études

[Entrées formatées]

## Sources web

[Entrées formatées]

---

## Notes
- Nombre total de sources: [X]
- Sources à retrouver/compléter: [Liste]
```

Sauvegarder dans: `{output_folder}/5-review/bibliography.md`

---

## Conseils pour l'Agent
- La rigueur bibliographique reflète la rigueur de la recherche
- Encourager à noter les références IMMÉDIATEMENT lors de la lecture
- Rappeler qu'un DOI est préférable à une URL
- Si une source semble douteuse, alerter l'utilisateur
- Proposer de créer un fichier .bib si l'utilisateur utilise LaTeX
