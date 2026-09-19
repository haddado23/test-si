# Mesures générales de sécurisation

La sécurisation doit être progressive parce que certaines mesures peuvent casser des applications anciennes.

Je propose notamment :

- segmentation entre utilisateurs, serveurs et administration ;
- moindre privilège ;
- MFA pour les accès sensibles ;
- suppression ou désactivation des protocoles inutiles ;
- durcissement Windows et Linux ;
- EDR/antivirus correctement supervisé ;
- firewall avec règles revues régulièrement ;
- limitation des flux d'administration ;
- gestion des certificats ;
- sauvegardes séparées et protégées ;
- revue régulière des vulnérabilités.

Les règles de firewall existantes ne doivent pas être nettoyées uniquement parce qu'elles semblent anciennes. Il faut d'abord vérifier leur utilisation afin d'éviter une interruption d'une application métier.

Pour les changements sensibles je garderais toujours le principe : test, validation, changement, vérification et possibilité de rollback.
