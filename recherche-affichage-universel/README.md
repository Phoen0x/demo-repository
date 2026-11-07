# Recherche exhaustive des écrans et systèmes d'affichage universels

> **Statut :** dossier documentaire initial, en cours de constitution — 7 novembre 2026.
>
> **Visibilité :** ce dépôt GitHub est **public**. Ne publier ni secrets, identifiants, coordonnées privées, sauvegardes personnelles, ni détails matériels personnels non approuvés.

## Objectif

Concevoir une recherche mondiale, historique et actuelle sur les écrans, téléviseurs, Smart Monitors, stations d'accueil, hubs, KVM, switches et matrices HDMI/DisplayPort, adaptateurs USB/CEC, processeurs vidéo, audio et contrôle, afin de comparer les systèmes les plus polyvalents et réellement compatibles.

Ne pas confondre fonction annoncée, implémentée, mesurée, compatible sous conditions, non documentée et incompatible. Vérifier les fonctions **simultanément exploitables** et les restrictions de toute la chaîne.

## Sources et état du cahier des charges

- [**Index des versions et de leur provenance**](INDEX-VERSIONS.md) : distinction entre « original », v1 (nom d'archivage), v2.0 et v2.1.
- [**Original fourni / prompt prédécesseur**](VERSION-1-PREDECESSEUR.md) : les 20 sections du premier grand texte de comparaison, historiquement avec exigence USB 3.x.
- [**Version 2.0 consolidée**](VERSION-2.0-CONSOLIDEE.md) : les 20 sections du prompt actualisé, avec USB 2.0 minimum et les classements A/B.
- [**Version 2.1 — Amendements A1–A15**](VERSION-2.1-AMENDEMENTS.md) : correctifs approuvés à lire **en plus** de la version 2.0.
- [**Rapport des propositions du 7 novembre**](RAPPORT-PROPOSITIONS-20261107.md) : dernières validations (3/5/6/7/8/9/10) et toutes les propositions en attente.
- [**Rapport des échanges**](JOURNAL-ECHANGES-20261107.md) : déroulement chronologique des décisions.
- [**Décisions**](DECISIONS.md), [**propositions en attente**](PROPOSITIONS_EN_ATTENTE.md) et [**registre des preuves**](REGISTRE_DES_PREUVES.md).

**Précaution historique :** le texte du prédécesseur est bien archivé, mais une version « originale » encore plus ancienne et distincte n'a pas été établie. La comparaison octet par octet avec un export de conversation n'a pas été possible. Les propositions validées après rédaction des amendements v2.1 sont consignées, mais restent à intégrer textuellement dans une révision future.

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
