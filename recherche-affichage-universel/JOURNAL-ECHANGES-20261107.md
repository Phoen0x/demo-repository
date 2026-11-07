# Rapport chronologique des échanges — 7 novembre 2026

## Statut et périmètre

**Synthèse fidèle des décisions**, et non transcription littérale de messages privés. Les phrases entre guillemets signalées « verbatim » sont de courts extraits effectivement présents dans la conversation ; les autres formulations sont des synthèses. Ce fichier est destiné à un dépôt public : il évite les informations privées sans rapport avec l'étude.

## Échange 1 — comparaison des versions

L'utilisatrice fournit intégralement :
- un prompt plus récent intitulé « MISSION — RECHERCHE EXHAUSTIVE DES MEILLEURS ÉCRANS ET SYSTÈMES D'AFFICHAGE UNIVERSELS — Version 2.0 — Cahier des charges consolidé » ;
- son prédécesseur intitulé « Mission : recherche exhaustive des meilleurs écrans et systèmes d'affichage universels ».

Elle demande de vérifier que la v2.0 ne perd aucune exigence et de formuler des remarques.

L'audit conclut : forte conservation et enrichissement substantiel, mais précisions perdues ou implicites, surtout sur variantes Apple/Android, G-SYNC, câbles/adaptateurs, MST macOS, recharge/veille USB, maintenance interne, KVM, audio, contrôle multiplateforme, éclairage, catégories d'indétermination et reproductibilité des scores. La v2.0 change volontairement USB 3.x obligatoire en USB 2.0 minimum ; le statut des USB-A uniquement recharge reste ambigu.

## Échange 2 — premières validations

L'utilisatrice valide intégralement le **point 3** de l'audit et les remarques **5A, 5B, 5C, 5D**. Elle indique : « on verra le reste plus tard ».

**Conséquence :** les autres recommandations ne deviennent pas validées.

## Échange 3 — amendements v2.1

À sa demande « vas modifie le prompt », l'assistant rédige **Version 2.1 — Amendements correctifs validés**, 15 amendements A1–A15 couvrant les validations, à ajouter sans effacer v2.0. Ce n'est **pas** une refonte fusionnée ni une modification rétroactive du texte v2.0.

## Échange 4 — nouvelles idées

L'utilisatrice demande d'autres améliorations. Dix propositions sont formulées :
1 coexistence ; 2 EDID/HPD ; 3 mesures ; 4 scénarios multi-appareils ; 5 sécurité ; 6 colorimétrie ; 7 confort ; 8 longévité ; 9 registre ; 10 Pareto.

## Échange 5 — validations des dix propositions

L'utilisatrice demande explicitement de **ne pas oublier les propositions précédentes**. Elle valide **3, 5, 6, 7, 8, 9 et 10**. Elle ne valide ni ne rejette **1, 2 et 4**.

Elle suggère de conserver le projet dans un dépôt GitHub existant inutilisé, sans sacrifier le suivi historique.

## Échange 6 — initialisation GitHub

Une PR de brouillon est créée dans `Phoen0x/demo-repository`, sur `docs/recherche-affichage-universel-20261107` : [PR #4](https://github.com/Phoen0x/demo-repository/pull/4).

Elle contient initialement `README.md`, `DECISIONS.md`, `PROPOSITIONS_EN_ATTENTE.md`, `REGISTRE_DES_PREUVES.md`, dans `recherche-affichage-universel/`. Elle ne modifie pas `main`.

## Échange 7 — demande d'archivage historique

L'utilisatrice demande : « fout original + v1 + v2 + rapport des dernieres propositions + rapport des echange sur github si pas deja fait ».

**Interprétation de conservation :** archiver séparément les textes réellement fournis, indiquer avec transparence les versions dont la provenance ou le texte complet n'ont pas été retrouvés, sans inventer de version historique. Ajouter le rapport de propositions et le présent journal. Réutiliser la PR brouillon, sans suppression ni fusion automatique.

## Règles de tenue du journal

- Ne jamais transformer une proposition en décision approuvée.
- Ajouter toute modification significative chronologiquement.
- Ne pas fabriquer de texte original pour combler une version manquante.
- Conserver les documents sources en lecture historique et publier les révisions en nouveaux fichiers/commits.
- Protéger les détails privés dans ce dépôt public.
