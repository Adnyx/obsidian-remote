
# TP
## Commandes

| Commandes                             | Besoins               | Descriptions                                                                  |
| ------------------------------------- | --------------------- | ----------------------------------------------------------------------------- |
| {commande} ?                          |                       | `Donne des informations sur la commande tappée`                               |
| show  ip interface breif              |                       | `Donne une liste des interfaces disponibles`                                                                              |
| show version                          |                       | `Donne la version de cisco`                                                   |
| show clock                            |                       | `Donne l'heure`                                                               |
| show running-config                   |                       | `Montre le fichier de configuration stocké dans la vram`                      |
| show startup-config                   |                       | `Montre le fichier de configuration stocké dans la mémoire morte`             |
| enable                                |                       | `Rentrer dans le premier mode de modification`                                |
| copy running-config startup-config    | enable                | `Sauvegarder la configuration actuelle dans la configuration de démarrage`    |
| configure terminal                    | enable                | `Rentrer dans le mode de configuration`                                       |
| hostname {name}                       | configure terminal    | `Changer le nom de l'appareil`                                                |
| line console 0                        | configure terminal    | `Passer au mode de configuration de la ligne de console 0`                    |
| password {password}                   | line console 0        | `Changer le mot de passe pour la ligne de console 0`                          |
| login                                 | line console 0        | `Confirmer le changement du mdp`                                              |
| enable secret {password}              | configure terminal    | `Changer le mot de passe crypté`                                              |
| service password-encryption           | configure terminal    | `Crypter un mot de passe non-crypté`                                          |
| banner motd "{banner}"                | configure terminal    | `Changer la bannière qui apparait au démarrage`                               |
| interface {interface}                 | configure terminal    | `Passer au mode de configuration de l'interface sélectionnée (souvent vlan1)` |
| ip address {ip address} {subnet mask} | interface {intreface} | `Changer l'addresse IP et le masque de sous-réseau de l'appareil`             |
| no shutdown                           | ?                     | ?                                                                             |


# Théorie
### Définitions
| Mot                            | Définition                                                                                                                                                                                                                                                       |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Réseau                         | Un réseau est un ensemble d'équipements et de logiciels qui permettent d'acheminer de l'information d'un émetteur jusqu'à un ou plusieurs récepteurs                                                                                                             |
| PAN                            | Personnal Area Network                                                                                                                                                                                                                                           |
| LAN                            | Local Area Network                                                                                                                                                                                                                                               |
| MAN                            | Metropolitan Area Network                                                                                                                                                                                                                                        |
| WAN                            | Wide Area Network                                                                                                                                                                                                                                                |
| Unicast                        | Une transmission point-à-point entre un expéditeur et un destinataire est appelée diffusion individuelle                                                                                                                                                         |
| Broadcast                      | Transmission à diffusion générale                                                                                                                                                                                                                                |
| Internet                       | Ensemble mondial de réseaux interconnectés qui coopèrent pour échanger des informations en utilisant des normes cohérentes et communément reconnues                                                                                                              |
| Intranet                       | LAN privé qui appartient à une entreprise (ou une administration) et auquel peuvent accéder uniquement ses membres, ses employésLAN privé qui appartient à une entreprise (ou une administration) et auquel peuvent accéder uniquement ses membres, ses employés |
| Extranet                       | lorsqu’une entreprise fournit un accès sécurisé aux personnes qui travaillent pour d'autres entreprises, mais qui ont besoin des données de l'entreprise en question                                                                                             |
| Segmentation                   | Découper les données à envoyer en parties de taille moins importante dans le but d'entremêler plusieurs conversations différentes (multiplexage)                                                                                                                 |
| BYOD (Bring your own device)   | Dans une entreprise, les employés peuvent apporter leurs propres machines sur le réseau                                                                                                                                                                          |
| Virtualisation                 | Faire fonctionner plusieurs systèmes sur un même serveur physique (voir pg 65/66 aventages et inconvénients)                                                                                                                                                     |
| Cloud computing                | Utiliser des ressources informatiques sous forme de service sur un réseau                                                                                                                                                                                        |
| CPL (courant porteur de ligne) | repose sur la possibilité de connecter un périphérique au réseau grâce à n'importe quelle prise électrique                                                                                                                                                       |
|                                |                                                                                                                                                                                                                                                                  |

### Normes cable ethernet 

