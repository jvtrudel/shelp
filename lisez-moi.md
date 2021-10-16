# SHelp

Framework léger pour la gestions de scripts shell.


## Usage

```
# Installe SHelp
git clone gitlab.local:datalyse/shelp ~/.local/bin/shelp
echo "export $PATH=$PATH:~/.local/bin/shelp" >> ~/.bashrc


# Installe les scripts externes
shelp install gitlab.local:datalyse/shelp-tests

# Utilise les scripts
shx shelp-tests list

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

## Scripts utilisables par SHelp

### Installation et compatibilité avec SHelp

  - Doivent pouvoir s'installer de la même manière que SHelp lui-même
  - Doivent pouvoir être reconnu par SHelp (implémente toutes les fonctionnalités core du framework)
