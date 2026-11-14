# Docker - I am groot

Plateforme : Root-Me (catégorie App - Script)
Date : 13/11/2026
Difficulté : facile
Durée : environ 1h

## Objectif
Trouver comment lire un fichier protégé en exploitant un conteneur Docker avec des privilèges root.

## Ce que j'ai compris
- Un périphérique de bloc, c'est un fichier qui représente un périphérique de la machine. Il ne contient rien, c'est un point d'accès. C'est comme une prise murale. 
- Un périphérique de bloc comme `/dev/sda1` représente la première partition du disque dur de la machine de base.
- Quand on est dans un conteneur Docker, on cherche à avoir accès à la machine d'origine.

## Commandes et outils utilisés
- `ls -al` : regarder les droits des fichiers cachés ou non.
- `find /dev -type b` : chercher les périphériques de type bloc auxquels on a accès.
- `umount [nom disque]` : sert à démonter un disque dur.
- `mount [nom disque] [emplacement souhaité]` : sert à monter un disque dur.
- `cat [nom fichier]` : afficher le contenu d'un fichier.

## Ce qui m'a bloqué
Je n'avais pas de documentation, donc pas d'indication sur par où commencer.

## À retenir
Les conteneurs `--privileged` sont une faille à part entière, il faut tout faire pour éviter de les utiliser.