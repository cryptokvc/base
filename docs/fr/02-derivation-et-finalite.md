# Dérivation et finalité

Le pipeline de dérivation reconstruit les entrées L2 à partir de données publiées sur Ethereum.
Il doit suivre l'origine L1, gérer les réorganisations et ne jamais avancer au-delà des données disponibles.
Les états unsafe, safe et finalized expriment des garanties différentes que les clients RPC ne doivent pas confondre.
La SafeDB conserve les repères nécessaires à une reprise cohérente du consensus.
Une divergence entre source L1, séquenceur et base locale doit conduire à une restauration déterministe.
La sécurité du L2 dépend ainsi de la provenance et de l'ordre des données, pas seulement de l'EVM.

Suite : [03 — Exécution](03-execution-et-chainspec.md).
