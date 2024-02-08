##### Le binaire dans le numérique
Pour représenter les valeurs binaires, on utilise des dispositifs n'ayant que 2 états. Par exemple, un interrupteur: ouvert ou fermé, 0 ou 1.

##### Circuits logiques
Un circuit numérique peut réagir en fonction d'un signal d'entrée. Ça s'appelle la logique du circuit. Logique. C'est un circuit logique

##### Circuits intégrés
Bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla circuit imprimé bla bla bla bla bla bla bla bla bla bla bla bla plaque bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla bla différentes technologies bla bla bla bla bla TTL, TTL.LS, CMOS bla voltage bla bla...

##### Constantes et variables booléennes

Exemples:

| Niveau logique 0 | Niveau logique 1 |
| ---------------- | ---------------- |
| Faux             | Vrai             |
| Arrêt            | Marche           |
| Bas              | Haut             |
| Low (L)          | Hight (H)        |
| Non              | Oui              |
| Ouvert           | Fermé                 |

Addition logique: OU (+)
Multiplication logique: ET (.)
Complémentation inverse: NON (-)

$B = \bar{A}$
$\bar{\bar{B}} = B$

##### Algèbre de Boole

| A                  | F0    | F1            | F2              | F3  |
| ------------------ | ----- | ------------- | --------------- | --- |
| 0                  | 0     | 0             | 1               | 1   |
| 1                  | 0     | 1             | 0               | 1   |
| Nom de la fonction | NULLE | Identique à A | Complément de A | UN    |

### Fonctions particulières

##### ET

| X   | Y   | $F_{8}$  |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 1    |

$F_{8} = X.Y$

##### OU

| X   | Y   | $F_{14}$ |
| --- | --- | -------- |
| 0   | 0   | 0        |
| 0   | 1   | 1        |
| 1   | 0   | 1        |
| 1   | 1   | 1         |

$F_{14} = X + Y$

##### NAND

$F_{7} = \overline{X.Y} = \bar{X} + \bar{Y}$

| X   | Y   | $F_{7}$ |
| --- | --- | ------- |
| 0   | 0   | 1       |
| 0   | 1   | 1       |
| 1   | 0   | 1       |
| 1   | 0   | 1       |
| 1   | 1   | 0        |

##### NOR
$F_{1} = \overline{X + Y} = \bar{X}.\bar{Y}$

| X   | Y   | $F_{1}$ |
| --- | --- | ------- |
| 0   | 0   | 1       |
| 0   | 1   | 0       |
| 1   | 0   | 0       |
| 1   | 1    |  0       |

##### OU Exclusif XOR

$F_{6} = X⊕Y = X.\bar{Y}+\bar{X}+Y$

| X   | Y   | $F_{6}$ |
| --- | --- | ------- |
| 0   | 0   | 0       |
| 0   | 1   | 1       |
| 1   | 0   | 1       |
| 1   | 1   | 0        |

##### Égalité (inverse de XOR)

$F_{9}=\overline{XY}+XY = \overline{X⊕Y}$

| X   | Y   | $F_{9}$ |
| --- | --- | ------- |
| 0   | 0   | 1       |
| 0   | 1   | 0       |
| 1   | 0   | 0       |
| 1   | 1   | 1        |

