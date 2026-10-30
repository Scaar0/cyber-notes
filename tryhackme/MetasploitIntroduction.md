# Metasploit: Introduction 

Plateforme : TryHackMe
Parcours ou catégorie : Exploitation basics
Date : 30/10/2026
Difficulté : facile
Durée : 30 min

## Objectif
Introduction au framework Metasploit.

## Notions clés
- Définition : Exploit : un bout de code qui utilise une vulnérabilité présente sur le système. Vulnérabilité : un design, du code ou une erreur logique qui affecte le système cible. On exploite la vulnérabilité pour exécuter du code sur la cible. Payload : c'est le code que transporte notre exploit, il tourne sur le système cible.
- Auxiliary : les modules de support, comme les scanners, crawlers et fuzzers.
- Encoders : permettent d'encoder l'exploit et le payload pour éviter que l'antivirus ne les repère en les comparant à d'autres fichiers dans la base de données.
- Evasion : permet de tenter d'échapper à l'antivirus.
- NOPs : opérations qui ne font absolument rien, utilisées comme buffer pour avoir une taille constante de payload.

## Outils et commandes utilisés
| Outil ou commande | À quoi ça sert |
|---|---|
| `msfconsole` | Sert à lancer la console Metasploit |
| `search` | Permet dans la console Metasploit de chercher n'importe quel module en fonction de plusieurs paramètres. Par exemple des modules sur Apache : `search apache` |
| `show options` | Liste les paramètres requis pour ce module |
| `set VARIABLE VALEUR` | Commande pour définir la valeur d'un paramètre d'un module |
| `setg VARIABLE VALEUR` | Sert à paramétrer une variable mais de façon globale pour ne pas perdre la valeur en changeant de module |

## Lien avec la cybersécurité
Metasploit est un framework très utilisé. Il faut savoir l'utiliser pour du pentest et aussi comprendre comment un attaquant essaie d'exploiter notre machine.

## Ce qui m'a bloqué ou surpris
J'ai été surpris que ce soit à ce point automatisé.

## À retenir
Metasploit est un framework extrêmement puissant qu'il faut apprendre à connaître.

## Pour aller plus loin
À quel point Metasploit est-il encore utilisé aujourd'hui pour des attaques ?