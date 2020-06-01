## Défi: blocs de fleurs personnalisés

Ces fleurs ont toutes le même nombre de pétales extérieurs et intérieurs, et la taille de la fleur intérieure est proportionnelle à la fleur extérieure qui la contient:

![capture d'écran](images/flower-double-flowers.png)

Tu peux créer des fleurs comme cela avec l'aide d'un bloc personnalisé `dessiner une fleur double`{:class="block3myblocks"} qui a des entrées pour `couleur bordure`, `couleur remplissage`, et `taille`:

```blocks3
define dessiner une fleur double (couleur bordure) (couleur remplissage) (taille :: custom-arg)
dessiner une fleur (couleur bordure :: custom-arg) (taille :: custom-arg) (12) :: custom
dessiner une fleur (couleur remplissage :: custom-arg) ((taille :: custom-arg) / (2)) (20) :: custom
```

Le bloc `dessiner une fleur double`{:class="block3myblocks"} peut dessiner beaucoup de fleurs dans le même style:

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
dessiner une fleur double (160) (120) (100) :: custom
change x by (100)
dessiner une fleur double (120) (140) (75) :: custom
change x by (75)
dessiner une fleur double (140) (160) (50) :: custom
```

Créer un nouveau bloc personnalisé avec les entrées nécessaires que tu dois être en mesure de changer pour créer un type de fleur que tu aimes.

Utilise ensuite ton nouveau bloc pour créer un design cool!