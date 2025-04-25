tags : #coding #cpp 

L'evaluation !!! :D
L'evaluation c'est le sens dans le quel ton compilo( I supose) capte tes expressions (lvalue rvalue mon cul).

Par exemple : 
```i = 0;
a = ++i; //a = 1 et i = 1 pars ce qu'il incerementee i avant l'operation
a = i++; // a = 1 et i = 2 pars ce qu'il incermente apres
```

Certains langages ont surement des sens de lecture mais en cpp c'est pas definis dans tout les cas

genre dans le cas :
```
i = i++ + 2;
ou
i = ++i + i++
```
Aled, il incremente apres l'operation le i++ ou avant ?? en soit la ca change pas grand chose vus que c'est un calcule simple mais dans certains cas ca peut etre une sacre  merde T^T.
Donc en gros la il sortirais une erreur "undefined behaviour" ! :D

ps : Alors ca peu etre definis du coup. Et d'ailleuir les cas du dessus depuis C++17 ils sont gere. Mais y'as des cas ou ca peu rester chiant et dans d'autrea langages aussi ^^