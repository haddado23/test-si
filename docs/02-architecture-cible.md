# Architecture cible

Je propose une architecture cible qui reste assez simple. L'objectif n'est pas de rajouter des outils partout, mais de mieux séparer les usages et centraliser ce qui doit l'être.

```text
Utilisateurs
     |
     v
Réseau utilisateurs
     |
 Firewall / ACL
     |
     +--------------------+
     |                    |
     v                    v
Zone serveurs        Zone administration
     |                    |
 AD / Applications     Bastion
 DB / Windows/Linux       |
     |                 Admins
     |
     +-------> Logs centralisés / SIEM
     |
     +-------> Supervision
     |
     +-------> Sauvegarde
```

L'administration des serveurs doit progressivement passer par une zone d'administration dédiée ou un bastion. Il ne faut pas laisser RDP ou SSH accessible inutilement depuis tous les postes utilisateurs.

Active Directory reste la source principale pour les identités internes. Les logs importants doivent être centralisés et la sauvegarde doit avoir au moins une copie séparée de la production et idéalement immuable ou hors ligne.

Cette cible peut être mise en place progressivement, pour éviter un changement brutal de l'architecture existante.
