# Bash - unquoted expression injection

Plateforme : Root-Me (catégorie App - Script)
Date : 07/11/2026
Difficulté : facile
Durée : environ 1h30

## Objectif
Exploiter la faille d'un script qui ne protège pas ses variables avec des guillemets.

## Ce que j'ai compris
- Comment fonctionne `if test` en Bash, les différentes syntaxes avec ou sans `[`, et les différents arguments (`-o`, `-eq`, `==`...).
- Comment écrire un script de brute force en Python.

## Commandes et outils utilisés
- `python3 attack.py` : exécuter un script nommé attack.py en Python 3, pour automatiser les appels à `./wrapper`.
- `man test` : pour connaître les différents paramètres de `test`.
- Recherche internet : « unquoted expression security bash », pour trouver des informations sur la faille liée aux variables sans guillemets.

## Ce qui m'a bloqué
Je n'ai trouvé aucun exemple précis avec des `if`, seulement avec des `echo`. Le seul exemple avec un `if` utilisait du brute force, dans un contexte différent du mien. Après 1h sans rien trouver de mieux, j'ai tenté cette approche, sans succès. Puis j'ai compris qu'avec la bonne méthode, `-eq` n'accepte que des nombres, sous peine d'erreur. J'ai donc fait plusieurs essais inutiles avant d'élucider ce problème.

## À retenir
Toujours vérifier le type de comparaison attendu (`-eq`/`-ne`/... vs `=`/`!=`) avant de choisir les valeurs à injecter. Mon brute force aurait fonctionné si je l'avais configuré avec uniquement des nombres.