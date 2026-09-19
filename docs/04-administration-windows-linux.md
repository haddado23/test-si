# Administration Windows et Linux

## Windows

Pour les serveurs Windows je m'appuierais principalement sur Active Directory et les GPO afin d'avoir des configurations plus homogènes.

Actions principales :

- séparation des comptes administrateurs ;
- revue des GPO existantes avant d'en créer de nouvelles ;
- utilisation de Windows LAPS pour les mots de passe administrateurs locaux ;
- limitation de RDP ;
- activation des logs nécessaires ;
- durcissement progressif des serveurs.

## Linux

Pour Linux :

- utilisation de SSH par clé pour les administrateurs quand c'est possible ;
- limiter la connexion directe en root ;
- utiliser sudo et garder les traces des actions ;
- retirer les services inutiles ;
- mettre en place une politique de mise à jour ;
- centraliser les logs importants.

Je ne changerais pas tous les serveurs en même temps. Je commencerais par quelques machines pilotes puis extension après validation.
