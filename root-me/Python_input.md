# Python - input()

Plateforme : Root-Me (catégorie App - Script)
Date : 31/10/2026
Difficulté : facile
Durée : 30 min

## Objectif
Exploiter une vulnérabilité dans un script Python déjà présent sur la machine.

## Ce que j'ai compris
- En Python 2, `input()` n'est pas sécurisé et est sujet aux injections.
- Le script Python s'exécute sûrement avec les droits de la personne qui l'appelle. Si on l'appelle via un binaire SUID, il prend les droits du propriétaire de ce binaire et non ceux de l'exécutant.

## Commandes et outils utilisés
- Une injection en Python, par exemple avec : `__import__("xx").xxx` dans `input()`.

## Ce qui m'a bloqué
J'ai mis du temps à comprendre que `input()` exécutait `eval()` automatiquement. Je ne comprenais donc pas que je pouvais écrire mon injection directement dedans, alors qu'il n'y a pas de `print()` ni de fonction du même genre dans le code.

## À retenir
Beaucoup de méthodes étaient disponibles pour cet exercice. Par exemple, la méthode du `PATH` avec un binaire C SUID existe de façon similaire en Python avec `PYTHONPATH`.