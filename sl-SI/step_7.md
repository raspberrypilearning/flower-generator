## Naključni generator rož

Zdaj boš uporabil svoj blok `nariši rožo` {: class = "block3myblocks"} za stvarjenje stotih naključnih rož po celem odru, kadar pritisneš na tipko <kbd>r</kbd>.

![naključno cvetje](images/flower-random.png)

\--- task \---

Kodi figure dodaj nov blok z dogodki, tako da se bo na zaslonu `izbrisalo vse`{:class="block3extensions"}, `ko je pritisnjena tipka r`{: class = "block3events"}.

![cvetni sprite](images/flower-sprite.png)

```blocks3
ko je pritisnjena tipka [r v]
izbriši vse
```

\--- /task \---

\--- task \---

Dodajte v blok `ponovitev`{: class = "block3control"} in pojdite na `naključna mesta`{: class = "block3motion"} `100` -krat.

![cvetni sprite](images/flower-sprite.png)

```blocks3
ponovite (100)
  pojdi na (naključni položaj v)
konec
```

\--- /task \---

\--- task \---

Z blokom `narišite cvet`{: class = "block3myblocks"} ustvarite cvet, ki ima `naključna barva`{: class = "block3operators"} med `0` in `199`.

Koda mora zdaj izgledati tako:

![cvetni sprite](images/flower-sprite.png)

```blocks3
ko pritisnete tipko [rv]
izbrišite vse
ponovite (100) 
  pojdite na (naključni položaj v)
  narišite rožo (izberite naključno (0) do (199)) (100) (12) :: po meri
konec
```

\--- /task \---

Ta koda ustvari sto cvetov z različnimi barvami, vendar z enako velikostjo in številom cvetnih listov.

![rože samo z naključnimi barvami](images/flower-random-colour.png)

\--- task \---

Ali lahko spremenite `ko pritisnete tipko r`{: class = "block3events"}, tako da sta velikost cvetov in število cvetnih listov naključna?

\--- hints \---

\--- hint \---

Blok `nariše cvet`{: class = "block3myblocks"} naj bi izbral `naključna števila`{: class = "block3operators"} za velikost in število cvetnih listov.

\--- /hint \---

\--- hint \---

Naslednji bloki izberejo naključno velikost med `50` in `150` in naključno število cvetnih listov med `4` in `12`.

![cvetni sprite](images/flower-sprite.png)

```blocks3
(izberite naključno (50) do (150))

(izberite naključno (4) do (12))
```

\--- /hint \---

\--- hint \---

Tvoja koda bi morala izgledati tako:

![cvetni sprite](images/flower-sprite.png)

```blocks3
ko pritisnete tipko [rv]
izbrišite vse
ponovite (100) 
  pojdite na (naključen položaj v)
  narišite rožo (izberite naključno (0) do (199)) (izberite naključno (50) do (150)) (izberite naključno (4) do (12)) :: po meri
konca
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Pritisnite <kbd>r</kbd> in si oglejte naključne rože.

\--- /task \---