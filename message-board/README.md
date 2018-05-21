# Message Board

Le but de ce projet est de réaliser une message board semblable à twitter/mastodon.
Une API est mise à votre disposition sur http://whispering-spire-74666.herokuapp.com/.
Elle permet d'ajouter des utilisateurs, se connecter et envoyer/lire des messages.

# whispering-spire-74666.herokuapp.com

Plusieurs routes sont mises à votre disposition :

- GET */messages* : Retourne les derniers messages postés
- POST */users* : Inscrit un utilisateurs sur la plate-forme
- GET */users* : Retourne le profil de l'utilisateur connecté
- POST */messages* : Ajoute un message sur la plate-forme