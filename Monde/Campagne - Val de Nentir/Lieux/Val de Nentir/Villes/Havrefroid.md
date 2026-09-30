---
Région: "[[Val de Nentir]]"
Type: Village
Capitale: Non
---
# Carte

![[havrefroid.png]]

# Lieux importants

1. Porte et remparts extérieurs : Deux gardes sont postés à la porte extérieure. 
2. Auberge de Wrafton : Cette auberge et taverne spacieuse sert de lieu de rencontre public pour la région. 
3. Place du March : Un jour sur deux environ, des chariots se rassemblent sur la place pour offrir des marchandises aux habitants de Havrefroid. Une fois par semaine, le jour officiel du Marché appelle les villageois à faire leurs courses et à socialiser sur la place. 
4. Écuries : Les voyageurs peuvent y mettre leurs montures en écurie pour 2 pièces d’or par jour. Rarement (d20 : 1-2), le maître d’écurie a un cheval de monte ou un chariot à vendre.
5. Forge: Thair Cogne-charbon dispose d’un stock dearmes simples, mais les armes militaires nécessitent un jour pour être achevées, et les armes supérieures nécessitent une semaine de travail. 
6. Tour de Valthrun: Valthrun le Prescient est un sage et un érudit qui connaît fort bien la région. 
7. Grand bazar de Bairwin : Bairwin Wildarson est le propriétaire de ce commerce. 
8. Guilde des Combattants : Rond Kelfem, capitaine de la Milice de Havrefroid, supervise également la Guilde des Combattants, qui entraîne les villageois à l’utilisation des armes et des boucliers. 
9. Logements : Les résidents du village qui ne possèdent pas de ferme ou qui travaillent à l’intérieur des murs du village vivent dans ces appartements ou dans des maisons (marquées H sur la carte) sur le côté ouest du village. 
10. Temple : Cette grande structure en pierre est le temple du village. Parmi les plusieurs divinités adorées par les locaux, Avandra, déesse de la chance et du changement, est la plus importante. 
11. Porte intérieure : Deux gardes sont stationnés ici et interrogent quiconque cherche à rendre visite à Lord Padraig dans son manoir. 
12. Réserves de siège : De l’eau, de la farine et d’autres denrées alimentaires de base sont stockées ici pour nourrir les villageois en cas de siège. 
13. Caserne : La Milice y dort en dortoir. 
14. Manoir : Dotée de cinq domestiques, la maison seigneuriale où Lord Padraig vit avec sa femme et ses quatre fils est un bel exemple d’architecture en pierre dans un village par ailleurs construit en bois et en chaume.

# Habitants importants

```base
properties:
  note.type:
    displayName: Type
  note.statut:
    displayName: Statut
  note.updated:
    displayName: Mis à jour
  file.name:
    displayName: Nom
views:
  - type: cards
    name: Notes
    filters:
      and:
        - Type == "Pnj"
        - note["Ville/Village"] == link("Havrefroid")
    order:
      - file.name
      - statut
      - Image
      - Alignement
      - Profession
      - Relation
    sort:
      - property: file.name
        direction: ASC

```