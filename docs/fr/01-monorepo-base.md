# Le monorepo du nœud Base

Le dépôt réunit aujourd'hui les composants publics nécessaires au nœud Base : consensus, exécution, builder et outillage.
Le consensus dérive la chaîne L2 depuis les données L1 et les informations du séquenceur.
L'exécution applique ces blocs avec les règles EVM et les extensions propres à Base.
Le builder construit les payloads tandis que les services RPC exposent différents niveaux de finalité.
Cette séparation clarifie les responsabilités mais impose de synchroniser les versions entre composants.
Le Cargo workspace est la carte la plus directe des frontières internes du système.

Suite : [02 — Dérivation](02-derivation-et-finalite.md).
