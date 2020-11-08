#Rendu TOS
	
	-Arthur HEMONO 2A2

##	1. (1 point) Un appel système : (plusieurs choix possibles)
		
		* Est en général un service proposé par le noyau du système d’exploitation
		
		* write sous Linux est un appel système
		
		*Son appel entraînera la suspension de mon programme pour passe en mode kernel
		
		*Un appel système nécessite une instruction particulière du processeur

##	2. (1 point) Un espace d’adressage sur 32bits peut aller jusqu’à : (un seul choix possible)
		
		*2^32 soit 0x1_0000_0000

##	3. (1 point) La commande man sert à : (plusieurs choix possibles)
		
		* Obtenir diverses documentations notamment celles des appels systèmes
		
		* Lire des exemples de code pour utiliser un syscall
		
		* Connaître des options sur une commande de shell comme ls
		
##	4. (2 points) L’appel système read attends trois paramètres : décrivez les
		* Un descripteur de fichier | type : int
			- une clé abstraite pour accéder à un fichier
		
		* Un buffer | type : void*
			- adresse ou stoqué ce qui est lu
		
		* Un nombre de d'octets | type : syze_t
			- nombre d'octets a lire

##	(2 points) Avec vos mots, tentez de formuler quelles sont les missions principales d’un système d’exploitation. Pour orienter votre réponse : Réfléchissez aux ressources d’un ordinateur. Comment les mettre à disposition ?

		* Gestion du matériel "abstraite"

		* Gestion des processus (chargement/execution) - Ordonance

		* Gestion des entrées/sorties
			-périphérique utilisateurs
			-RAM
			-Stockages 

		* Sécurité

		* Services aux logiciels (userland/syscall)

##	(2 points) La fonction en C printf est elle un appel système ?

		* Non

##	(2 points) Recherche personnelle : Si vous exécutez un programme compilé comme firefox. Que se passe-t-il sans entrer dans les détails dans notre système pour exécuter un proramme ? Quelles sont vos intuitions ?

		* L'appel system exec excute mon binaire, un procesus est lancé sur ma machine (non détaillé)
