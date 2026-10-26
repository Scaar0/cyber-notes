# Cryptography Basics

Plateforme : TryHackMe
Parcours ou catégorie : Cryptography
Date : 26/10/2026
Difficulté : facile
Durée : [environ X min]

## Objectif
Apprendre les bases de la cryptographie et du chiffrement symétrique.

## Notions clés
- Le but de la cryptographie est d'assurer une communication sécurisée en présence d'adversaires.
- Plaintext : c'est la donnée que l'on veut chiffrer.
- Ciphertext : c'est la donnée chiffrée avec un algorithme de chiffrement (cipher).
- Chiffrement symétrique : les deux parties ont la même clé pour chiffrer et déchiffrer le message.
- Chiffrement asymétrique : chaque personne a une paire de clés, une clé publique et une clé privée. Celui qui envoie le message le chiffre avec la clé publique du destinataire, et le destinataire le déchiffre avec sa clé privée. Les deux clés sont différentes et liées par des mathématiques complexes.

## Lien avec la cybersécurité
La cryptographie est un pilier de la sécurité informatique : c'est ce que les attaquants cherchent toujours à casser et ce que les défenseurs cherchent à renforcer.

## À retenir
La sécurité d’un chiffrement moderne repose sur le secret de la clé, pas sur celui de l’algorithme, qui est public.

## Pour aller plus loin
Déchiffrer par force brute une clé ou un message est aujourd'hui irréalisable en pratique avec un algorithme moderne et une clé assez longue. Comment les attaquants cherchent-ils à contourner le problème ?