# Analyse de la situation et des risques

Avant de modifier l'environnement je commencerais par un inventaire. Avec 600 comptes et plusieurs serveurs, il faut éviter de supprimer ou bloquer quelque chose qui est encore utilisé par une application.

## Risques prioritaires

| Risque | Impact possible | Priorité |
|---|---|---|
| Comptes d'anciens collaborateurs encore actifs | accès non autorisé au SI | Critique |
| Trop de privilèges sur certains comptes | compromission plus importante en cas de vol d'un compte | Critique |
| Sauvegardes non testées | impossibilité de restaurer après une panne ou ransomware | Critique |
| Patchs irréguliers | exploitation de vulnérabilités connues | Critique |
| Supervision réactive | détection tardive des incidents | Elevée |
| Peu de documentation | dépendance envers certaines personnes et erreurs d'exploitation | Elevée |
| Logs dispersés | investigation difficile après incident | Elevée |

## Première analyse

Le sujet qui me parait le plus urgent est la combinaison entre les privilèges excessifs et les sauvegardes qui n'ont pas été testés. En cas de compromission importante, on pourrait à la fois perdre des systèmes et découvrir trop tard que la restauration ne marche pas.

Je ne supprimerais pas directement les comptes des anciens employés. Il faut les identifier avec les RH et les responsables, vérifier qu'ils ne servent pas pour un service ou une tâche planifiée, puis les désactiver. La suppression peut venir après une période définie.

Il faut aussi faire une cartographie des serveurs et applications critiques pour savoir dans quel ordre intervenir.
