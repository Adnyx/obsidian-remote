
## Programmation orientée objet (POO)
La POO est une façon de penser différente de la programmation procédurale:
En procédural:
```
A=(0,0)
B=(0,1)
distance(A,B)
```
En POO:
```
A=(0,0)
B=(0,1)
B.distance(A)
```
### Propriété et attribut
Propriété: manière de manipuler un attribut (lecture seule, accès non autorisé,...)
Exemple: Attribut=age, sa propriété=accès non-autorisé sauf par la méthode anniversaire
Dans beaucoup de languages, propriété=attribut. Pas en python.

### Avantages de la POO
- Lisibilité
- Facilité de maintenance
- Code source réduit
- Évolutivité

### Inconvénient de la POO
- Apprentissage plus complexe


### La classe
La classe est une abstraction qui définit un objet. Une classe est comme un plan de conception, un genre. ex: Humain.
On peut faire des abstractions plus ou moins précise. (ex. Classe moto et classe voiture ou une seule classe véhicule)
Un objet est une instance de classe, du genre de la classe. ex: Johan, Erwin,...

### Points importants
- Un objet est une entité qui possède un état.
- Une classe est une description d'un ensemble d'objets qui ont les mêmes attributs
- (à finir)
- (à finir)

"Pour pouvoir dégommer le piéton, il faut connaitre la position de la voiture  et du piéton" -Erwin Desmet

Selon Euclide, un point n'a comme caractéristique que sa position

### Modélisation des exigences
- Méthode: fonction d'une classe (sur l'objet)
- Méthode de classe: fonction d'une classe avec une forte appartenance à une classe (sur la classe qui peut être instancié)
- Méthode statique: fonction d'une classe mais indépendante de la classe (sur la classe qui ne peut pas être instancié)

### Encapsulation
(à finir)

L'encapsulation permet de définir des niveaux de visibilité de la classe. Par défaut, les attributs d'une classe sont privés et ses méthodes sont publiques

3 niveaux:
- Public: Les méthodes et attributs avec mot-clé sont accessibles aisément par l'user et la classe
- Protected: Les méthodes et attributs avec ce mot-clé sont accessibles uniquement depuis la classe et ses héritées.
- Private: Les méthodes et attributs avec ce mot-clé sont accessible uniquement depuis la classe.

Pour choisir le bon niveau, par défaut on les protège au maximum, rester sensible à chaque élément, faire attention à l'impact des niveaux d'accès sur le reste de la classe et identifier les éléments qui ont besoin d'accès.

### Interface et contrat
Un contrat d'une classe correspond à son interface et à la définition de ses méthodes. Ex: Toutes les classes "étudiants" doivent implémenter une méthode "étudier", même si elle est différente.
Ex2: on peut comparer la puissance de 2 ordinateurs en RAM mais pas de 2 humains en RAM mais on peut comparer 2 humains sur autre chose. Ils ont tous les deux une méthode "comparer" mais elle compare différemment. 

Il n'y a que des méthodes dans l'interface. Son seul but est d'obliger les méthodes à exister.

Classe Humain implémente soit la classe Étudiant avec la méthode Étudier soit la classe Prof avec la méthode Enseigner.

### Le constructeur
3 types de constructeurs:
- Par défaut (pas de paramètre)
- Par recopie (Le paramètre est une autre instance de classe)
- Paramétrique (on recrée un constructeur) - on va l'utiliser le plus


