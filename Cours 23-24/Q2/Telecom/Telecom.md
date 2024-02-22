# Découpage réseau

Sous-diviser un réseau permet d'ajouter un niveau hiérarchique: réseau, sous-réseau, hôte

Exemple: 550 employés, 130 commerciaux, 10 directeurs - 192.168.160.0/19
550 employés = 1024 addresses:
192.168.160.0 à 192.168.164.0 
130 commerciaux = 256 addresses:
192.168.164.0 à 192.168.165.0
10 directeurs = 16 addresses:
192.168.165.0 à 192.168.165.16

Exercice 1: Par service puis par étage
Top floor: direction, 8personnes
3e étage: ressources humaines (5) et financers (6)
2e étage: vente (28) marketing (17)
1e: informatique (2), réception (6) employés (505)
réseau: 10.192.224.0 255.255.224.0
Employés: 10.192.224.0 à 10.192.226.0/23
Vente: 10.192.226.0 à 10.192.226.32
Marketing: 10.192.226.32 à 10.192.226.64
Réception: 10.192.226.64 à 10.192.226.72
Finances: 10.192.226.72 à 10.192.226.80
Ressources humaines: 10.192.226.80 à 10.192.226.88
Direction: 10.192.226.88 à 10.192.226.104


Exercice 2:
centre: 
	5 Directeurs   -   195.208.193.11
	5 secrétaires  -  192.208.193.25
ouest: 
	3 compta  -  195.208.193.205
	12 info  -  192.208.193.29
nord: 
	2 RH  -  192.208.193.4
	90 commercial  -  195.208.192.33
	15 marketing  -  192.208.192.210
sud: 
	60 manufacture  -  192.208.192.133


Suite: Ajouter le département Testing (20 personnes) et un espace client (100 personnes) - optimisé