## Générateur de fleurs aléatoires

Tu vas maintenant utiliser ton bloc `dessiner une fleur`{:class="block3myblocks"} pour créer une centaine de fleurs aléatoires sur toute la scène chaque fois que tu appuies sur la touche <kbd>r</kbd>.

![fleurs aléatoires](images/flower-random.png)

--- task ---

Ajoute un nouveau bloc événement au code de ton sprite afin que `quand la touche r est pressée`{:class="block3events"}, l'écran est `effacé`{:class="block3extensions"}.

![sprite de fleur](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

--- /task ---

--- task ---

Ajoute un bloc `répéter`{:class="block3control"} pour aller à une `position aléatoire`{:class="block3motion"} `100` fois.

![sprite de fleur](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

--- /task ---

--- task ---

Utilise le bloc `dessiner une fleur`{:class="block3myblocks"} pour créer une fleur qui a une couleur `aléatoire`{:class="block3operators"} entre `0` et `199`.

Ton code devrait maintenant ressembler à ceci:

![sprite de fleur](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  dessiner une fleur (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

Ce code crée une centaine de fleurs aux couleurs différentes, mais avec la même taille et le même nombre de pétales.

![fleurs juste avec des couleurs aléatoires](images/flower-random-colour.png)

--- task ---

Peux-tu modifier le script `quand la touche r est pressée`{:class="block3events"} pour que la taille des fleurs et le nombre de pétales soient aussi aléatoires?

--- hints ---

--- hint ---

Le bloc `dessiner une fleur`{:class="block3myblocks"} devrait `choisir des nombres aléatoires`{:class="block3operators"} pour la taille et le nombre de pétales.

--- /hint ---

--- hint ---

Les blocs suivants choisissent une taille aléatoire entre `50` et `150` et un nombre aléatoire de pétales entre `4` et `12`.

![sprite de fleur](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

--- /hint ---

--- hint ---

Ton code devrait ressembler à ceci:

![sprite de fleur](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  dessiner une fleur (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Appuie sur <kbd>r</kbd> pour voir tes fleurs aléatoires.

--- /task ---