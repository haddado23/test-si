# Sécurisation et modernisation d'un environnement système critique

## Contexte

L'environnement concerné supporte environ 600 utilisateurs avec un Active Directory, des serveurs Windows et Linux, des bases de données ainsi que plusieurs applications métiers.

L'audit montre plusieurs points qui nécessitent une action assez rapide : des anciens comptes sont encore actifs, certains utilisateurs ou administrateurs ont plus de droits que nécessaire, les mises à jour ne sont pas régulières et surtout les sauvegardes n'ont pas été réellement testées en restauration depuis plus d'un an.

L'objectif de ce travail est donc de proposer une remise sous contrôle progressive de l'environnement, sans créer une grosse interruption des services.

## Mon approche

Je préfère éviter de commencer directement par de gros changements en production. La première étape est de savoir exactement ce qu'on a, ce qui est critique et où sont les risques les plus importants.

Je propose donc 3 grandes étapes :

1. **J0 à J30 : reprendre le contrôle de l'existant**
2. **J31 à J60 : sécuriser et standardiser**
3. **J61 à J90 : industrialiser et améliorer la supervision**

Un principe important durant toute la période est de ne pas faire de changement critique sans test et sans possibilité de retour arrière.

## Priorités identifiées

Les premières priorités sont :

- désactiver les comptes qui ne doivent plus avoir accès au SI ;
- revoir les droits administrateurs et les privilèges ;
- vérifier immédiatement si les sauvegardes sont réellement restaurables ;
- remettre en place un patch management régulier ;
- centraliser progressivement les logs ;
- améliorer la supervision pour ne plus attendre qu'un utilisateur signale une panne ;
- documenter les procédures importantes.

## Organisation du dépôt

- `docs/` : analyse et propositions techniques
- `governance/` : risques, responsabilités et indicateurs
- `procedures/` : quelques procédures d'exploitation

## Résultat attendu à 90 jours

A la fin des 90 jours, l'objectif n'est pas forcément d'avoir tout remplacé ou tout modernisé. L'objectif est surtout d'avoir un environnement mieux connu, avec les risques critiques réduits, des sauvegardes testées, des accès mieux maitrisés et une exploitation beaucoup plus proactive.
