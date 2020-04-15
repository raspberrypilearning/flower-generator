## Uitdaging: aangepaste bloemblokken

Deze bloemen hebben allemaal hetzelfde aantal buitenste en binnenste bloembladen, en de grootte van de binnenste bloem staat in verhouding tot de buitenste bloem:

![schermafbeelding](images/flower-double-flowers.png)

Je kunt dergelijke bloemen maken met behulp van een `teken dubbele bloem`{:class="block3myblocks"} blok met invoer voor `kleur buitenkant`, `kleur binnenkant`en `grootte`:

```blocks3
definieer teken dubbele bloem (kleur buitenkant) (kleur binnenkant) (grootte :: custom-arg)
teken bloem (kleur buitenkant :: custom-arg) (grootte :: custom-arg) (12) :: custom
teken bloem (kleur binnenkant :: custom-arg) ((grootte :: custom-arg) / (2)) (20) :: custom
```

Het blok `teken dubbele bloem`{:class="block3myblocks"} kan veel bloemen in dezelfde stijl tekenen:

```blocks3
wanneer [d v] is ingedrukt
wis alles
ga naar x: (-100) y: (0)
teken dubbele bloem (160) (120) (100) :: custom
verander x met (100)
teken dubbele bloem (120) (140) (75) :: custom
verander x met (75)
teken dubbele bloem (140) (160) (50) :: custom
```

Maak een nieuw aangepast blok met de nodige invoer die je moet kunnen veranderen om de bloem te maken die je leuk vindt.

Gebruik dan je nieuwe blok om een cool ontwerp te maken!