###### 568B (plus utilisé): 
orange-blanc
<font style="color:orange">orange</font>
vert-blanc
<font style="color:blue">bleu</font>
bleu-blanc
<font style="color:green">vert</font>
brun-blanc
<font style="color:rgb(168, 88, 53)">brun</font>
###### 568A
vert blanc
<font style="color:green">vert</font>
orange blanc
<font style="color:blue">bleu</font>
bleu blanc
<font style="color:orange">orange</font>
brun blanc
<font style="color:rgb(168, 88, 53)">brun</font>

`Voir pg 6/7 (Attention QCM)`
U/UTP -> pas 
F/UPT -> l'ensemble est protégé par de l'alluminium
F/FTP -> l'ensemble et les paires torçadées sont protégées par de l'alluminium
S/FTP -> Protection maximale (souvent pour les usines car beaucoup de perturbations)
F/UTQ -> plusieurs cables ensembles

| Type  | Protection                                                  |
| ----- | ----------------------------------------------------------- |
| U/UTP | Pas protégé                                                 |
| F/UTP | Couche d'alluminium autour de l'ensemble                    |
| F/FTP | Couche d'alluminium autour de l'ensemble et de chaque cable |
| S/FTP | Protection maximale, souvent utilisé pour les usine         |
| F/UTQ | Foiled/ Unshielded twisted quads                            |

#### Connecteurs fibre optique
- ST
- SC
- LC
- Duplex multimode LC

##### Il y a 4 caractéristiques de base pour répondre aux besoins des utilisateurs
- Tolérence aux pannes
	Pour que le réseau soit en permanence disponible
-  Évolutivité
	Pour que les performances restent correctes même quand plus d'utilisateurs se connectent
-  Qualité de service
	Utilisation de niveaux de priorités, classer les informations selon leur importance
-  Sécurité

## Adressage IP

##### Rappel: Binaire
| ...      | 1024 | 512 | 256 | 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| -------- | ---- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Exemple1 | 0    | 0   | 0   | 0   | 0   | 1   | 0   | 1   | 1   | 0   | 1   |
| Exemple2 |      |     |     |     |     | 1   | 1   | 1   | 1   | 0   | 0    |

Pour traduire du binaire au décimal, il faut additionner les nombres qui correspondent à la colonne dans lesquelles les 1 se trouvent. Voir Exemple1: 101101 vaut 45 car 32+8+4+1 = 45

Pour traduire du décimal au binaire, il faut vérifier quel est le plus grand nombre dans la table qui rentre dans notre nombre à traduire, ajouter un 1 dans la colonne où c'est le cas et répéter. Voir Exemple2:  Pour traduire 60 en binaire, on voir que 32 est le plus grand chiffre de la table qui entre dans 60, on ajoute un 1 dans la colonne du 32 et on le soustrait à 60. 60-32 = 28. 16 entre dans 28 donc on ajoute un 1 et on le soustrait à 28. On obtient 12, 8 entre dans 12 donc on ajoute un 1 et on soustrait. on obtient 4, 4 est le plus grand nombre qui entre dans 4 donc on ajoute un 1 et on le soustrait. On obtient 0, 2 n'entre pas dans 0 donc on met un 0 dans la colonne, 1 n'entre pas dans 0 donc on met un 0 dans la colonne. On peut vérifier notre opération en traduisant du binaire au décimal. 32+16+8+4 = 60, l'opération est correcte.


##### Classes d'IP
| Classes | Masque réseau | Adresse Réseau              |
| ------- | ------------- | --------------------------- |
| A       | 255.0.0.0     | 1.0.0.0   - 126.255.255.255 |
| B       | 255.255.0.0   | 128.0.0.0 - 191.255.255.255 |
| C       | 255.255.255.0 | 192.0.0.0 - 223.255.255.255 |
| D       | 240.0.0.0     | 224.0.0.0 - 239.255.255.255 |
| E       | Non défini    | 240.0.0.0 - 255.255.255.255 |

##### Plage d'IP privées
| Préfixe         | Plage  IP                   |
| --------------- | --------------------------- |
| 10.0.0.0 /8     | 10.0.0.0 - 10.255.255.255   |
| 172.16.0.0 /12  | 172.16.0.0 - 172.31.255.255 |
| 192.168.0.0 /16 | 192.168.0.0 - 192.168.255.255                        |

Le nombre maximum d'hôtes est de 2^n. Où n = au nombre de bit dans le Host ID
Voir exercice papier.

