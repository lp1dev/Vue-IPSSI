# 2048

   Le but de ce projet est de réaliser un jeu suivant les règles du jeu [2048](https://lp1dev.github.io/2018.js/#/). Il doit pouvoir être joué avec les touches directionnelles du clavier, afficher le score du joueur et à chaque fin de partie envoyer celui-ci ainsi que la durée de la partie sur le leaderboard disponible sur [leaderboard.lp1.eu](https://leaderboard.lp1.eu).

# Ressources

- https://fr.wikipedia.org/wiki/2048_(jeu_vid%C3%A9o)#Syst%C3%A8me_de_jeu
    
## Leaderboard

L'API du leaderboard est accessible sur https://leaderboard.lp1.eu/api.

Deux routes sont mises à votre disposition :

*GET https://leaderboard.lp1.eu/api/json* : Permet de récupérer le leaderboard au format JSON
*GET https://leaderboard.lp1.eu/api/<name>/<score>/<time>* : Permet d'ajouter un score et un temps au leaderboard

## 2048

    Vous pouvez, si vous le souhaitez utiliser le fichier Board.js fourni afin de ne pas perdre de temps sur l'implémentation de la logique du jeu. Il exporte une instance de la classe Board contenant des méthodes implémentant ce dont vous avez besoin pour mettre en place le jeu.

## Board.js

### init(size)

Avant toute chose il est nécéssaire d'initialiser votre plateau de jeu, cela se fait avec la méthode *init(size)*, par exemple, pout initialiser un plateau de 4x4, on utilisera Board.init(4).
Les cases du jeu sont contenues dans le tableau à double entrées squares de la classe.
    
### move(key)

La méthode move permet de calculer un déplacement horizontal ou vertical. Elle prend en paramètre une direction, up, down, left ou right, calcule le déplacement demandé sur Board.squares et ne retourne rien.