### 1. Tension
Tension(Différence de potentiel): $U$ en volt
Excès d'élections: $V_{P}$
Manque d'électrons: $V_{N}$
Si on a le nbr d'électrons d'une pile, sa tension est un delta entre le + et le -. $U_{PN}=V_{P}-V_{N}$
$U = \frac{W}{Q}$ où $W$ est l'énergie (en Joules) et $Q$ est la charge électrique (en Coulombs)
Sur un schéma, la différence de potentiel se représente par une flèche partant du potentiel le plus bas vers le plus haut
### 2. Intensité
L'intensité (déplacement des électrons): $I$ en ampères
$I = \frac{Q}{t}$ où $t$ est le temps en secondes(/!\\)

### 3. Résistance
Les matériaux ont des propriétés différentes. Une de ces propriété est la résistance($R$ en Ohm $\Omega$): l'aptitude d'un matériau à résister au courant électrique.
##### 3.1. Loi de Pouillet: 
$R =\frac{\rho.l}{S}$ où $\rho$ est la résistivité du matériau($\Omega.m$), $l$ est la longueur en $m$ et S et la surface en $m^2$
/!\\ Cette loi n'est valable qu'à une température de 0°C
/!\\ Le $\rho$ du cuivre est de $1,6.10^{-8}\Omega.m$

##### 3.2. Loi de Mathiessen: 
$R_{T}=R_{0}.(1+\alpha.T)$ où $R_{T}$ est la R à la température voulue, $R_{0}$ est R à 0°C, $\alpha$ est le coefficient de température($°C^{-1}$) et T la température en °C
Cette loi s'applique aussi sur la résistivité des matériaux: $\rho_{T}=\rho_{0}(1+\alpha T)$ où $\alpha = 0,004°C^{-1}$ 

Relation entre $U, I$ et $R$: $R=\frac{U}{I}$

##### 3.3 Propriété des résistances
En série: $R_{éq}=\sum R_{série}$
En parallèle (3 ou +): $R_{éq}=\frac{1}{R_{1}}+\frac{1}{R_{2}}+\frac{1}{R_{3}},\dots$
En parallèle (2): $R_{éq}= \frac{R_{1}.R_{2}}{R_{1}+R_{2}}$
### 4. Puissance
$P = U.I$ où P est la puissance en watt

### 5. L'effet Joule
On a vu pour la résistance que les matériaux bloquaient le passage des électrons. En bloquant le passage, l'énergie des électrons se traduit en chaleur. $W_{cal}=R.I^{2}.t$

### 6. Lois de Kirchhoff
##### 6.1 Loi des noeuds

$\sum alg I_{entrant}=\sum alg I_{sortant}$
![[Pasted image 20240118140950.png|200]]
##### 6.2 Loi des mailles 
$\sum alg U_{maille} = 0V$ (dans un sens)


##### 6.3 Autres propriétés
Dans une même portion de circuit, l'intensité est identique en tout points
$I_{AB} = I_{BC} = I_{tot}$

Dans une même portion de circuit, les U s'additionnent
$U_{AB}+U_{BC}=U_{tot}$

##### 6.4 Théorème de Kennelly
Il permet de simplifier les circuits lorsqu'il est impossible de calculer la résistance par la méthode série ou parralèle:
![[Pasted image 20240118155839.jpg]]
$$R_{AC} = R_{A'C'}$$
<=> 
$$$R_{\alpha}+R_{\gamma}=\frac{R_{c}.(R_{a}+R_{b})}{R_{a}+R_{b}+R_{c}}$$

### 7. Mesures des grandeurs de tension, courant et résistances
##### 7.1 Diviseur de tension
Avec deux résistances en série:
Trouver une tension de sortie en connaissant la tension d'entrée:
$V_{s}=U_{2}=U_{e}. \frac{R_{2}}{R_{1}+R_{2}}$
Avec le même raisonnement, on peut trouver la tension d'entrée en connaissant la tension de sortie:
$U_{1}=U_{e}. \frac{R_{1}}{R_{1}+R_{2}}$

##### 7.2 Diviseur de courant
Avec deux résistances en parallèle:
On sait que la tension: $U_{1}=U_{2}=U$
On sait que la résistance: $R_{éq}=\frac{R_{1}.R_{2}}{R_{1}+R_{2}}$
$I_{1}=\frac{R_{2}}{R_{1}+R_{2}}.I_{e}$

##### 7.3 Mesure 
Tension continue: Le voltmètre se place TOUJOURS en parallèle
Courant continu: L'ampèremètre se place TOUJOUTS en série

