# 6 — Fixture, bloc épinglé et limites

HyperliquidTestFixture permet de présenter aux précompiles un état obtenu depuis un RPC, via FFI dans un profil séparé.
Épingler un bloc rend un scénario reproductible ; utiliser zéro signifie dépendre du dernier état disponible.
Le réseau, l’URL RPC et la hauteur font partie du cas de test et doivent apparaître dans son manifeste.
Un mock vérifie le comportement de l’appelant face à des retours choisis, pas la fidélité complète de HyperCore.
Un fork réseau apporte du réalisme mais dépend de la disponibilité et de l’historique du fournisseur RPC.
Les deux approches couvrent des risques différents et doivent rester identifiables dans les rapports.
Ce parcours est documentaire : aucune installation, compilation, FFI, transaction ou exécution de tests.
Les affirmations peuvent être confrontées aux fichiers src/, test/ et test-ffi/ du dépôt.
