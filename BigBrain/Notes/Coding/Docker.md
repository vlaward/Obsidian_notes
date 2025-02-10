Go back : [[Web]]

tags : #coding #dockers #web 

liens utils :  [[DockerUtils | Docker Utils]] [Docker Doc](https://docs.docker.com/)

Docker est un programme qui permet de lancer des daemon, des taches dans un environement independant, comme une sorte de [[Machine Virtuelle|machine virtuelle]] beaucoup plus legere, avec seulement lancer les besoins de la tache en question.

Docker est souvent utiliser pour lancer de peittes taches, souvent ecouter sur un socket. Cela peu servire notemment a pourvoir lancer plusieurs sites sur le meme serveur. Ou quand un site utilise plusieurs services differents en meme temps a pouvoir les lancer et les liers entre eux facilement.

Pour creer un Conteneur, une instance qui execute des commandes, if nous faut un *Dockerfile* qui definis une image de l'instance a executer pars les differentes commandes a executer au lancement de cette dite image. Il faut d'abord creer l'image a partir du *Dockerfile* puis lancer, ce qui en fait un contenair. Une fois cela fait, le program docker peut gerer les images et contenairs, les lister, les arreter, les relancer etc...

Le dockerfile est un format de fichier decrivant comment creer une image de service a lancer par le program docker. Une fois cette image monter on peu la lancer en *contenair* qui tourne en tant que [[Deamon]].

Un *contenair* docker, demande un environement dans le quel se lancer. Cela peu etre pars exemple Python, ou bien un System d'exploitation comme, debian ou apline.

dockefile ex :

<code>FROM debian:latest<BR>
<BR>
RUN echo hello world<BR>
</code>
