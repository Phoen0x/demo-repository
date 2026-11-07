# Propositions en attente et arbitrages ouverts

Actualisé le 2026-11-07. **Aucune de ces propositions n'est réputée validée.**

## Dernière série de dix propositions

- **1 — Matrice explicite de coexistence :** documenter les interactions entre 4K/HDR/VRR/DSC/USB/KVM/dongles et les combinaisons simultanées. La v2.0 possède déjà des vérifications de simultanéité, mais une matrice systématique reste proposée.
- **2 — EDID/HPD/continuité :** émulation EDID, HPD, gestion des écrans au changement de source, persistance USB et transparence des KVM. Le cahier des charges couvre déjà certains aspects ; renforcement proposé.
- **4 — Scénarios multi-appareils :** procédures d'essai concrètes, mise sous tension/veille, changements d'hôtes et reprise après panne ou déconnexion.

## Propositions plus anciennes qui restent en discussion

- **USB-A recharge uniquement :** l'ancienne version les interdisait même avec deux autres USB-A de données, alors que v2.0 ne les déclare plus explicitement éliminatoires. Choix à effectuer ; **ne pas modifier le texte existant par supposition**.
- **Méthodologie d'exécution en cinq phases :** inventaire ; conformité éliminatoire ; investigations détaillées ; validation des architectures ; classements et verdicts. Non encore validée comme obligation.
- **Distinction taxonomique des dalles :** séparer dalle, rétroéclairage et architecture OLED pour éviter de traiter IPS/VA, Mini-LED et WOLED/QD-OLED comme des catégories de même nature. Remarque 5E de l'audit, non encore acceptée.
- **Autres précisions envisagées dans les recommandations originales :** statuer individuellement sur tout élément n'ayant pas déjà été validé ou inclus dans les amendements v2.1 ; éviter de valider une reformulation par simple recoupement.

## Règles

- L'absence d'arbitrage n'est **ni une acceptation, ni un rejet**.
- Toute décision ultérieure doit préciser le numéro et l'origine de la proposition.
- Éviter les doublons : vérifier d'abord si une nouvelle disposition est déjà entièrement couverte par v2.0 ou v2.1.
- Conserver les désaccords, corrections et raisons de choix dans l'historique des commits/PR.
