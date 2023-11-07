Typage statique: variable reste du même type (ex: C)
Typage dynamique: type de variable peut changer (ex: python
Typage inplicite: ne pas préciser la variable ( i = 1 )
Typage explicite: préciser le type de variable (int i = 1; )
Déclaration: prévoir la place de la variable en mémoire
Affectation: =
opérateurs logiques:
ET : and / &&
OU : or / ||
NON : not / !
Structures conditionnelles:
	En C:
		if (text expression)
		{
		//code
		}
		else
		{
		//code
		}
		En Python:
		if test expression:
		//code
		else:
		//code
		
3 Types de boucles:
- boucles avec compteur (for loop)
- En C:
int t[5];
for (int i = 0; i < 5; i++)
{
t[i] = i;
}
- boucle conditionnelles (while loop)
do ... while -> peu importe la condition, la boucle sera exécutée au moins une fois
- boucles de parcours (foreach)
		seq = [18, 20, 32]
		for each x in seq
		print x
		end
	En python:
	```py
		fruits = ["apple", "banana", "cherry"]
		for x in fruits:
		print(x)
	```
Spécification d'un prob:
Trouver le chemin le plus court:
	entrée a: adresse
	entrée b: adresse
	pré-condition: a et b sont dans mons
	sortie c: chemin
	post-condition: c relie a et b, et c < c'
- Formalisation:
	- Étapes et/ou Schéma
	- Algorithme

- Algorithme:
	- Def: 
		- Pas d'initiatives par l'exécutant
			- Parfait pour un ordinateur
		- Éviter les ambiguités
		- Utilisation d'un language clair -> Language de prog
	- Les preuves:
		- s'assurer que l'algorithme terminera en un temps fini
		- S'assurer que le résultat fournit par l'algorithme est bien une solution au problème
		- S'assurer que pour une classe de problèmes, l'algorithme donnera bien l'ensemble des solutions correspondantes

- Structures: 
	- Structures de contrôle
		- Séquences
		- Conditionnelles
		- Boucles
	- Structures de données
		- Constantes
		- Variables
		- Tableaux
		- Structures récursives


- Donées
	- Infinité de classe de problème

-  Tableaux
	- Accès par index
		- tab[0]
	- Les données sont contigües
	- Ajout/Suppression impossible

	- Aventages:
		- Attribuer un seul nom à un ensemble de varaibles
		- Connaître le nombre d'éléments et leur type
	- Attention au débordement d'indices (tab[6], index de 0 à 5, pas de 1 à 6 !!)
	- Tableaux à n dimentions: (matrices,...)
	- Tableaux dynamiques

- Listes chaînées: ^147338
	- Ne se suivent pas en mémoire mais pointent vers le prochain élément de la liste
	- Pour ajouter un élément dans la liste: créer en lien entre le le nouveau et le suivant puis entre le précédent et le nouveau
	- Pour supprimer un élément: garder l'élément à supprimer en mémoire temporairement pour pouvoir le supprimer

	- Listes circulaires 
- Listes doublement chainées
	- servent à aller dans les deux sens:
		- <-> a <-> b <-> c  <->[[test.canvas|test]]

- Valeurs tampons: 
	- servent à stocker une valeur qui doit être écrasée et réutilisée

			a = 15 -> a = 5
			b = 5 -> b = 25
			c = 25 -> c = 15
			tmp = a
			a = b
			b = c
			c = tmp

- Piles et Files
	- Piles : (comme une pile d'assiète)
		- Last in, first out (LIFO)

	- Files:
		- First in, first out (FIFO)

---

- Les fonctions: 
	- Paramètres (a, b)
	- Variables locales (c)
		- "return" donc elle doit être stockée dans une variable
	- Fonctions/ Procédures
		- "Fonctions" -> return
		- "Procédure" -> pas de return
	- Appels de fonctions

			def add(a,b):
				c = a + b
				return c
			
- Paramètres obligatoires:
		def add(a , b=5):
			c = a + b
			return c
- Paramètres par défaut
- Paramètres par mot-clé
		def add(a,b):
			c = a + b
			return c
		somme = add(b=2, a=5)
- Paramètres de taille de variable (fais une liste des variables)

---

Les Preuves:

1) Preuve d'arrêt
	- Bien fondé
	- Appel avec paramètres de valeurs inférieurs
2) Preuve de validité 
	- Correction partielle
	- démontrer que si ça fonctionne pour n, ça doit fonctionner pour n-1

Dérécursivation
- Passer d'un algo récursif à  itératif

Aventages de la récursivité:
-  Facile à comprendre
-  Simple à lire

Inconvénients de la récursivité:
-  Utilisation ++ de la mémoire
-  Utilisation ++ du CPU


Sorting algorithm

- Complexité temporelle
	- nbr opérations élémentaires
	- taille des données, notées n
	- la donnée en question:
		- calcul dans le meilleur cas, le pire cas et le cas moyen
- 


 