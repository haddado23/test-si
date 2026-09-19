# Plan d'amélioration sur 90 jours

## J0 à J30 - Reprendre le contrôle

Objectif : connaitre l'environnement et réduire les risques les plus urgents.

Actions :

- inventaire des serveurs, applications et comptes ;
- identifier les applications critiques ;
- audit des comptes AD ;
- validation des comptes d'anciens employés avec les RH ;
- désactivation des comptes confirmés inutiles ;
- revue des groupes privilégiés ;
- état des patchs ;
- vérification des sauvegardes ;
- premier test de restauration ;
- collecte des logs les plus importants ;
- commencer la documentation.

A J30 je veux pouvoir dire quels sont les actifs critiques, qui a des droits importants et si on est capable de restaurer les principaux systèmes.

## J31 à J60 - Sécuriser et standardiser

Actions :

- séparation comptes utilisateurs/admin ;
- correction des privilèges excessifs ;
- mise en place d'un groupe pilote pour les patchs ;
- calendrier de maintenance ;
- durcissement Windows/Linux ;
- centralisation des logs ;
- supervision des services critiques ;
- MFA sur les accès sensibles quand possible ;
- procédures d'exploitation principales.

## J61 à J90 - Industrialiser

Actions :

- étendre le patch management ;
- automatiser certaines tâches répétitives ;
- nouveaux tests de restauration ;
- revue des accès ;
- tableau de bord KPI ;
- exercice simple de gestion d'incident ;
- compléter les procédures ;
- bilan avec la direction.

## Gestion du risque pendant les 90 jours

Les changements les plus risqués seront d'abord testés sur un périmètre pilote. Pour chaque changement important il faut avoir une procédure de retour arrière.

L'objectif n'est pas de tout changer en 90 jours mais d'avoir une base saine et une organisation qui permet de continuer l'amélioration après les 90 jours.
