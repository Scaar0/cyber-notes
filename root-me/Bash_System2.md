# Bash - System 2

Plateforme : Root-Me
Parcours ou catégorie : App - Script
Date : 30/10/2026
Difficulté : très facile
Durée : 1 heure

## Objectif
Récupérer le flag en exploitant les droits de fichiers et les scripts shell, en réutilisant ce qui a été vu dans Bash - System 1 ou en passant par les liens symboliques.

## Notions clés
- Les liens entre fichiers permettent de lier deux fichiers ensemble. Il existe les liens physiques (`ln` sans argument) et les liens symboliques (`ln -s`). Les liens physiques ne sont possibles que dans le même système de fichiers.
- Variable PATH : c'est la variable qui indique où le système va chercher le code des commandes Linux, par exemple `ls`.

## Outils et commandes utilisés
| Outil ou commande | À quoi ça sert |
|---|---|
| `ln` | Crée un lien entre deux fichiers |
| `export PATH=.:$PATH` | Permet de modifier la variable PATH en y ajoutant le répertoire courant |

## Ce qui m'a bloqué ou surpris
J'ai été bloqué en essayant d'utiliser la méthode du lien entre les fichiers, ce n'était pas la bonne solution. Je suis revenu au changement de PATH classique.

## À retenir
Il ne faut pas rester bloqué sur la même option. Je ne dois pas hésiter à tester plusieurs approches.

## Pour aller plus loin
Y avait-il une véritable solution avec le lien symbolique, comme présenté dans la documentation d'aide ?