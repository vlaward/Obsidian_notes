
tags : #coding #dockers #web 

liens utils :  [[DockerUtils | Docker Utils]] [Docker Doc](https://docs.docker.com/)

Docker est un programme qui permet de lancer des daemon, des taches dans un environement independant, comme une sorte de [[vm|machine virtuelle]] beaucoup plus legere, avec seulement lancer les besoins de la tache en question.

Docker est souvent utiliser pour lancer de peittes taches, souvent ecouter sur un socket. Cela peu servire notemment a pourvoir lancer plusieurs sites sur le meme serveur, chaques dockers ecoutant sur un socket different.

Pour creer un Conteneur, une instance qui execute des commandes, if nous faut un [[Dockerfile]] qui definis une image de l'instance a executer pars les differentes commandes a executer au lancement de cette dite image. Il faut d'abord creer l'image a partir du [[Dockerfile]] puis lancer, ce qui en fait un contenair. Une fois cela fait, le program docker peut gerer les images et contenairs, les lister, les arreter, les relancer etc...

