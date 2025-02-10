Go back : [[DataBase]]

Usefull link : [MariaDB site](https://mariadb.org/fr/) [[MariaDB_utils]]

tags : #coding #data 

MariaDB est une un system de gestion de donne (en gros un serveur Data Base) open source, dans le meme concept et fait pars le meme créateur que [[MySQL]]. Sur le meme model, il y a donc un au niveau de compatibilité avec [[MySQL]], et plus généralement, bien que plus complexe, envers tout les derive SQLs.

MariaDB utilise comme moteur de stockage : 

- [InnoDB](https://mysql.developpez.com/tutoriels/manuel-de-reference-mysql-5-0/?page=Le-moteur-de-tables-InnoDB#L15) : Plus general
- [Aria](https://mariadb.com/kb/en/aria-storage-engine/) : Copie plus facile de tables
- [MyISAM](https://mariadb.com/kb/en/myisam-overview/) : L’ancêtre de Aria. Utilise principalement pars soucis de compatibilite
-  [MyRock](https://mariadb.com/kb/en/about-myrocks-for-mariadb/) : Archivage/compression
- [CONNECT](https://mariadb.com/kb/en/introduction-to-the-connect-engine/) : Connexion a d'autres types de donnes
- [Mroonga](https://mariadb.com/kb/en/about-mroonga/) : optimisation de recherche
