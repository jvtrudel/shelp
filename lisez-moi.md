# SHelp

Framework léger pour la gestions de scripts shell.


## Usage

```
# Installe SHelp
git clone git@gitlab.local:datalyse/shelp $HOME/.local/share/shelp
ln -s $HOME/.local/share/shelp/bin/shelp  $HOME/.local/bin/shelp

# ou à partir du script d'installation
curl gitlab.local/datalyse/shelp/-/raw/master/scripts/install_shelp | bash

# Désinstalle
$HOME/.local/share/shelp/scripts/uninstall


# Installe les scripts externes
shelp install gitlab.local:datalyse/shelp-tests

# Désinstalle un script externe
shelp uninstall shelp-tests


# affiche a liste des scripts disponibles
shelp list


# Utilise les scripts
shx shelp-tests list


# Consulte le manuel de SHelp
shelp

# Consulte le manuel d'un script
shx shelp-tests help

# Obtient la liste des scripts disponibles
shelp list

```


```
# Met à jour de SHelp
shelp update

# Met à jour un script
shelp update shelp-tests

```



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
