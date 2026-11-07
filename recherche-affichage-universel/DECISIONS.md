# Journal des décisions — recherche d'affichage universel

Mise à jour : 2026-11-07. Chaque entrée distingue **VALIDÉ**, **EN ATTENTE**, **DÉJÀ INTÉGRÉ** et **NON DÉCIDÉ**. Les propositions non validées ne deviennent pas automatiquement des exigences.

## Socle déjà adopté : v2.0

La version 2.0 constitue la base de 20 sections, sans limitation arbitraire de générations ou de marchés, avec deux classements A/B, 20 verdicts et les six pondérations générales 25/20/20/20/10/5.

USB : minimum matériel USB 2.0 pour les ports utilisateur de données ; deux USB-A de données obligatoires (A : intégrés à l'écran ; B : disponibles dans l'architecture complète). USB 3.x et supérieur restent des bonus à évaluer sur leurs gains réels.

**Point toujours non arbitré :** le statut éliminatoire des ports **USB-A exclusivement destinés à la recharge**, qui était différent dans une ancienne version du cahier des charges.

## Révision v2.1 — décisions validées et déjà rédigées sous forme d'amendements

### Corrections du point 3 de l'audit comparatif original — VALIDÉES

1. Compatibilité mobiles par modèle, OS/version, connecteur et protocole.
2. Distinction précise des implémentations matérielles G-SYNC.
3. Adaptateurs actifs/passifs, certification/longueur des câbles.
4. Restrictions DisplayPort MST sous macOS.
5. Recharge rapide, puissances réelles et alimentation USB en veille.
6. Exclusion explicite des interfaces USB internes de fabrication/maintenance des exigences utilisateur.
7. KVM : systèmes, pilotes et stabilité des reconnexions.
8. Latence de microphone et audio aller-retour distinctes.
9. Outils de contrôle Windows/Linux/macOS.
10. Profils d'éclairage spécifiques aux jeux, films et entrées.
11. Classe séparée pour les candidats de conformité indéterminée.
12. Sous-critères de notation définis avant l'évaluation ; niveau de confiance des scores.
13. Classement secondaire explicitement non conforme pour les candidats éliminés.

### Remarques techniques 5A–5D de l'audit original — VALIDÉES

- **5A :** interférences USB 3.x/2,4 GHz ; tester dongles, ports, hubs, blindage, éloignement et charge.
- **5B :** Switch Lite : distinguer sortie native, modification matérielle, capture externe et impossibilité d'un simple adaptateur USB-C/HDMI de créer la fonction.
- **5C :** PS4 Slim et CEC : preuves indépendantes pour navigation, écran d'utilisateur, commande PS, association DualShock et dépendance au firmware ; examiner les démonstrations historiques stb-tester.
- **5D :** HDMI 2.2/Ultra96 : vérifier débit certifié et négocié de la chaîne complète, pas seulement l'étiquette de norme.

Ces 17 groupes de corrections sont couverts dans les amendements A1 à A15 rédigés pour v2.1. **Les textes complets des amendements et de v2.0 restent à importer littéralement dans GitHub.**

## Propositions supplémentaires — décision explicite du 7 novembre 2026

| Numéro | Proposition | Statut |
|---|---|---|
| 1 | Matrice de coexistence des fonctionnalités | EN ATTENTE |
| 2 | EDID, HPD, émulation et continuité des connexions | EN ATTENTE |
| 3 | Protocole de mesures de latence normalisées, comparables et reproductibles | **VALIDÉ** |
| 4 | Scénarios de fonctionnement multi-appareils en conditions réelles | EN ATTENTE |
| 5 | Sécurité, confidentialité et isolation entre appareils | **VALIDÉ** |
| 6 | Calibration avancée, LUT, ICC, tone mapping, HGiG, EOTF | **VALIDÉ** |
| 7 | Confort visuel mesuré, textes, PWM, reflets et usages prolongés | **VALIDÉ** |
| 8 | Vieillissement, réparabilité et garanties par région | **VALIDÉ** |
| 9 | Registre structuré des preuves et export CSV/JSON/XLSX | **VALIDÉ** |
| 10 | Frontière de Pareto et comparatifs d'efficacité réelle | **VALIDÉ** |

**Ne pas déclarer les sept propositions ci-dessus déjà fusionnées dans le prompt v2.1.** Elles sont approuvées pour une révision future, mais restent à intégrer textuellement.

## Gouvernance

- Aucune modification de `main` sans revue de la PR.
- Aucun écrasement des anciens prompts : versions historiques et diffs conservés.
- Toute capacité réputée confirmée doit être étayée par une preuve datée.
- Toute nouvelle décision sera ajoutée chronologiquement à ce journal.
- Un avis technique, une suggestion ou une absence de réponse ne constitue pas une validation.
