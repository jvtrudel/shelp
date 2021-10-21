
   NAME
      shelp  -  Framework léger pour la gestions de scripts shell

   SYNOPSIS

    Information sur l'état de shelp
      Affiche l'aide
        shelp
        shelp help|man|usage

    Gestion de shelp
      Installe
        curl gitlab.local/datalyse/shelp/-/raw/master/scripts/install_shelp | bash
      Désinstalle
        shelp uninstall|remove|delete
      Met à jour
        shelp update

      Gestion des scripts
        shelp install <git repo>    # installe un script
        shelp uninstall <script id>
        shelp update <script id>

      Édition des scripts
        Génère un projet de script
          shelp new $SCRIPT_ID
        Relie le script à un repo remote
          shelp link $SCRIPT_ID $ORIGIN_URL
        Affiche le répertoire vers le script
          shelp path $SCRIPT_ID
        Affiche le path vers le répertoire du script
          shelp dir $SCRIPT_ID
        Sauvegarde des modifications
          shelp save $SCRIPT_ID [ "$COMMIT_MESSAGE" ]

