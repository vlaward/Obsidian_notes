Go back : [[Web]]

tags : #web #coding 

Un load balancer est un program qui permet de repartis le point de request sur plusieurs server different, pour ne pas en overwhelm un. Il y a different type d'algorythmes pour le faire :
- **Round Robin:** Envoies les requêtes a chaque serveurs un pars un. (serv 1, puis 2, puis 3 puis re 1, 2....)
- **Least Connections:** Envoies les requêtes au server ayant le moins de connection en cours 
- **IP Hash:** Redirige la requête en fonction de l’adresse IP d'ou elle viens (pour une connection avec le plus petit liens, si les different serveurs ne sont pas au meme endroit)