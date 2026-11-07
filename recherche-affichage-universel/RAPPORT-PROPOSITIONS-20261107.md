# Rapport des propositions — 7 novembre 2026

> **Instantané historique** : les statuts ci-dessous reflètent la première synthèse du 7 novembre. Depuis, la proposition **1** a été validée et intégrée en v2.3 ; les propositions **2 et 4** restent en attente. Se reporter à [DECISIONS.md](DECISIONS.md) pour l'état à jour.

**Portée :** audit du prompt antérieur contre la v2.0, rédaction d'amendements v2.1, puis nouvelles propositions. Ce document distingue **validé**, **proposé** et **non arbitré**. Il ne remplace ni les prompts complets ni le journal des décisions.

## 1. Audit comparatif — corrections VALIDÉES

L'utilisatrice valide **tout le point 3** du rapport comparatif, soit :
1. Vérification explicite des compatibilités mobiles par modèle/OS/connecteur/protocole.
2. Distinction entre les technologies G-SYNC (module matériel dédié, scaler intégré, Compatible).
3. Vérification des adaptateurs actifs/passifs, certifications et caractéristiques des câbles.
4. Vérification des restrictions macOS/MST.
5. Recharge rapide, puissance réellement négociée et alimentation des ports USB en veille.
6. Distinction des interfaces USB internes réservées à la fabrication/maintenance.
7. Vérifications KVM par OS/pilotes, après changement d'hôte.
8. Latences séparées du microphone et aller-retour audio.
9. Contrôle des moniteurs sous Windows, Linux et macOS.
10. Profils lumineux selon jeu, film ou entrée.
11. Catégorie indépendante « Candidats à conformité indéterminée ».
12. Sous-critères de notation définis avant la recherche et niveaux de confiance.
13. Classement secondaire explicite des candidats non conformes.

L'utilisatrice valide également **les remarques 5A–5D** de ce rapport :
- **A** : interférences USB 3.x et dongles 2,4 GHz, blindage, emplacement et charge ;
- **B** : Switch Lite : ne pas confondre sortie vidéo native, modification matérielle et capture ;
- **C** : vérifier séparément les preuves historiques de contrôle CEC des PS4 (navigation, connexion, touche PS, association DS4, modèle/firmware) ;
- **D** : HDMI 2.2/Ultra96 : débit réellement certifié, transmis et négocié sur la chaîne complète.

**Statut :** ces dispositions ont été rédigées sous forme d'amendements A1–A15 au-dessus de la v2.0, dans la réponse intitulée « Version 2.1 — Amendements correctifs validés ».

## 2. Série ultérieure de dix propositions

| No | Proposition | Statut | Observations |
|---:|---|---|---|
| 1 | Matrice de coexistence des fonctionnalités | EN ATTENTE | Vérification systématique HDR/VRR/USB/KVM/dongles simultanés, au-delà des tests existants |
| 2 | Continuité EDID/HPD et émulation HID | EN ATTENTE | Persistance des écrans et périphériques lors de commutations |
| 3 | Protocole commun de mesure de latence | **VALIDÉ** | Séparer input lag, temps de réponse, persistance, clic-vers-photon, conditions et instruments |
| 4 | Scénarios complets de fonctionnement multi-appareils | EN ATTENTE | Recettes d'essais à froid/veille/commutations/pannes |
| 5 | Sécurité, confidentialité et isolation | **VALIDÉ** | Smart Monitors, KVM IP, docks réseau, mises à jour, télémétrie et cloud |
| 6 | Calibration et chaîne colorimétrique | **VALIDÉ** | LUT 1D/3D, ICC, tone mapping, HGiG, EOTF, calibration par entrée |
| 7 | Confort visuel mesuré | **VALIDÉ** | Netteté des textes selon OS, sous-pixels, PWM, reflets, persistance |
| 8 | Vieillissement, réparabilité, garanties | **VALIDÉ** | Burn-in, pannes, pièces, garantie régionale et coûts d'import |
| 9 | Registre des preuves et exports | **VALIDÉ** | Identifiants, références, conditions, sources, CSV/JSON/XLSX |
| 10 | Pareto et efficacité réelle | **VALIDÉ** | Solutions non dominées, au-delà de la seule note pondérée |

**Important :** les propositions 3, 5, 6, 7, 8, 9 et 10 sont **approuvées pour intégration ultérieure**, mais ne doivent pas être présentées comme déjà insérées mot à mot dans les 20 sections de v2.0 ni dans les amendements A1–A15.

## 3. Autres propositions antérieures NON ARBITRÉES

- **USB-A uniquement recharge** : l'ancien prompt interdisait ces ports sur les composants évalués, même en présence d'autres ports conformes ; la v2.0 ne les compte pas parmi les ports de données sans réaffirmer cette interdiction. Aucun arbitrage définitif.
- **Méthode en cinq phases** : inventaire mondial ; vérification éliminatoire ; investigation détaillée ; validation de chaînes modulaires ; classements. Suggérée, non approuvée.
- **Taxonomie des dalles (ancienne remarque 5E)** : séparer la technologie de dalle (IPS/VA), le rétroéclairage (Mini-LED) et les architectures OLED (WOLED/QD-OLED). Suggérée, non approuvée.
- **Dernière série, points 1, 2, 4** : explicitement en attente.

## 4. Contraintes qui NE CHANGENT PAS

- Ni budget, taille ou génération imposés arbitrairement.
- USB 2.0 matériel minimum sur les ports de données accessibles ; deux USB-A de données minimum pour A (natif) ou B (système entier).
- Six poids 25/20/20/20/10/5.
- Classement A écran autonome / classement B système modulaire.
- Vingt verdicts.
- Preuves testées et compatibilités conditionnelles clairement distinguées.
- Aucune modification de `main` sans revue ; PR brouillon.
