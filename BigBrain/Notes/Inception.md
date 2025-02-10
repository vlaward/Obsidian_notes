Go back : [[4e_cercle]]

tags : #42school  #42projects #coding #dockers #web

Inception est un projet du tronc commun de l'[[ecole 42]], il demande de setup 3 [[Docker|dockers]] codependant dans un [[vm|machine virtuelle]] :
-[[NGINX]]
-[[WordPress]]
-[[MariaDB]]

Ici, Wordpress seras dependant de MariaDB car ca seras sa data base. NGINX seras dependant de Wordpress, toutes ces dependances suront definis dans un "Docket-Network".

Le projet doit se lancer avec un Docker-compose, si possible avec un makefile pour simplifier le lancement des nombreuses commandes.