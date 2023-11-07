

# RAM

RAM : Random access memory (très chouette album de daft punk)

Stock les données nécessaires au bon fonctionnement du CPU
Les données sont perdues une fois l'alimentation coupée

##### DRAM
![[Pasted image 20231102134713.png]]
Moins cher et plus simple. A une meilleure densité mais a besoin d'une fréquence de rafraichissement.

##### SRAM
![[Pasted image 20231102134726.png]]
Plus cher et plus complexe. Moins dense mais plus rapide (souvent utilisée comme cache (CPU))

#### Caractéristiques de la RAM
- Capacité 
- Type (DDRx)
- Format (DIMM, SO-DIMM)
- Fréquence
- Timing
- Canaux
- Fonctionnalités
- Refroidissement et autre

#### À quoi sert d'ajouter de la RAM ?

Si la capacité de la RAM n'est pas assez élevée, les données seront stockées dans la mémoire morte, rendant l'accès aux données beaucoup plus lent.

|         | RAM       | SSD   | HDD     |
| ------- | --------- | ----- | ------- |
| Débit   | 20Go/S    | 2Go/s | 0.2Go/s |
| Latence | 0.00001ms | 0.1ms | 10ms    |

#### Types de mémoires
- DDR: Double Data Rate (optimisé pour les latences)
- GDDR: Graphics (optimisé pour les débits)
- HBM: Hight Bandwidth Memory (optimisé pour les débits. Mémoire empilée et soudée)

#### Formats
- DIMM (PC)
- SO-DIMM (Laptop)

#### Fréquence de fonctionnement
$$
Fréquence*bus=Débit
$$
$$
2800MHz*64bits=179200Mb/S=22400Mo/S
$$
/!\\ Synchronization entre les fréquences CPU et RAM

#### Les timings

1) Envoi de la commande ACTIVE qui contient le numéro de ligne (Row Access Strobe)
2) Envoi de la commande READ (ou WRITE), qui contient le numéro de colonne (Column Address Strobe)
3) Envoi de la commande PRECHARGE pour fermer la page mémoire sélectionnée
4) La commande PRECHARGE envoie à la mémoire le signal de fermeture de la page
5) Une fois fermée, le cycle peut recommencer

Les timings d'une barrette de RAM sont exprimées en cycles et non en ns
1 tCLK = 1 cycle = 1/Fréquence

#### Multi-channel

Pour exploiter simultanément plusieurs barrettes afin de cumuler les débits

#### UDIMM ET RDIMM
- UDIMM: C'est le CPU qui contrôle la mémoire et qui adresse la RAM
- RDIMM: Il y a une puce qui s'occupe de l'adressage (+ latence)

#### Rank
![[Pasted image 20231102143731.png]]

# CPU

CPU = Central Processing Unit
Il ne sert qu'à faire des calculs et à contrôler les déplacements de données

#### Composition
- Transistors (pour les calculs (portes logiques))
- Mémoire (fournir les données aux transistors)
- Bus de données (entrées et sorties des données)


