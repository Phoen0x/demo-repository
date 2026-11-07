# Ajouts supplémentaires approuvés — Source de consolidation v2.2

Ce fichier contient **uniquement les sept propositions validées** après rédaction des amendements A1–A15. Le document de référence directement exécutable sera `VERSION-2.2-FUSIONNEE.md`, où ces textes seront intégrés aux sections pertinentes. Ne pas considérer ce fichier isolément comme un nouveau cahier des charges autonome.

## P3 — Section 4 — Protocole normalisé des mesures de latence

Définir des méthodes comparables de mesure de la latence et des caractéristiques temporelles, en distinguant notamment :

- Le délai de traitement vidéo et l'input lag du moniteur.
- Le délai de balayage, selon la position de mesure sur l'écran.
- Le temps de réponse réel des pixels, l'overshoot et la persistance lumineuse.
- La latence d'un périphérique de commande.
- La latence du moteur de jeu et du pipeline CPU/GPU.
- La latence clic-vers-photon ou entrée-vers-photon complète.
- Les performances dans les modes SDR, HDR, VRR, upscaling et strobing.

Pour chaque résultat chiffré, documenter : méthode de déclenchement, instrument, calibration, emplacement du capteur, mode de l'écran, résolution/fréquence, FPS et frametime lorsqu'applicables, firmware, pilote, environnement, répétitions, nombre d'échantillons et méthode de calcul.

Présenter les médianes et percentiles pertinents, ainsi que le jitter ou les distributions lorsque disponibles ; ne pas fabriquer de statistiques absentes des sources. Vérifier les variations à 60, 120, 240 Hz et au-delà lorsque pertinent, ainsi que les conditions à 30/40/60/120 fps.

Comparer uniquement des mesures produites selon des protocoles suffisamment compatibles. Lorsque les essais disponibles sont incomparables, l'indiquer et garder leurs résultats séparés plutôt que produire un ordre arbitraire.

## P5 — Section 13 — Sécurité, confidentialité et isolation entre appareils

Évaluer les surfaces d'attaque et les mécanismes de protection des Smart Monitors, téléviseurs, docks réseau, KVM IP, appareils USB partagés, contrôleurs CEC, applications de gestion et systèmes d'automatisation.

Rechercher les politiques de mises à jour et de correction des vulnérabilités, les permissions, comptes obligatoires, interfaces distantes, API locales, services cloud, télémétrie, publicité, accès au microphone ou à la caméra et possibilités de fonctionnement hors ligne.

Analyser les risques de communication non désirée entre hôtes via hub/KVM, les mécanismes d'isolation des périphériques et les contrôles d'accès ; distinguer les fonctions natives effectivement documentées des protections seulement supposées.

Documenter les compromis entre fonctions intelligentes, ergonomie, interopérabilité, confidentialité, maintien du support et sécurité. Valoriser la réduction réelle de la dépendance au cloud sans transformer cette préférence en nouvelle exigence éliminatoire.

## P6 — Section 5 — Calibration avancée et fidélité de la chaîne colorimétrique

Évaluer les possibilités et les performances de calibration matérielle et logicielle : LUT 1D/3D, profils ICC, gestion des espaces sRGB/DCI-P3/Adobe RGB, point blanc, gamma, précision et dérive colorimétrique, ainsi que le maintien des réglages par entrée, source ou mode.

Pour le HDR, vérifier le suivi de la courbe EOTF/PQ, le tone mapping, les métadonnées réellement prises en charge, HGiG lorsque pertinent, les limites de luminance, le clipping, la fidélité des tons et les compromis introduits par le mode jeu.

Comparer séparément les pipelines Windows, Linux, macOS, consoles et applications de lecture vidéo. Distinguer les profils effectivement appliqués par l'hôte des réglages stockés dans l'écran et des traitements imposés par le téléviseur.

Rechercher des essais instrumentés comparables, en précisant la mire, la méthode, le matériel de mesure, les points d'échantillonnage, les conditions lumineuses, les versions firmware et les réglages. Ne pas déduire une bonne fidélité colorimétrique de la seule couverture d'un gamut.

## P7 — Section 5 — Confort visuel mesuré en usage prolongé

Étudier la netteté et la lisibilité des textes selon Windows, Linux et macOS, y compris les conséquences des sous-pixels RGB, BGR ou atypiques, des moteurs de rendu, du lissage de caractères, de l'anticrénelage, de l'échelle logique et de la densité de pixels.

