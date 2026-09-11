# 5 — Actions sensibles et conservation

Le dépôt expose transferts de vault, délégation, staking, spot send, changement de classe USD et autorisation de builder fee.
Les actions sendAsset et reflectEvmSupplyChange touchent directement à la conservation entre domaines.
Pour un token ou NFT fractionné, l’offre EVM reflétée doit rester liée à une source d’autorité unique.
Un transfert cross-DEX doit vérifier actif, DEX source, destination, bénéficiaire et unité avant émission.
Les chemins de dépôt et de retrait doivent être disponibles avant d’accepter un actif récupérable.
Une autorisation de builder fee doit avoir plafond, bénéficiaire et procédure de révocation explicites.
Chaque action asynchrone exige un état échoué et une stratégie de reprise qui n’envoie pas deux fois la valeur.

Suite : [fixture et reproductibilité](06-fixture-et-reproductibilite.md).
