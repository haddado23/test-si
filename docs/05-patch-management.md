# Patch management

Actuellement les mises à jour sont irrégulières. Il faut donc avoir un processus prévisible.

Je propose le chemin suivant :

```text
Correctif disponible
       |
       v
Environnement de test
       |
       v
Petit groupe pilote
       |
       v
Production
```

Pour les vulnérabilités critiques, un processus plus rapide doit exister.

Avant le déploiement sur un serveur important il faut vérifier l'impact, avoir une sauvegarde correcte si nécessaire et surtout savoir comment revenir en arrière si le patch pose un problème.

Un objectif à 90 jours serait d'avoir au moins 95% des correctifs critiques appliqués dans le délai fixé par l'entreprise. Ce délai devra être défini selon la criticité des serveurs.

Il faut également prévoir une fenêtre de maintenance régulière pour éviter que les mises à jour soient toujours repoussées.