Examiner les revêtements de dalle, la diffusion des reflets, la granularité, les angles de vision, l'uniformité, la stabilité de la luminance, le PWM et le flicker à différentes valeurs de luminosité, ainsi que les comportements en VRR et à différentes fréquences.

Comparer la netteté en mouvement, la persistance lumineuse et les effets des traitements stroboscopiques. Distinguer les données instrumentées des témoignages subjectifs de confort ou de fatigue oculaire, sans transformer une observation en allégation médicale universelle.

Évaluer les usages prolongés de programmation, bureautique, lecture, création de contenu, films et gaming, sans favoriser arbitrairement un type de dalle.

## P8 — Section 13 — Vieillissement, réparabilité et garanties selon les régions

Rechercher les défaillances connues, défauts récurrents et taux observables de fiabilité, en séparant les problèmes de conception des incidents isolés. Examiner notamment le burn-in OLED, la perte de luminosité, les pixels défectueux, la dégradation du rétroéclairage, les ventilateurs, les alimentations et les ports.

Vérifier les protections de dalle, leur efficacité documentée, les firmwares, la disponibilité des pièces détachées, l'accès à la maintenance et la possibilité de remplacement de composants.

Pour une acquisition en France, distinguer neuf, reconditionné, occasion auprès d'un professionnel, occasion entre particuliers et importation depuis l'Union européenne ou hors UE ; comparer la garantie légale et commerciale applicable, les exclusions, les coûts de transport/retour, la fiscalité d'importation, le SAV et la disponibilité réelle des pièces.

Ne pas extrapoler directement les résultats d'essais accélérés à une durée de vie exacte en usage normal. Ajouter ces facteurs au coût complet, à la fiabilité et à l'évolutivité dans le respect de la pondération existante.

## P9 — Section 1 — Registre des preuves et exports reproductibles

Maintenir un registre structuré, versionné et réutilisable de toutes les affirmations techniques, décisions de conformité, mesures et sources.

Pour chaque produit, variante, révision et configuration, attribuer un identifiant stable. Pour chaque assertion, conserver : identifiant du produit, fonction évaluée, port, appareil source, version matérielle/firmware/logicielle, statut (confirmé/conditionnel/non conforme/indéterminé), preuve exacte, organisme ou auteur, URL ou référence archivée, date de publication, date de vérification, protocole de test et degré de confiance.

Pour les mesures, conserver l'unité, l'instrument, les réglages, les conditions expérimentales, le nombre d'échantillons et les statistiques disponibles. Signaler les sources contradictoires et les changements introduits par des firmwares ultérieurs. Ne pas remplacer une mesure historique par une nouvelle sans conserver sa provenance.

Prévoir des exports en formats ouverts et exploitables par programmes, notamment CSV et JSON, ainsi qu'un export XLSX lorsque pertinent, sans faire de ces formats une obligation de livraison immédiate pour les données encore inexistantes.

Documenter le schéma de données, les règles de validation et les méthodes de génération des tableaux ou classements. Éviter les doublons et permettre une mise à jour incrémentale sans refaire toute la recherche. Ne pas publier de secrets ou de données personnelles non nécessaires.

## P10 — Section 18 — Frontière de Pareto et comparatif d'efficacité réelle

En complément des classements pondérés inchangés, étudier une frontière de Pareto entre configurations techniquement comparables et suffisamment documentées.

Une configuration peut être considérée comme dominée seulement lorsqu'une autre fait au moins aussi bien sur tous les critères retenus et strictement mieux sur au moins un, en tenant compte du sens de chaque métrique, des incertitudes et des exigences éliminatoires.

Ne pas classer comme dominé un équipement faute de données : distinguer les cas indéterminés, les domaines de comparaison incomplets et les mesures non comparables.

Présenter les compromis observables : fonctionnalité maximale, performance, latence, complexité, fiabilité, coût complet, simplicité d'utilisation et potentiel d'évolution. Mettre en évidence plusieurs solutions non dominées lorsqu'il n'existe pas un gagnant démontré sur toutes les dimensions.

Cette analyse complète, mais ne remplace jamais, les **six pondérations générales** ni la séparation des classements A et B. Elle n'ajoute aucune nouvelle exigence éliminatoire.
