
tags : #coding #cpp 

La rvlaue c'est une prvalue ou xvalue(une fois utilise comme reference). c'est edes trucs qui sont pas accessible pars ton programme mais qui y servent.

en gros une lvalue c'est une valeur que ton programme peu acceder, genre une variable etc..

les gvalue c'est les lvalue et les Xvalue. En gros, c'est ce qui est accessible, les xvalue sont ens soit "plus" accessible pars ton programe a un moent mais l'on ete a un autre. Enfgin c afait sens je trouve :/

les prvalue c'est des trucs que t'access pas. Tes literaux, les appels fonction qui retourne un type non inference"( en  gros un truc inferent c'est que le compilot peu capter avec le contrexte ce que ca veux dire) 
les objets cree pendant l'[[Evaluation]]  et les trucs seulement acceccible par le compilo

en gros c'est tout ce que ton programme accesse pas.

une xvalue c'est une adresse que ton programme peu plus access mais qui peut servire de ref pour une rvalue

genre : 
```
i = foo(87); // ici le resultat de foo(87) est une xvalue et i c'est une lvalue
i = INT_MAX; // i est toujours lvalue mais "INT_MAX" ton programme a pas d'action dessus. C'est une prvalue, gerer que pars ton compilo.
```

faut penser que lvalue c'est les expression de gauche, rvalue c'est les expression de droite.

