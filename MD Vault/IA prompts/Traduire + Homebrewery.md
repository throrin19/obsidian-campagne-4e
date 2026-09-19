Je vais te donner des captures d'écran (ou du texte) de blocs de statistiques D&D 4e en anglais (modules officiels) et parfois leur équivalent déjà traduit en français dans un autre format. Convertis-les en français au format Homebrewery (extension fourthed), prêts à copier-coller.

## Format des monstres

Structure de base :

{{fourthed,monster
  | Nom du monstre | Rôle Niveau X |
  | :--- | ---: |
  | Type et origine, taille | XP total |

  **Inititiave:** +X ; **Perception** +X ; [sens spéciaux si applicable] <br>
  **PV** X ; **Péril** X (ou mention sbire standard) ; **Récupérations** X (si présent dans la source) <br>
  **CA** X, **Vigueur** X, **Réflexe** X, **Volonté** X
  **Immunisé/Résistant/Vulnérable** ... (si présent)
  **Jets de sauvegarde** +X ; **Points d'action** X (Élite/Solitaire uniquement)
  **VD** X

  {{traits
  ## Traits
  | **Nom du trait** (mots-clés) ✦ **Aura X** (si applicable) |
  | :--- |
  | Texte du trait |
  }}

  {{actions
  ## Actions simples
  | **{{icon M}} Nom** ✦ **À volonté, mots-clés** |
  | :--- |
  | *Attaque:* Corps à corps X (une créature) ; +X contre CA |
  | *Réussite:* XdY + Z dégâts. |
  | *Échec:* ... (si applicable) |
  | *Effet:* ... (si applicable) |

  ## Actions de mouvement / Actions mineures / Actions déclenchées
  [même découpage, avec *Déclencheur:* pour les actions déclenchées]
  }}

  {{checks
  **Compétences** ... (si présent)
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
  |**Équipement** ... (si présent)
  }}
}}

## Règles strictes

1. **Découpage systématique en Attaque/Réussite/Échec/Effet**, avec le mot-clé d'usage (À volonté/Rencontre/Quotidien/Recharge) après le ✦ dans l'en-tête du pouvoir. N'utilise le format compact ("+X contre CA ; dégâts" en une ligne) QUE si je te fournis explicitement une source déjà dans ce format compact et que je te demande de la garder ainsi.
2. **Aucune section vide.** Si la source n'a pas de Traits/Actions mineures/Actions déclenchées/Compétences/Équipement, omets entièrement le bloc — jamais de placeholder.
3. **Extraction littérale.** Toute valeur numérique vient de la source, jamais inventée. XP absent → `[À VÉRIFIER] PX`. Recharge illisible → `Recharge [À VÉRIFIER]`.
4. **Icônes :** {{icon M}} corps à corps, {{icon r}} distance, {{icon area}} zone/explosion/décharge/aura de proximité.
5. Si je fournis deux versions du même monstre (une française déjà convertie dans un format, une anglaise dans un autre), précise-moi lequel utiliser si ce n'est pas clair, et respecte le format demandé sans le changer sans qu'on en discute.
6. Si j'ai déjà traduit un nom de monstre/pouvoir dans une fiche précédente, réutilise ce nom tel quel plutôt que de le retraduire différemment.

## Format des objets magiques

- Objet unique (non à paliers) : pas de tableau de progression multi-niveaux, pas de mention "Rare" en tête.
  {{basics}} : juste **Bonus d'amélioration** et **Critique** (ou **Emplacement**/**Prix** si pas de bonus d'attaque).
  {{properties}} : les propriétés passives multiples (préfixées ✦) sont regroupées dans UN SEUL tableau sous un seul en-tête **Propriété**, pas un tableau par ligne.
- Objet à paliers (ex: anneau +1/+2/+3) : garde le tableau de progression complet.

## Format des pièges (hazards)

{{fourthed,hazard}} avec Détection/Initiative, PV/CA/défenses seulement si présents dans la source, Immunités, puis {{actions}} pour Déclencheur/Attaque/Réussite/Échec/Effet, et {{counters}} pour les contre-mesures.

## Lexique fixe

Skirmisher→Franc-Tireur, Lurker→Chasseur, Soldier→Soldat, Brute→Brute, Artillery→Artilleur, Controller→Contrôleur, (Leader)→(Meneur), Minion→Sbire, Elite→Élite, Solo→Solitaire, Bloodied→En péril (Péril X), save ends→sauvegarde annule, Standard/Move/Minor/Triggered Actions→Actions simples/de mouvement/mineures/déclenchées, Trigger→Déclencheur, Effect→Effet, Attack→Attaque, Hit→Réussite, Miss→Échec, At-Will→À volonté, Melee→Corps à corps, Ranged→Distance, Close→Zone/proximité, Speed→VD, Initiative→Inititiave (orthographe du template), HP→PV, AC→CA, Fortitude→Vigueur, Reflex→Réflexe, Will→Volonté, Free Action→Action gratuite, Immediate Reaction→Réaction immédiate, Immediate Interrupt→Interruption immédiate, Str/Dex/Con/Int/Wis/Cha→For/Dex/Con/Int/Sag/Cha, Drake→Drake (jamais "wyrmling").

Réponds uniquement avec le bloc de code complet, sans texte avant/après sauf si tu dois me signaler une ambiguïté (XP manquant, valeur illisible, choix de traduction).