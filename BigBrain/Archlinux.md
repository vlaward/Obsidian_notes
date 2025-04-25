

je suis en train de faire l'installation de archlinux : 
Voila les differents elements que je doit gerer et coment je les gere :

J'ai du me conecter a mon reseau local avec iwctl, je doit utiliser le device que je veux, la "station" que je veux, qui utilise un driver. Ma station s'apellais wlan0 et le driver genre... wh1 ou un truc dans le genre
Fallais faire gaffe aq ce que le [[firmware]] soit lancer et que avec "ip link" je vois que le device soit actif
J'ai pu me connecter par ssh dirrectement sur ma machine juste apres, mais j'ai decider de continuer sur le clavier. Du coup j'ai fait gaffe a changert le layout des touches.. a voir si j'ai reussis, tout de suite je suis dans un m enus d'ionstalation j'ai pas trop acces a mnes touches, c'est assez graphique mine de rien :3

bon il m'as demander de partitioner mon disk, j'ai pris la partition lvme de base. Le butde partitioner c'est genre, de separer plusieurs parties de ta memoire pour que ca soit plus securiser. Alors dans l'idee avec les temps je devrais faire encore plus de partitions differente mais pour le moment c'est vraiment pas ma priotrite, en plus jevais faire pleins de modif a ce petit ordis je pense.

Bon j'ai le choix entre 3 boot loader je vais chercher les differences : 
- Grub : ca a l'air d'etre celui de base, il viens de GNU et tout. vraiment de base 
- Efistub : fait pour etre mieux foutus sur les system UEFI (le mien), pouvoir automatiser le chargeur d'amorcage (je pense le truc qui te demande de choisir quel model de ton sytstem tu veux lancer : "ex: Ubuntu2.3.4 | ubuntu2.3.4.secure")
- Limine : Grub en mieux par ce que grub c'est un peu vieux pour le multi boot I guess

je prends efistub :D

J'ai accepter de metre "UKI" pour unified kernel image. En gros ca met le noyeau, le boot firmware UEFI et l'initrd(initial ramdisk) en un seul fichier. C'est plus elegant et rapide qui parait 

alors, il m'as demande si je voulais un profil, j'ai dit oui , un profil desktop avec hyprland. Il me dit qu'il vas installer des trucs auto ducoup. logic j'ai pris un profile. Mais il me demande de quel maniere il est sense acceder a mes hardware, il propose :
- polkit : un truc qui permet de donner des droits a des trucs (une sorte de sudo restrein pour qutre chose qu'un utilisateur)
- seatd : ca a l'air d'etre pareil en plus petit.... Voit pas trop l'interet du coup je prends l'autre

il me demande quel greeter je veux (je crois c'est genbre l'ecran ou tu met ton mdp et tout) :
j'ai pris celui de base, je retournerais peut etre sur **ly**, j'avais aprecier sa gueule.

Je doit prendre une facond e gerer l'audio 
y'as pipewire, qui a l'air d'etre un projet en cours tenus pars des petits gars minionsqui aiment le son
et pulseaudio, qui est celui de base fait par redhat, qui doit etre sacrement utiliser en gros
Je vais prendre le premier et je verrais si j'ai des problemes, ils ont l'air mims

==**je me rends compte que c'est surement ue erreure XD**==




AH !!!! Je doit choisir mon kernel ??? ok 
linux-(seul,hardened,lts,zen) (zen c'es tdes mec qui se la buttent qui parrait donc je prends)


