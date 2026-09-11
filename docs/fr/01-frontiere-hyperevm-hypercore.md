# 1 — Frontière HyperEVM–HyperCore

Le dépôt fournit deux bibliothèques Solidity : L1Read pour observer HyperCore et L1Write pour lui envoyer des actions.
Une lecture est exécutée par staticcall vers une précompile, tandis qu’une écriture cible le contrat système CoreWriter.
Ces deux chemins partagent le consensus mais pas la même sémantique de réussite.
Une transaction EVM réussie prouve l’acceptation locale de l’appel, pas l’exécution métier finale sur HyperCore.
Les valeurs lues correspondent à l’état disponible lors de la construction du bloc EVM.
L’intégration doit donc modéliser séparément demande, observation et finalité.
Cette frontière est le point de départ de toute revue de sécurité du protocole appelant.

Suite : [lectures et erreurs typées](02-lectures-et-erreurs.md).
