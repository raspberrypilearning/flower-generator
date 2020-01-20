## Izziv: cvetni bloki po meri

Vsi ti cvetovi imajo enako število zunanjih in notranjih cvetnih listov, velikost notranjega cvetja pa je sorazmerna z zunanjo rožo:

![posnetek zaslona](images/flower-double-flowers.png)

Tako lahko ustvarite takšno cvetje s pomočjo `risanja dvojnega cveta`{: class = "block3myblocks"} bloka po meri, ki ima vhode za `zunanja barva`, `notranjo barvo`in `velikost`:

```blocks3
določite risanje dvojni cvet (zunanja barva) (notranja barva) (velikost :: custom-arg)
narišite cvet (zunanja barva :: custom-arg) (velikost :: custom-arg) (12) :: custom
draw flower ( notranja barva :: custom-arg) ((velikost :: custom-arg) / (2)) (20) :: custom
```

Blok `riše dvojno cvet`{: class = "block3myblocks"} lahko nariše veliko rož v istem slogu:

```blocks3
ko pritisnete tipko [dv]
zbrišite vse
pojdite na x: (-100) y: (0)
narišite dvojni cvet (160) (120) (100) :: po meri
spremenite x s (100)
narišite dvojni cvet (120) (140) (75) :: po meri
spremenite x za (75)
narišite dvojni cvet (140) (160) (50) :: po meri
```

Naredite nov blok po meri s potrebnimi vhodi, ki jih morate spremeniti, da ustvarite vrsto rože, ki vam je všeč.

Nato uporabite svoj novi blok, da ustvarite kul dizajn!