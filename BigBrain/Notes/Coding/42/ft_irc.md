Go back : [[4e_cercle]]

tags : #42school  #42projects #coding

ft_irc est un projet du tronc commun de l'[[ecole 42]] 



notes generales : 
 J';ai besoin de faire les transfere de fichier,m qui se font pars cdes requettes DCC, (Client to client) donc j'ai pas besoin de faire moi meme le transfere, juste renvoyer le bon message, il devrais avoir cette forme la 

PRIVMSG <recipient> :\001DCC SEND <filename> <IP> <port> <size>\001

Where:

- `<recipient>` → The nickname of the client receiving the request.
- `<filename>` → Name of the file being sent.
- `<IP>` → The sender's IP **as a long integer** (converted from standard IPv4).
- `<port>` → The TCP port the sender is listening on.
- `<size>` → The file size in bytes (optional, but useful).


la request ressemble a ca :


PRIVMSG User2 :\001DCC SEND myfile.txt 2130706433 5000 102400\001

🔹 Explication des paramètres :
- `image.png` → Nom du fichier.
- `2130706433` → **IP en format entier** (2130706433 = `127.0.0.1` en IPv4).
- `5000` → Port TCP d'écoute de l'expéditeur.
- `102400` → Taille du fichier en octets.

normal request 


PRIVMSG <recipient> :<message>


- `PRIVMSG` is the command used for sending messages.
- `<recipient>` is either:
    - A **nickname** (for private messages to a user).
    - A **channel** (if sending a message to a chatroom, e.g., `#general`).
- `:<message>` contains the actual text to be sent.


and server answere 

:<sender> PRIVMSG <recipient> :<message>

