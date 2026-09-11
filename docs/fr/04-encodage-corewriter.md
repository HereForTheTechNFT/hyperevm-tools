# 4 — Encodage et domaine CoreWriter

Chaque action L1Write possède une variante encode* et une variante send*.
Le payload engage une version, un identifiant d’action et des champs dont la largeur doit correspondre au protocole HyperCore.
Une erreur d’ordre, de signe ou de largeur peut produire des octets valides mais une intention différente.
Les enums comme TimeInForce font partie du domaine métier et doivent être validés avant encodage.
Les identifiants client d’ordre servent à rendre la réconciliation observable, mais ne remplacent pas une règle d’idempotence.
Le contrat appelant doit borner montants, prix et index avant tout cast réducteur.
Il faut journaliser l’intention canonique et son hash avant de considérer l’action comme émise.

Suite : [actions sensibles](05-actions-sensibles.md).
