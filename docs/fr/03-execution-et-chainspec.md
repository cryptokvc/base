# Exécution, chain spec et mises à niveau

La chain spec fixe l'identité du réseau, les activations de forks et les paramètres compris par le moteur d'exécution.
Le payload builder assemble transactions, retraits et attributs dérivés avant l'exécution.
Les règles EVM de Base doivent s'activer au même bloc que les règles de consensus correspondantes.
Une mauvaise configuration peut produire une chaîne localement valide mais incompatible avec le réseau.
Les mises à niveau doivent donc engager code, paramètres et calendrier dans un même processus vérifiable.
Les modules execution et consensus offrent deux vues complémentaires de ces invariants.

Suite : [04 — Flashblocks](04-flashblocks-et-preconfirmations.md).
