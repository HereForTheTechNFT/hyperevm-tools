# 3 — Fraîcheur et cohérence des instantanés

Une précompile expose l’état HyperCore connu au moment où le bloc HyperEVM est construit.
Deux lectures dans le même appel sont cohérentes avec cet instantané, mais pas avec une action CoreWriter émise ensuite.
Le numéro de bloc L1Read fournit un repère de fraîcheur à conserver avec les valeurs dérivées.
Un protocole de crédit doit refuser ou borner une décision fondée sur un prix trop ancien.
Une interface doit annoncer la hauteur observée plutôt que présenter la donnée comme temps réel absolu.
Les caches hors chaîne doivent indexer réseau, bloc, précompile et arguments.
La réconciliation s’effectue sur un bloc postérieur, sans supposer qu’une écriture est immédiatement lisible.

Suite : [encodage CoreWriter](04-encodage-corewriter.md).
