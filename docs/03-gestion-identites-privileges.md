# Gestion des identités et privilèges

## Comptes utilisateurs

Il faut mettre en place un cycle de vie clair :

Création -> modification -> revue -> désactivation -> suppression.

Les RH doivent informer l'IT lorsqu'une personne arrive, change de fonction ou quitte l'entreprise. Pour les départs, la désactivation doit être faite rapidement.

Une revue des comptes sera faite au début du projet pour trouver :

- comptes inactifs ;
- anciens collaborateurs ;
- comptes sans propriétaire clair ;
- comptes de services utilisés comme des comptes normaux.

## Privilèges

Je propose d'appliquer le principe du moindre privilège. Un utilisateur ou administrateur ne doit avoir que les droits nécessaires à son travail.

Pour les administrateurs, le compte normal et le compte d'administration doivent être séparés. Exemple :

`hbiadja` pour l'utilisation quotidienne  
`adm-hbiadja` pour l'administration.

Les groupes sensibles comme Domain Admins doivent être revus. Il faut éviter de donner des droits directement à une personne si on peut passer par un groupe AD.

Le MFA sera activé sur les accès sensibles quand la solution utilisée le permet.

A moyen terme une solution PAM peut être étudiée, mais je ne pense pas que ce soit la première chose à déployer avant d'avoir déjà nettoyé les comptes et les groupes existants.
