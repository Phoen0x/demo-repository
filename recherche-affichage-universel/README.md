# Recherche exhaustive des écrans et systèmes d'affichage universels

> **Statut :** dossier documentaire initial, en cours de constitution — 7 novembre 2026.
>
> **Visibilité :** ce dépôt GitHub est **public**. Ne publier ni secrets, identifiants, coordonnées privées, sauvegardes personnelles, ni détails matériels personnels non approuvés.

## Objectif

Concevoir une recherche mondiale, historique et actuelle sur les écrans, téléviseurs, Smart Monitors, stations d'accueil, hubs, KVM, switches et matrices HDMI/DisplayPort, adaptateurs USB/CEC, processeurs vidéo, audio et contrôle, afin de comparer les systèmes les plus polyvalents et réellement compatibles.

Ne pas confondre fonction annoncée, implémentée, mesurée, compatible sous conditions, non documentée et incompatible. Vérifier les fonctions **simultanément exploitables** et les restrictions de toute la chaîne.

## Sources et état du cahier des charges

- **v2.0** : cahier des charges consolidé original (20 sections), fourni dans la conversation source. **Texte intégral non encore importé dans ce dépôt.**
- **v2.1** : v2.0 + amendements correctifs A1 à A15 déjà rédigés dans la conversation source. **Texte intégral non encore importé dans ce dépôt.**
- **Prochaines révisions** : seules les améliorations expressément validées sont éligibles à intégration ; toute autre proposition demeure en attente.
- Voir [DÉCISIONS.md](DECISIONS.md), [PROPOSITIONS_EN_ATTENTE.md](PROPOSITIONS_EN_ATTENTE.md) et [REGISTRE_DES_PREUVES.md](REGISTRE_DES_PREUVES.md).

**Important :** ce dossier ne constitue pas encore la copie exhaustive et autonome des prompts v2.0 et v2.1. Leur importation littérale et la vérification de leur intégrité restent à faire sans écraser les versions précédentes.

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

Ce premier dépôt contient **les décisions, les propositions en suspens et une spécification documentaire de preuve**. Il ne contient pas encore le catalogue de produits, les données de tests ni les prompts intégraux. Ces absences sont explicites pour éviter toute fausse impression d'exhaustivité.
