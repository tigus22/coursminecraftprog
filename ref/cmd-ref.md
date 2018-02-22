# Minecraft Commands Reference
***
## echo
`/js echo(expression)` 

Afficher un message
* Exemple: `/js echo("Bonjour")` affichera "Bonjour" à la console minecraft.  
***
## box / box0
`/js box(block, [width, height, depth])  `  
Créer un bloc.  

`/js box0(block, [width, height, depth])`   
Créer un bloc vide sans fond et sans couvercle.

* Exemple: `/js box('5')` fera apparaitre un cube de bois de chène.  Alors que `/js box('5:2')` fera apparître un cube de bois blanc.
* Tous les types de blocs sont disponibles [ici](https://minecraft-ids.grahamedgecombe.com/)
* Les paramètres `width, height, depth` sont optionnels et servent à définir la taille du bloc.
    + width = largeur
    + height = hauteur
    + depth = profondeur  
* `/js box0('42')` fera apparître un cube creux en fer.  

***
## cylinder / cylinder0
`/js cylinder(block, [radius, height])`  
Créer un cylindre plein.

`/js cylinder0(block, [radius, height])`  
Créer un cylindre vide sans fond et sans couvercle.

* Exemple: `/js cylinder0('42')` permet de créer un cylindre creux en fer, parfait pour faire une cheminée!
***
## prism / prism0

`/js prism(block, [width, depoth])` : Créer un prisme plein.

`/js prism0(block, [width, depoth])` : Créer un prisme vide.
***
## up/down/left/right/fwd/back
`/js up/down/left/right/fwd/back(numberOfBlocks)`  
Déplacer le drone vers la direction demandée  
up = vers le haut  
down = vers le bas
left = vers la gauche
right = vers la droite
fwd = vers l'avant
back = vers l'arrière

* Exemple:  
`/js left(2)` déplacera le drone de deux blocs vers la gauche.

## turn
`/js turn(numberOfTurns)`
Faire pivoter le drone de 90 degrés vers la droite.

Exemple

