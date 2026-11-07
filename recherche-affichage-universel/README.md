# Recherche exhaustive des écrans et systèmes d'affichage universels

> **Statut :** prompt de référence **v2.3 intégralement fusionné**, sous revue dans la PR #4 — 7 novembre 2026.
>
> **Visibilité :** ce dépôt GitHub est **public**. Ne publier ni secrets, identifiants, coordonnées privées, sauvegardes personnelles, ni détails matériels personnels non approuvés.

## Objectif

Concevoir une recherche mondiale, historique et actuelle sur les écrans, téléviseurs, Smart Monitors, stations d'accueil, hubs, KVM, switches et matrices HDMI/DisplayPort, adaptateurs USB/CEC, processeurs vidéo, audio et contrôle, afin de comparer les systèmes les plus polyvalents et réellement compatibles.

Ne pas confondre fonction annoncée, implémentée, mesurée, compatible sous conditions, non documentée et incompatible. Vérifier les fonctions **simultanément exploitables** et les restrictions de toute la chaîne.

## Prompt de référence à utiliser

**[VERSION-2.3-FUSIONNEE.md — Cahier des charges intégral et autonome](VERSION-2.3-FUSIONNEE.md)**

Ce fichier contient directement les 20 sections du cahier v2.0, les 15 amendements A1–A15, les 7 propositions déjà validées (3, 5, 6, 7, 8, 9, 10) et la proposition 1, intégrée aux sections 3, 4, 7, 9, 10, 14 et 19. Il n'est plus nécessaire de juxtaposer plusieurs documents pour utiliser le prompt.

Le [rapport de conservation v2.3](RAPPORT-CONSERVATION-V2.3.md) documente les contrôles de cette nouvelle version, et [celui de v2.2](RAPPORT-CONSERVATION-V2.2.md) reste disponible. La revue indépendante et la fusion de la PR restent à faire.

## Sources et état du cahier des charges

- [**Index des versions et de leur provenance**](INDEX-VERSIONS.md) : distinction entre « original », v1 (nom d'archivage), v2.0, v2.1, v2.2 et v2.3.
- [**Original fourni / prompt prédécesseur**](VERSION-1-PREDECESSEUR.md) : les 20 sections du premier grand texte de comparaison, historiquement avec exigence USB 3.x.
- [**Version 2.0 consolidée**](archives/versions/VERSION-2.0-CONSOLIDEE.md) : les 20 sections du prompt actualisé, avec USB 2.0 minimum et les classements A/B.
- [**Version 2.1 — Amendements A1–A15**](archives/versions/VERSION-2.1-AMENDEMENTS.md) : document historique des correctifs approuvés.
- [**Version 2.2 — Ajouts validés**](archives/versions/VERSION-2.2-AJOUTS-VALIDES.md) : source de traçabilité des sept nouvelles propositions intégrées.
- [**Version 2.2 — Fusion autonome historique**](archives/versions/VERSION-2.2-FUSIONNEE.md) : version précédente, archivée à contenu identique.
- [**Version 2.3 — Fusion autonome courante**](VERSION-2.3-FUSIONNEE.md) : version de référence, avec matrice de coexistence systématique.
- [**Rapport de conservation v2.2**](RAPPORT-CONSERVATION-V2.2.md) et [**v2.3**](RAPPORT-CONSERVATION-V2.3.md) : contrôles de conservation successifs.
- [**Rapport des propositions du 7 novembre**](RAPPORT-PROPOSITIONS-20261107.md) : synthèse historique des validations (3/5/6/7/8/9/10) et propositions de l'époque ; consulter DECISIONS.md pour la validation ultérieure du point 1.
- [**Rapport des échanges**](JOURNAL-ECHANGES-20261107.md) : déroulement chronologique des décisions.
- [**Décisions**](DECISIONS.md), [**propositions en attente**](PROPOSITIONS_EN_ATTENTE.md) et [**registre des preuves**](REGISTRE_DES_PREUVES.md).

**Précaution historique :** le texte du prédécesseur est bien archivé, mais une version « originale » encore plus ancienne et distincte n'a pas été établie. La comparaison octet par octet avec un export de conversation n'a pas été possible. Les propositions validées après rédaction des amendements v2.1 ont été intégrées directement dans la v2.2, puis la proposition 1 dans la v2.3 ; les propositions 2 et 4 restent non arbitrées.

## Invariants validés

- Pas de budget, taille, technologie de dalle ni génération éliminatoires par principe.
- Deux classements indépendants : **A** appareil natif tout-en-un ; **B** architecture modulaire complète.
- Au moins **deux ports USB-A de données USB 2.0 minimum** (dans l'écran pour A, dans le système pour B).
- Tous les ports USB de **données** accessibles à l'utilisateur sur les équipements retenus doivent être matériellement capables d'au moins USB 2.0 ; ports limités à USB 1.x non conformes.
- Ne pas imposer USB 3.x pour le HID 8K ; valider les fréquences, le jitter et la stabilité effectivement obtenus.
- Six pondérations générales **inchangées** : compatibilité appareils 25 %, image/gaming 20 %, connectique/USB 20 %, CEC/KVM 20 %, audio/personnalisation/ergonomie 10 %, prix/fiabilité/évolutivité 5 %.
- Quatre statuts fonctionnels : conforme confirmé ; non conforme confirmé ; conformité conditionnelle ; conformité indéterminée.
- **20 verdicts** principaux et spécialisés tels que définis dans la v2.0.
- Le cas PS4 Slim doit privilégier les solutions non destructrices, sans présumer d'un contrôle par touche PS grâce au seul HDMI-CEC.
- Les informations et mesures non vérifiées ne doivent pas être inventées.

## Méthode de travail documentaire

1. Conserver toutes les versions historiques ; les nouvelles révisions sont additives ou explicitement documentées par diff.
2. Inscrire les décisions prises, leur statut, leur date et leurs conséquences.
3. Conserver aussi les propositions rejetées ou non encore arbitrées sans les déclarer adoptées.
4. Pour chaque produit, documenter modèle/révision/firmware, source, date, conditions de test et niveau de confiance.
5. Favoriser les ajouts en branche puis pull request pour revue ; ne jamais réécrire silencieusement les versions historiques.
6. Lorsqu'une fonction est inconnue, poursuivre les vérifications puis inscrire « Indéterminé — informations insuffisantes ».

## Périmètre initial de ce commit

Ce premier commit avait initialisé les décisions et le registre. Des commits documentaires ultérieurs ont ajouté les prompts historiques disponibles, les amendements et les rapports. Le catalogue de produits et les mesures techniques restent à constituer.
