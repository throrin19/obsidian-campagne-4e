```
Je vais te donner des captures d'écran (ou du texte) de blocs de statistiques de monstres D&D 4e en anglais (issus de modules officiels comme le Monster Manual, Harkenwold, etc.). Je veux que tu les convertisses en français au format Homebrewery (extension fourthed.monster), prêts à copier-coller.

## Structure de sortie exacte

{{fourthed,monster
  | Nom du monstre | Rôle Niveau X |
  | :--- | ---: |
  | Type et origine, taille | XP total |

  **Inititiave:** +X ; **Perception** +X ; [vision nocturne/crépusculaire/dans le noir si applicable] <br>
  **PV** X ; **Péril** X (ou la mention standard sbire si applicable) <br>
  **CA** X, **Vigueur** X, **Réflexe** X, **Volonté** X  
  **VD** X

  {{traits
  ## Traits
  | **Nom du trait** |
  | :--- |
  | Texte du trait |
  }}

  {{actions
  ## Actions simples
  | **{{icon M}} Nom** (mots-clés) ✦ **À volonté** |
  | :--- |
  | *Attaque:* Corps à corps X (une créature) ; +X contre CA |
  | *Réussite:* XdY + Z dégâts. |

  | **{{icon r}} Nom** (mots-clés) ✦ **À volonté** |
  | :--- |
  | *Attaque:* Distance X/Y (une créature) ; +X contre CA |
  | *Réussite:* XdY + Z dégâts. |

  ## Actions mineures
  [même structure]

  ## Actions déclenchées
  | **Nom** ✦ **À volonté / Recharge {{icon 4}} {{icon 5}} {{icon 6}}** |
  | :--- |
  | *Déclencheur:* ... |
  | *Effet (type d'action):* ... |
  }}

  {{checks
  **Compétences** ... (si présent dans la source)
  ||||
  |---|---|---|
  |**For** X (+Y)|**Dex** X (+Y)|**Sag** X (+Y)|
  |**Con** X (+Y)|**Int** X (+Y)|**Cha** X (+Y)|
  }}

  {{tail
  |||
  |---|---|
  |**Alignement** ... |**Langues** ...|

  ||
  |---|
  |**Équipement** ... (uniquement si présent dans la source)
  }}
}}

## Règles strictes

1. **Extraction littérale uniquement.** Toutes les valeurs numériques (taille, PV, CA, défenses, caractéristiques, dégâts, XP) doivent venir exactement de la source fournie. Ne jamais inventer, arrondir ou déduire une valeur absente.
2. **Ne crée aucune section vide.** Si la source n'a pas de Traits, pas d'Actions mineures, pas d'Actions déclenchées, pas de Compétences, ou pas d'Équipement — omets entièrement le bloc correspondant. N'ajoute une section que si elle contient du contenu réel de la source.
3. **Icônes :** {{icon M}} pour corps à corps, {{icon r}} pour distance, {{icon area}} pour zone/explosion (à ajuster si tu as une meilleure convention).
4. Réponds uniquement avec le bloc de code Homebrewery complet, sans texte avant/après sauf si je dois valider un choix de traduction ambigu — dans ce cas, signale-le brièvement après le bloc.

## Lexique fixe

- Skirmisher → Franc-Tireur
- Lurker → Chasseur
- Soldier → Soldat / Brute → Brute / Artillery → Artilleur / Controller → Contrôleur
- (Leader) → (Meneur)
- Minion → Sbire / Elite → Élite / Solo → Solitaire
- Bloodied → En péril (Péril X = seuil de PV)
- save ends → sauvegarde annule
- Standard/Move/Minor/Triggered Actions → Actions simples/de mouvement/mineures/déclenchées
- Trigger → Déclencheur / Effect → Effet / Attack → Attaque / Hit → Réussite / Miss → Échec
- At-Will → À volonté / Recharge → Recharge / Aura → Aura
- Melee → Corps à corps / Ranged → Distance / Close → Zone
- Speed → VD / Initiative → Inititiave (orthographe du template) / HP → PV / AC → CA
- Fortitude → Vigueur / Reflex → Réflexe / Will → Volonté
- Free Action → Action gratuite / Immediate Reaction → Réaction immédiate / Immediate Interrupt → Interruption immédiate
- Str/Dex/Con/Int/Wis/Cha → For/Dex/Con/Int/Sag/Cha
- Drake → Drake (ne pas traduire par "wyrmling")

Si un terme n'est pas listé, choisis le meilleur équivalent cohérent avec le lexique D&D 4e français. Si j'ai déjà utilisé un nom particulier pour un monstre ou un pouvoir ailleurs dans ma campagne, je te le préciserai — sinon propose ta meilleure traduction et je validerai.
```