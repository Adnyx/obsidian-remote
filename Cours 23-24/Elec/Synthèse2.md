## Chapitre 1
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
/!\\ Le $\rho$ du cuivre à 0°C est de $1,6.10^{-8}\Omega.m$

##### 3.2. Loi de Mathiessen: 
$R_{T}=R_{0}.(1+\alpha.T)$ où $R_{T}$ est la R à la température voulue, $R_{0}$ est R à 0°C, $\alpha$ est le coefficient de température($°C^{-1}$) et T la température en °C
Cette loi s'applique aussi sur la résistivité des matériaux: $\rho_{T}=\rho_{0}(1+\alpha T)$ où $\alpha = 0,004°C^{-1}$ 
Le coefficient de température du Cu est $\alpha_{Cu}=0,004°C^{-1}$

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


## Chapitre 2 L'électrostatique
### 1. Étude des charges
Un corps est neutre quand $q(t)=0C$, $q(t)$ étant la quantité de charge en Coulomb. $1C =6,25.10^{18}e^-$

Un corps est chargé quand $\sum_{alg} q_{(t)}\neq 0C$
Un corps est chargé négativement lorsqu'il y a un excès d'électrons
Un corps est chargé positivement lorsqu'il y un un manque d'électrons

### 2. Loi de Coulomb
Soit 2 charges ponctuelles: q1 positive et q2 négative, séparés par une distance r.
La force $\vec{F}$ de q1 sur q2 s'exprime par la loi de coulomb:
$|\vec{F}|= \frac{|q_{1}|.|q_{2}|.|\vec{1r}|}{4\pi\varepsilon 0}$ en newton
et $|\vec{F_{q_{1}}}|= -|\vec{F_{q_{2}}}|$

### 3. Le champ électrostatique
$\vec{E}=\frac{\vec{F}}{q}$ , q étant une charge unitaire. $[\frac{N}{C}]$
Si un en 1 point donné, il existe plusieurs champs, il faut les additionner.

### 4. Le potentiel 
La différence de potentiel entre M et P:
$U_{MP}=\int_{M}^{P}\vec{E}.\vec{dl} =U_{P}-U_{M}$

Pour ces cas particuliers, c'est plus simple:
Potentiel dû à une charge ponctuelle: $U_{P}=\frac{q}{4\pi \varepsilon_{0} .r}$

### 5. Le condensateur
##### 5.1 Principe
Des charges A et B équilibrées de part et d'autre d'un isolant. On ajoute un dispositif pour charger positivement A et négativement B. un champ $\vec{E}$ se crée. Si il y a un $\vec{E}$, il y a une $U_{AB}$.
Par définition: $C = \frac{q_{A}}{U_{AB}} = \frac{q_{B}}{U_{AB}}$ 

##### 5.2 Condensateur plan
Deux barres parallèles A et B de charges opposées sont à une distance d.
$C = \varepsilon_{0}\frac{S}{d}$ (vide d'air)
$C = \varepsilon_{0}\varepsilon_{r}\frac{S}{d}$ (autre que le vide d'air)

##### 5.3 plusieurs condensateurs
En parallèle: $C_{eq}=C_{1}+C_{2}+C_{3}$
En série: $C_{eq}=\frac{1}{\frac{1}{C_{1}}+\frac{1}{C_{2}}+\frac{1}{C_{3}}}$

##### 5.4 Énergie électrostatique
$W = \frac{1}{2}CU^2$
