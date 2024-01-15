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

RSA: A envoi à B -> sécurisation avec clé publique de B -> B décrypte avec sa clé privée

AES: Text + clé secrète -> cipher

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
Par contre, il existe des problèmes juridiques, les transactions sont lentes, mauvais passage à l'échelle par rapport au nombre de transaction, très très mauvais pour l'écosystème.

### Tiers de confiance (modèle centralisé)
C'est quelqu'un (ou quelque chose) qui joue l'intermédiaire dans les échanges. ça facilite les échanges mais c'est un single point of failure, et la dépendance envers le tiers de confiance.

### Modèle décentralisé
Ici, c'est l'inverse. Il n'y a pas de "middle man" en qui on doit avoir confiance puisque tous les utilisateurs se parlent entre eux. Donc pas de single point of failure, pas de dépendance à un tiers par contre, difficulté à évoluer, à accéder aux informations,...

# Temple OS
Un schizophrène crée un OS car dieu lui a demandé. Il a créé son propre language, le Holy C. Il y a pleins de programmes religieux dessus. Tout l'OS se déroule dans la console, certains programmes sont assez complexes.

# Google Glass
Dans la vidéo c'est pas les google glasses qui sont importantes, à la fin il explique qu'il y a 2 types d'apprentissages: le book learning et le expansive learning. Le book learning c'est apprendre ce que l'humanité connait déjà et le expansive learning c'est découvrir des choses.


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

### Intelligences artificielles
Il y a différents types d'IA. Celles qui traitent du texte, celles qui reconnaissent des images, celle qui apprennent automatiquement (Machine Learning), celles qui peuvent générer du contenu (image, texte, musique,...) et des IA de navigations.
Les IA posent des problèmes étiques. 
Il est possible d'attaquer les IAs avec notamment avec des prompt injections.

Le machine learning utilise des algorithmes pour que l'IA puisse tirer des conclusions en apprenant.
Le deep learning est une sous-catégorie du machine learning mais qui utilise des réseaux ne neurones.

### IA et voitures 
Les IA sont déjà dans nos voitures, avec par exemple les assistance à la décision. 