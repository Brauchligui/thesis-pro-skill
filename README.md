# thesis-pro

**Claude Code Skill** | Assistant expert pour la redaction de theses professionnelles

*Expert assistant for professional thesis writing*

---

## FR - Francais

### Description

**thesis-pro** est un skill pour [Claude Code](https://claude.ai/code) qui vous accompagne tout au long de la redaction de votre these professionnelle (Executive MBA, MS, Doctorat). De l'ideation a la revision finale, Dr. Alex - votre conseiller academique virtuel - vous guide avec rigueur et bienveillance.

### Fonctionnalites

- **5 phases completes** : Ideation, Recherche, Structure, Redaction, Revision
- **44 techniques de brainstorming** integrees (SCAMPER, Six Chapeaux, Design Thinking...)
- **4 styles de citation** : APA, Chicago, Harvard, Vancouver
- **Bilingue FR/EN** : communication et redaction dans les deux langues
- **Workflows structures** : chaque etape est guidee pas a pas avec des sous-etapes detaillees
- **Revue de litterature guidee** en 6 etapes (concepts fondateurs → positionnement → synthese)
- **Analyse sectorielle** avec Porter, PESTEL, cartographie des acteurs
- **Conception methodologique** : paradigme, collecte, echantillonnage, analyse, ethique

### Menu (13 commandes)

| # | Cmd | Description |
|---|-----|-------------|
| 1 | `MH` | Menu - Reafficher le menu |
| 2 | `CH` | Chat - Discuter librement avec Dr. Alex |
| 3 | `BS` | Brainstorm - Explorer ou affiner sa problematique |
| 4 | `LR` | Literature Review - Revue de litterature guidee |
| 5 | `FS` | Find Studies - Rechercher des etudes de reference |
| 6 | `SA` | Sector Analysis - Analyse marche/sectorielle |
| 7 | `MT` | Methodology - Concevoir sa methodologie de recherche |
| 8 | `OL` | Outline - Creer ou affiner son plan de these |
| 9 | `WR` | Write - Aide a la redaction d'une section |
| 10 | `BIB` | Bibliography - Gerer ses sources et citations |
| 11 | `RV` | Review - Verifier coherence et style academique |
| 12 | `CFG` | Config - Modifier ses preferences |
| 13 | `DA` | Dismiss - Quitter l'assistant |

### Installation

1. Copiez le contenu de ce repo dans votre projet :
   ```bash
   # Depuis la racine de votre projet
   mkdir -p .claude/skills/thesis-pro
   cp -r <chemin-vers-ce-repo>/* .claude/skills/thesis-pro/
   ```

2. Copiez le template de configuration :
   ```bash
   cp .claude/skills/thesis-pro/config-template.yaml .claude/skills/thesis-pro/config.yaml
   ```

3. Lancez le skill dans Claude Code :
   ```
   /thesis-pro
   ```
   Dr. Alex vous guidera pour configurer vos preferences au premier lancement.

### Utilisation

```
> /thesis-pro

🎓 Bonjour Guillaume ! Je suis Dr. Alex, votre conseiller academique.

Que souhaitez-vous faire aujourd'hui ?

 1. [MH] Menu - Reafficher ce menu
 2. [CH] Chat - Discuter librement
 3. [BS] Brainstorm - Explorer ma problematique
 4. [LR] Literature Review - Revue de litterature
 ...

> 3
```

---

## EN - English

### Description

**thesis-pro** is a [Claude Code](https://claude.ai/code) skill that guides you through your entire professional thesis journey (Executive MBA, MS, Professional Doctorate). From ideation to final review, Dr. Alex - your virtual academic advisor - guides you with rigor and encouragement.

### Features

- **5 complete phases**: Ideation, Research, Structure, Writing, Review
- **44 brainstorming techniques** built-in (SCAMPER, Six Hats, Design Thinking...)
- **4 citation styles**: APA, Chicago, Harvard, Vancouver
- **Bilingual FR/EN**: communication and writing in both languages
- **Structured workflows**: each step is guided with detailed sub-steps
- **Guided literature review** in 6 steps (foundational concepts → positioning → synthesis)
- **Sector analysis** with Porter, PESTEL, actor mapping
- **Methodology design**: paradigm, data collection, sampling, analysis, ethics

### Installation

1. Copy this repo's contents into your project:
   ```bash
   # From your project root
   mkdir -p .claude/skills/thesis-pro
   cp -r <path-to-this-repo>/* .claude/skills/thesis-pro/
   ```

2. Copy the configuration template:
   ```bash
   cp .claude/skills/thesis-pro/config-template.yaml .claude/skills/thesis-pro/config.yaml
   ```

3. Launch the skill in Claude Code:
   ```
   /thesis-pro
   ```
   Dr. Alex will guide you through configuration on first launch.

---

## Structure

```
thesis-pro-skill/
├── README.md
├── LICENSE
├── .gitignore
├── skill.json              # Skill metadata
├── skill.md                # Main skill definition (Dr. Alex persona + menu)
├── config-template.yaml    # Configuration template (copy to config.yaml)
├── data/
│   ├── brainstorming-techniques.csv    # 44 techniques
│   ├── citation-styles/
│   │   ├── apa.md
│   │   ├── chicago.md
│   │   ├── harvard.md
│   │   └── vancouver.md
│   └── templates/
│       ├── research-template.md
│       └── thesis-brief-template.md
└── workflows/
    ├── 1-ideation/         # Brainstorming & topic exploration
    ├── 2-research/         # Literature review, studies, sector analysis, methodology
    ├── 3-structure/        # Thesis outline creation
    ├── 4-writing/          # Section drafting
    └── 5-review/           # Bibliography & coherence check
```

## License

MIT - see [LICENSE](LICENSE)

## Author

Guillaume Brauchli - [@Brauchligui](https://github.com/Brauchligui)
