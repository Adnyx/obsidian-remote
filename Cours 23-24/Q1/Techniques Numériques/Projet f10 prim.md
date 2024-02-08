
7 portes
#### Table de vérité

| D   | C   | B   | A   | F     |
| --- | --- | --- | --- | ----- |
| 0   | 0   | 0   | 0   | 0     |
| 1   | 0   | 0   | 0   | 0     |
| 0   | 1   | 0   | 0   | ==1== |
| 1   | 1   | 0   | 0   | ==1== |
| 0   | 0   | 1   | 0   | 0     |
| 1   | 0   | 1   | 0   | ==1== ! |
| 0   | 1   | 1   | 0   | ==1== |
| 1   | 1   | 1   | 0   | ==1== !|
| 0   | 0   | 0   | 1   | ==1== |
| 1   | 0   | 0   | 1   | ==1== |
| 0   | 1   | 0   | 1   | 0     |
| 1   | 1   | 0   | 1   | 0     |
| 0   | 0   | 1   | 1   | ==1== |
| 1   | 0   | 1   | 1   | ==1== |
| 0   | 1   | 1   | 1   | 0     |
| 1   | 1   | 1   | 1   | 0     |


#### Tableau de Karnaugh

| __DC/BA__ | __00__  | __01__  |__11__  | __10__  |
| ----- | --- | --- | --- | --- |
| __00__    |     | 1    |1     |     |
| __01__    |  1   |     |     | 1    |
| __11__    |   1  |     |     |  1   |
| __10__      |     | 1    | 1    | 1    |

#### Pour les 1
$F10 = \bar{C}A + C \bar{A} + DB \bar{A}$
$F10 = \overline{\overline{\bar{C}A + C \bar{A} + DB \bar{A}}}$
$F10 = \overline{\overline{\bar{C}A} . \overline{C\bar{A}} . \overline{DB \bar{A}}}$


#### Pour les 0 (inverseuse à la fin)

$F10 = \bar{D}\bar{C}\bar{A}+ \bar{B} \bar{A} \bar{C} +AC$

$F10 = \bar{A}\bar{C}(\bar{D}+\bar{B})+AC$

$F10 = \bar{A}\bar{C}(\overline{DB})+AC$ # De morgan

$F10 = \bar{A}\bar{C} \overline{(\overline{\overline{DB})+AC}}$

$F10 = \bar{A}\bar{C} \overline{(\overline{\overline{DB}}).\overline{AC}}$

$F10 = \bar{A}\bar{C} \overline{(DB).\overline{AC}}$


//
$F10 = \overline{\overline{\bar{D}\bar{C}\bar{A}+ \bar{B} \bar{A} \bar{C} +AC}}$
$F10 = \overline{\overline{\bar{D}\bar{C}\bar{A}} . \overline{\bar{B} \bar{A} \bar{C} } .\overline{AC}}$
//
