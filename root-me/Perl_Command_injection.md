# Perl - Command injection

Plateforme : Root-Me (catégorie App - Script)
Date : 31/10/2026
Difficulté : facile
Durée : 15 min

## Objectif
Exploiter une vulnérabilité dans un script Perl déjà présent sur la machine.

## Ce que j'ai compris
- En Perl, la fonction `open()` est dangereuse car elle est vulnérable à des injections.
- Le script Perl s'exécute sûrement avec les droits de la personne qui l'appelle. Si on l'appelle via un binaire SUID, il prend les droits du propriétaire de ce binaire et non ceux de l'exécutant.

## Commandes et outils utilisés
- Injection de commande via l'entrée transmise à `open()`. L'entrée exacte n'est volontairement pas détaillée ici.

## Ce qui m'a bloqué
J'ai mis un peu de temps à trouver la méthode d'injection.

## À retenir
Les injections suivent le même schéma : une entrée utilisateur est interprétée comme du code ou une commande. C'est une famille de failles très puissante, il faut savoir la repérer.