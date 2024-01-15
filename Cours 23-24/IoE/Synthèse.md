# Cryptographie

### Cryptographie != Stéganographie
La cryptographie sert à cacher et codes des messages pour les rendre invisibles alors que la stéganographie cache l'existance d'un message. (cacher le contenu du message vs cacher le message)

La cryptographie a toujours été une course entre les cryptologues et les cryptanalystes (ou décrypteurs/hackeurs). Cette course a forcer les deux camps à élaborer des techniques toujours plus complexes.

### Périodes de la cryptographie
Il existe 4 périodes de la cryptographie qui se démarquent.
La cryptographie:
- Manuelle;
	- Coursier, fumée, lumière, bruit,...
- Mécanique (ou électromécanique);
	- Télégraphe de Chappe (utilisation d'un code pour décrypter le message)
- Moderne (ou numérique);
	- Ordinateurs plus ou moins modernes
- Quantique;
	- Ordinateurs quantiques

### La guerre et la cryptographie

Il était primordial pendant la guerre de garder des secrets. Il était tout aussi primordial de déchiffrer les secrets ennemis.
Meilleur exemple: Enigma. Cryptographe allemand réputé incassable mais prouvé cassable par les anglais en 43 ce qui jouera un rôle important dans la victoire des alliés. 

### Hack !

Sur internet, il existe plusieurs couches: 
- le Surface web:
	- Celui qu'on connait tous. Dans celui-ci, tous les sites sont consultables par les moteurs de recherches.
- le Deep web:
	- Les sites du deep web ne sont pas indexés par les moteurs de recherches, donc inacessibles.
- le Dark web (oouuuuh)
	- Sous ensemble de web invisible, chiffré, le web browser TOR permet d'y accéder. 
# AES RSA

# Hashing
### Hashing et Salting de mots de passe

Le chiffrement d'un mot de passe est utilisé lorsqu'on doit récupérer le mdp en texte clair.
Chiffrement: plaintext -> ciphertext. Si déchiffré: ciphertext -> plaintext

Le hachage est similaire au chiffrement mais il ne va que dans un sens.
Hashing: plaintext -> ciphertext
Le serveur stocke une version hachée du mdp, et quand l'utilisateur se login, le serveur calcul son hachage et vérifie si ils correspondent.

Le salage consiste à (comme ajouter du sel dans un plat) ajouter une chaine de caractères au début ou à la fin d'un mdp pour le sécuriser plus.
# Blockchain
La blockchain est une technologie de stockage et de transmition d'informations. Elle est transparente, sécurisée et fonctionne sans organe central de contrôle.
Elle contient l'historique de toutes les transactions effectuées depuis sa création.

Les blockchains publiques ont besoin d'un token programmable. Les transactions sont regroupées en blocs et chaque bloc est vérifié par une technique de "Proof of work" (preuve de fonctionnement, minage). Une fois validé, le bloc est ajouté à la chaine.

Avantages de sécurité, de réduction des coûts, de dématérialisation de processus et une atténuation des risques. 
Par contre, il existe des problèmes juridiques, les transactions sont lentes, 



# Temple OS
Un schizophrène crée un OS car dieu lui a demandé. Il a créé son propre language, le Holy C. Il y a pleins de programmes religieux dessus. Tout l'OS se déroule dans la console, certains programmes sont assez complexes.

# Google Glas

# Failles web + whatsapp

### Failles courrantes
1) Oubli de valider les entrées utilisateurs (injections SQL)
2) Mauvais contrôle d'accès (Liste de mdp visible, pas de mdp par défaut)
3) Vol de session
4) Injection de code dans un site
5) Dépassement de mémoire tampon
6) Injection de commandes (!= de l'injection de code)
7) Mauvaise gestion d'erreurs
8) Mauvais chiffrement
9) Faille dans l'administration distante
10) Mauvaise configuration du serveur web

### Piratage Whatsapp
Suite à un leak de base de donnée, une vague de spam et de phishing est survenue sur whatsapp 

# Présentations élèves