# Flashblocks et préconfirmations

Flashblocks diffuse des blocs partiels pour rendre l'état pending observable avant la production du bloc complet.
Chaque fragment doit s'inscrire dans le même payload et respecter un ordre monotone.
Une préconfirmation améliore la latence perçue mais ne possède pas la même finalité qu'un bloc dérivé puis finalisé sur L1.
Le client doit savoir remplacer un état partiel si le payload final diffère ou si la connexion est interrompue.
Les RPC pending et le flux WebSocket exposent donc une garantie de fraîcheur, pas une promesse irrévocable.
Les intégrateurs doivent afficher clairement cette distinction aux utilisateurs.

Suite : [05 — Preuves](05-preuves-metering-et-limites.md).
