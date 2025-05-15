Comment utiliser IRC :


Lancer le serveur :
Make -> ./ircserv <port> <mdp>

Lancer les clients :

Deux facons :
- ./client -> /connect localhost <port> <mdp> (interface graphique)

Exemple :
	/connect localhost 6969 aaa

- nc localhost <port> puis tu ecris ces lignes (tu dois appuyer sur entree entre chaque ligne)
PASS <mdp>
NICK <ton pseudo (sera affiche sur irc)>
USER <ton nom (ne sera pas affiche)>

Exemple :

nc localhost 6969
PASS aaa \
NICK Michel \
USER Michel :Jacky \

Liste des commandes classiques irssi :
/join

Liste des commandes classiques nc :
JOIN #nomDuChannel
PRIVMSG #nomDuChannel :<msg>

Liste des commandes operateur (elles sont dans le sujet aussi)


Si tu passes par le client irssi :
/kick <pseudo>
/invite <pseudo>
/topic <nomDuTopic>
/mode <voir sujet>

Si tu passes par nc :
KICK #nomDuChannel <pseudo> : <raison>
INVITE <pseudo> #nomDuChannel
TOPIC #nomDuChannel : <nouveauTopic>
MODE <voir sujet>
