
## Tas
Arbre binaire parfait
Priorité du tas: clé d'un nœud parent a une plus haute priorité que les clés de ses enfants.
On peut associer un arbre binaire à une liste.

Trier par tas: Trouver l'élément le plus grand, l'échanger avec le dernier élément, l'ignorer. Mettre le nouvel élément le plus grand en haut, recommencer. (2swap, 1remove)
donc: 
- Respecter la priorité Max-Heap
- Swap la racine avec le dernier élément
- Réduira la taille de 1
- Repositionner l'élément le plus grand à la racine

Complexité $O(n \log n)$ -> Tout le temps
Complexité spatiale $O(1)$
Stabilité: non



## Hachage et Salage

#### SHA-256
1: compatibilité des données -> Padding
2: Initialisation des constantes -> h0 à h7 à partir des 32 premiers bits
3: Division en block
4: Traitement des blocks -> traitement individuel, transformation des blocs 

## Pathfinding
### Dijkstra
/!\\

### Floyd-Marshall
1) Déterminer la matrice d'adjacence

|       | A   | B     | C     | D   | E   |
| ----- | --- | ----- | ----- | --- | --- |
| **A** | 0   | 4     | -x- 5 | 5   | x   |
| **B** | x   | 0     | 1     | x   | 6   |
| **C** | 2   | -x- 6 | 0     | 3   | x   |
| **D** | x   | x     | 1     | 0   | 2   |
| **E** | 1   | -x- 5 | x     | 4   | 0   |
Une fois la matrice déterminée, trouver les chemins les plus courts en remplaçant les x par des points intermédiaires 

### Heuristique (A*)
Méthode de calcul qui fournit rapidement une solution réalisable mais pas forcément optimale
Évaluation: 
1) Qualité du résultat
2) Coût de l'heuristique (complexité)
3) Étendue du domaine d'application

### Algorithmes Probabilistes
- Monte-Carlo
	- Temps: déterministe
	- Résultat: probabilité minime d'incorrection
- Las Vegas
	- Temps: aléatoire
	- Résultat: correct
- Atlantic City

# Jeux et algorithmes
## Minimax
- Le joueur est maximisant (on veut maximiser nos gains)
- L'opposant est minimisant (on veut minimiser les gains de l'adversaire)
Créer un arbre pour déterminer les meilleures situations -> lent
### Élagage alpha beta
On ajoute des paramètres ($\alpha$ et $\beta$ )