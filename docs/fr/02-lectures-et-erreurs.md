# 2 — Lectures, index et erreurs typées

L1Read encode directement les arguments attendus par chaque précompile : il ne s’agit pas d’un appel ABI de contrat ordinaire.
Les fonctions couvrent positions, soldes spot, prix, délégations, offre, marge et états borrow/lend.
Les index perpétuels récents utilisent 32 bits ; réduire silencieusement vers 16 bits peut sélectionner un autre actif.
Les variantes strictes revertent avec une erreur typée lorsque la précompile échoue.
Les variantes try* permettent au protocole appelant de distinguer indisponibilité et valeur métier nulle.
Une donnée absente ne doit jamais être convertie en prix zéro, solde zéro ou autorisation implicite.
Les bornes d’index et la longueur du retour restent des invariants à contrôler.

Suite : [fraîcheur et cohérence](03-fraicheur-et-coherence.md).
