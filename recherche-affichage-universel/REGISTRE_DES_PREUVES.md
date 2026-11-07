# Spécification initiale du registre des preuves

> Proposition n° 9 **validée** pour une prochaine révision ; ceci constitue une spécification préliminaire, pas une base de mesures déjà constituée.

## Objectif

Relier chaque assertion technique à un équipement exact, une variante, un firmware, une interface, une configuration testée et une source consultable. Aucun score ne doit reposer sur une affirmation non attribuée.

## Identifiants

- `product_id` : référence stable d'un modèle exact ; ne pas confondre variantes régionales.
- `hardware_revision` : révision lorsque connue.
- `firmware_version` : firmware testé, ou « inconnu » explicite.
- `source_device_id` : hôte ou console exact, avec version de système si pertinent.
- `chain_id` : architecture complète et branchement des composants.
- `claim_id` : assertion vérifiable unique (fonction, mode, débit ou mesure).
- `evidence_id` : preuve et conditions du test associées.

## Champs minimaux par assertion

| Champ | Description |
|---|---|
| `claim_id` | Identifiant unique |
| `product_id` | Modèle exact du produit |
| `hardware_revision` / `firmware_version` | Variantes et versions |
| `interface` / `port` | Interface et port exact |
| `source_device_id` / `chain_id` | Contexte de test |
| `feature` | Fonction précise (ex. 4K120 HDR+VRR) |
| `status` | Confirmé, non conforme, conditionnel ou indéterminé |
| `measurement_method` | Méthode / instrumentation / protocole |
| `observed_value` / `unit` | Résultat observé, si mesuré |
| `conditions` | Fréquence, HDR, VRR, câbles, pilote, OS, charge, mode, etc. |
| `source_url` | Source primaire ou secondaire |
| `source_type` | Constructeur, norme, certification, labo, communauté |
| `source_date` / `verified_at` | Date de publication et de vérification |
| `confidence` | Élevé, moyen ou faible |
| `contradictions` | Références opposées et explications éventuelles |
| `remaining_tests` | Essais nécessaires pour conclure |

## Exports envisagés

- Markdown : lecture et revue.
- CSV : inventaire et comparatifs tabulaires.
- JSON : automatisation, recherche de contradictions et réutilisation par outils.
- XLSX : comparatifs analytiques et classement.

## Contraintes d'intégrité

1. Toute assertion garde son identifiant au fil des révisions.
2. Une correction ne supprime pas silencieusement l'ancienne valeur : conserver une trace de provenance.
3. Les données de mesure absentes restent `null` / indéterminées, jamais remplacées par zéro.
4. Les capacités applicables, inapplicables et non testées sont distinguées.
5. Les matrices de compatibilité ne doivent pas assimiler l'absence de mesure à une absence de fonction.
6. Les scores ne sont calculés qu'à partir de sous-critères définis préalablement.
7. Aucun résultat de test physique n'est revendiqué sans essai effectivement réalisé ou source documentée.
