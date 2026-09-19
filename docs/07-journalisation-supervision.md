# Journalisation et supervision

La supervision actuelle est surtout réactive. Le but est que l'équipe puisse connaitre un problème avant que plusieurs utilisateurs commencent à appeler.

## Supervision

Je superviserais en priorité :

- CPU et mémoire ;
- espace disque ;
- disponibilité réseau ;
- services Windows/Linux ;
- bases de données ;
- applications critiques ;
- certificats ;
- sauvegardes.

Les alertes doivent avoir des seuils réalistes. Trop d'alertes peut aussi être un problème car l'équipe finit par ne plus les regarder.

## Logs

Les logs importants doivent être envoyés vers un point central.

Sources prioritaires :

- Active Directory ;
- serveurs Windows ;
- Linux ;
- firewall ;
- applications critiques ;
- bases de données si nécessaire.

Il faut particulièrement suivre les échecs de connexion répétés, création de comptes, ajout dans les groupes privilégiés, changement de GPO et les connexions administratives.

Une solution SIEM peut ensuite permettre de corréler les événements, mais la première étape est déjà de collecter correctement les logs.
