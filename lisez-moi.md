# SHelp

Framework léger pour la gestions de scripts shell.


## Usage

  - [Utilisation de shelp. Voir le manuel de shelp](./doc/shelp-man.md)
  - [Utilisation de shx. Voir le manuel](./doc/shx-man.md)



# Spécifications

## Utilitaire SHelp

### Framework léger

  - Fournit le minimum.
  - Impose des quelques conventions strictes.
  - Forme un tout cohérent.
  - Est compatible avec les pratiques natives et les standards des langages shell.

### Installation et exécution

  - Peut être récupéré avec git
  - Peut être exécuté dans le projet
  - Pourrait être combiné en un fichier portable
  - Doit expliciter les dépendances
  - Doit être traçable
  - Doit être testable
  - Doit pouvoir être sourcé et utilisé en ligne de commande avec shx

## Scripts utilisables par SHelp

### Installation et compatibilité avec SHelp

  - Doivent pouvoir s'installer de la même manière que SHelp lui-même
  - Doivent pouvoir être reconnu par SHelp (implémente toutes les fonctionnalités core du framework)
  - Doivent avoir un point d'entré unique qui peut être exécuté en tant que commande cli et sourcé
