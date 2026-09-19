# Sauvegarde et restauration

Pour moi c'est un des points les plus urgents du cas. Une sauvegarde qui n'a jamais été restaurée ne donne pas assez de garantie.

## Actions immédiates

La première semaine, je vérifierais :

- les jobs de sauvegarde ;
- les erreurs récentes ;
- les volumes réellement sauvegardés ;
- la rétention ;
- l'emplacement des copies ;
- les accès aux serveurs de backup.

Ensuite je ferais un test de restauration sur un périmètre maitrisé.

## Cible

Je propose de se rapprocher d'une stratégie 3-2-1-1-0 :

- 3 copies des données ;
- 2 types de supports ;
- 1 copie hors site ;
- 1 copie offline ou immuable ;
- 0 erreur constatée pendant les tests.

Les RPO et RTO doivent être définis avec les métiers. On ne peut pas décider uniquement coté IT qu'une application peut rester indisponible 24h par exemple.

Les tests de restauration doivent ensuite devenir périodiques et documentés.
