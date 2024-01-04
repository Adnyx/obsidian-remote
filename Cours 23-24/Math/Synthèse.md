
# Rappel

## Fonctions:

Vocabulaire:
- Domaine de définition: ensemble des entrées acceptées par la fonction sur l'axe $x$, ex: $Dom f(x) = [-7,7]$.
- Ensemble Image: Même chose que le domaine de définition mais sur l'axe $y$.
- Les racines: les zéros d'une fonction.
- Injectif: 
- Surjectif: 
- Bijectif: à la fois injectif et surjectif
- Partout définie: Une droite verticale doit couper le graphe en 1 et 1seul point
- Paire: Symétrie avec l'axe Oy
- Impaire:
### Droites
Équation d'une droite: $y=mx+p$
où $m$ est la pente, $m=\frac{\Delta y}{\Delta x}$
et $p$ est l'ordonnée à l'origine (adaptation de la formule), $p=y_{A}-mx_{A}$

Deux droites sont parallèles si $m_{d_{1}}=m_{d_{2}}$. Elles sont parallèles et confondues si en plus, $p_{d_{1}}=p_{d_{2}}$

### Paraboles
Équation d'une parabole: $f(x)=ax^2+bx+c$ où $a\in \mathbb{R}_{0}$ et où $b$,$c$ $\in \mathbb{R}$
Pour représenter une parabole, il faut représenter 5 caractéristiques:
- Un axe de symétrie
	Une droite verticale d'équation $x=-\frac{b}{2a}$
- Un sommet
	$\left( -\frac{b}{2a},f\left( -\frac{b}{2a} \right) \right)$ ou $\left(  -\frac{b}{2a},-\frac{\Delta}{2a} \right)$ où $\Delta=b^{2}-4ac$
- Concavité:
	- Si $a>0$, la parabole sera convexe, tournée vers le haut. Le sommet sera un minimum.
	- Si $a<0$, la parabole sera concave tournée vers le bas. Le sommet sera un maximum.
- Intersection Oy:
	$x=0$ -> $y=f(0)=c$ -> Intersection en (0,c)
- Intersection Ox (Racines):
	Résoudre l'équation $ax^{2}+bx+c=0$ -> 3 possibilités:
	- Si $\Delta=b^{2}-4ac> 0$ alors:
		- $x_{1,2}=\frac{-b\pm \sqrt{ \Delta }}{2a}$
	- Si $\Delta=0$ alors:
		- $x_{1}=\frac{-b}{2a}$
	- Si $\Delta < 0$ alors pas d'intersection.



## Trigonométrie

Pour mesurer un angle en radian, il faut faire le rapport de la longueur $s$ de l'arc de cercle sur le rayon $R$ du cercle: $\alpha=\frac{s}{R}$
Les nombres trigonométriques d'un angle $\alpha$ sont définis par le $\cos \alpha, \sin \alpha,\tan \alpha,cotg\ \alpha$
![[Pasted image 20240104110744.png]]

# Logarithmes



# Matrices

Une matrice n x m est un tableau de nombres à n lignes et m colonnes

$$
\begin{equation*}
A_{3,3}=  \\

\begin{pmatrix}
1&2&3 \\
2&2&4 \\
4&5&2
\end{pmatrix}
\end{equation*}
$$
Si $m=1$, la matrice est appelée vecteur.
Si $n=m$, la matrice est une matrice carrée.
Une matrice est symétrique si $A_{ji}=A_{ij}$.
Elle est antisymétrique si les valeurs de part et d'autres de sa diagonale sont opposées.

#### Addition et soustraction
Pour additionner les matrices, celles ci doivent avoir la même dimension:

$$
\begin{pmatrix}
1&2&3 \\
2&4&5 \\
4&1&4 \\ 
\end{pmatrix}
+
\begin{pmatrix}
2&2&1 \\
4&5&4 \\
2&1&1
\end{pmatrix}
=
\begin{pmatrix}
3&4&4 \\
6&9&9 \\
6&2&5
\end{pmatrix}

$$
Idem pour la soustraction.

#### Multiplication
##### Multiplication par un nombre
Pour multiplier une matrice par un nombre, chaque terme de la matrice est multiplié par le nombre:
$$
2*
\begin{pmatrix}
1&5 \\
2&3 \\
4&0
\end{pmatrix}
=
\begin{pmatrix}
2&10 \\
4&6 \\
8&0
\end{pmatrix}
$$
##### Multiplication d'une matrice par une autre

Pour multiplier deux matrices, le nombre de colonnes de la matrice A doit être égal au nombre de lignes de la matrice B pour que le produit AB soit possible.
Le produit de la matrice AB est obtenu en multipliant chaque ligne de A avec chaque colonne de B

https://fr.khanacademy.org/math/terminale-option-math-expertes/x8ee233d324ccfb2e:matrices/x8ee233d324ccfb2e:operations-sur-les-matrices/v/multiplying-a-matrix-by-a-matrix
#### Transposition
On peut transposer une matrice en échangeant les lignes et le colonnes:
$$
\begin{align}
A=
\begin{pmatrix}
7&2 \\
3&4 \\
1&1
\end{pmatrix}\\
A^{T}=
\begin{pmatrix}
7&3&1 \\
2&4&1
\end{pmatrix}

\end{align}
$$



