# antoinefromafar_bot
 Un bot inline Telegram pour lire les messages avec la voix "AntoineFromAfar" de Acapela 

utilisation: `./antoinefromafar_bot.rb [token de l'API de bots Telegram] [fichier de cookies]`

## Création et mise à jour des cookies
Un fichier de cookies valide dans le format "cookies.txt" contenant des informations de connexion au site acapela-group.com est nécessaire. S'il est invalide, une musique de fond sera présente sur les messages générés.
Pour le générer, et les regénerer avant qu'ils n'expirent, créez une tâche cron lançant le script fourni dans ce dépot avec les variables d'environnement bash suivantes :

* `COOKIES_PATH` (chemin vers votre fichier de cookies)
* `ACAPELA_USER` (votre nom d'utilisateur acapela-group.com)
* `ACAPELA_PASS` (votre mot de passe acapela-group.com)
