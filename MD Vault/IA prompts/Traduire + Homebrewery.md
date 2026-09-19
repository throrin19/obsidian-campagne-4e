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
4. **Icônes :** 
   - `{{icon M}}` (majuscule) : le pouvoir effectue lui-même un jet d'attaque corps à corps. 
   - `{{icon m}}` (minuscule) : pouvoir corps à corps qui n'effectue pas lui-même de jet d'attaque mais utilise/complète un autre pouvoir d'attaque (ex: une feinte qui déclenche une attaque de base). 
   - `{{icon r}}` : attaque à distance. 
   - `{{icon c}}` : attaque de zone/explosion/décharge rapprochée. 
   - Pas d'icône pour un pouvoir sans composante d'attaque (téléportation pure, illusion, effet). 
   - Recharge sur dés : une icône par valeur, ex. `{{icon 5}} {{icon 6}}` — jamais de texte "Recharge X, Y". 
5. **Nom du pouvoir :** garder le mot-clé entre parenthèses juste après le nom (ex: "(arme)", "(téléportation)", "(charme)", "(illusion)") ET le répéter après la virgule dans le tag d'usage après ✦ (ex: "✦ **À volonté, arme**"). 
6. **En-tête du monstre :** ne jamais ajouter de suffixe lettre (ex: "(B)") au nom, même si présent dans la source. Pour un monstre présenté en groupe (ex: "2 Dryad Hunters"), le nom du statbloc reste au singulier et le PX affiché est celui d'un seul exemplaire, sans "chacune". Taille toujours abrégée (M, P, G, etc.), jamais en toutes lettres. 
7. **Mise en forme :** deux espaces en fin de ligne (retour à la ligne Markdown) après les lignes CA/Vigueur/Réflexe/Volonté, Jets de sauvegarde/Points d'action, et VD dans l'en-tête de stats. Orthographe imposée par le template : "Inititiave" (pas "Initiative"). 
8. Si je fournis deux versions du même monstre (une française déjà convertie dans un format, une anglaise dans un autre), précise-moi lequel utiliser si ce n'est pas clair, et respecte le format demandé sans le changer sans qu'on en discute. 
9. Si j'ai déjà traduit un nom de monstre/pouvoir dans une fiche précédente, réutilise ce nom tel quel plutôt que de le retraduire différemment.

## Cas particulier : monstre fourni en MM3 (anglais) + MM1 (français) déjà traduit

Quand je te fournis deux versions du même monstre — une en anglais au format MM3 (Attaque/Réussite séparées, maths retravaillées) et une déjà traduite en français au format MM1 (souvent en format compact) — traduis la version **MM3**, mais réutilise le wording français déjà établi dans la version MM1 (noms de pouvoirs, termes de condition, etc.) plutôt que de retraduire depuis l'anglais.

Règles :
1. **Les stats viennent toujours du MM3** (PV, CA, défenses, dégâts, DD) — jamais du MM1, même en cas d'écart entre les deux versions.
2. **Le MM1 est une référence de vocabulaire uniquement**, pas une source de contenu : si le MM1 a un pouvoir absent du MM3 (ou l'inverse), ne garde que ce qui figure dans le MM3 à convertir.
3. Si un terme du MM3 n'a pas d'équivalent dans le MM1 fourni (pouvoir nouveau), traduis-le toi-même selon le lexique fixe et signale ton choix.

## Cas inverse : convertir un monstre en maths MM1 vers les maths MM3

Si je te demande de mettre à jour un monstre plus ancien (maths MM1) vers les maths MM3, recalcule CA/Vigueur/Réflexe/Volonté/PV/dégâts à partir des profils par rôle et des tables de dégâts par niveau (fichier de référence *Créer des monstres.md*), en conservant le rôle, le niveau, les pouvoirs et le fluff d'origine. Signale-moi les valeurs qui changent significativement par rapport à l'original.

## Format des objets magiques

- Objet unique (non à paliers) : pas de tableau de progression multi-niveaux, pas de mention "Rare" en tête.
  {{basics}} : juste **Bonus d'amélioration** et **Critique** (ou **Emplacement**/**Prix** si pas de bonus d'attaque).
  {{properties}} : les propriétés passives multiples (préfixées ✦) sont regroupées dans UN SEUL tableau sous un seul en-tête **Propriété**, pas un tableau par ligne.
- Objet à paliers (ex: anneau +1/+2/+3) : garde le tableau de progression complet.

## Format des pièges (hazards)

{{fourthed,hazard}} avec Détection/Initiative, PV/CA/défenses seulement si présents dans la source, Immunités, puis {{actions}} pour Déclencheur/Attaque/Réussite/Échec/Effet, et {{counters}} pour les contre-mesures.

## Lexique fixe

`Skirmisher→Franc-Tireur, Lurker→Chasseur, Soldier→Soldat, Brute→Brute, Artillery→Artilleur, Controller→Contrôleur, (Leader)→(Meneur), Minion→Sbire, Elite→Élite, Solo→Solitaire, Bloodied→En péril (Péril X), save ends→sauvegarde annule, restrained→maîtrisé(e) (terme MM1, jamais "immobilisé(e)"), low-light vision→vision nocturne, Standard/Move/Minor/Triggered Actions→Actions simples/de mouvement/mineures/déclenchées, Trigger→Déclencheur, Effect→Effet, Attack→Attaque, Hit→Réussite, Miss→Échec, At-Will→À volonté, Melee→Corps à corps, Ranged→Distance, Close→Zone/proximité, Speed→VD, Initiative→Inititiave (orthographe du template), HP→PV, AC→CA, Fortitude→Vigueur, Reflex→Réflexe, Will→Volonté, Free Action→Action gratuite, Immediate Reaction→Réaction immédiate, Immediate Interrupt→Interruption immédiate, Str/Dex/Con/Int/Wis/Cha→For/Dex/Con/Int/Sag/Cha, Drake→Drake (jamais "wyrmling")`

Réponds uniquement avec le bloc de code complet, sans texte avant/après sauf si tu dois me signaler une ambiguïté (XP manquant, valeur illisible, choix de traduction).