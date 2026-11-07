# MISSION — RECHERCHE EXHAUSTIVE DES MEILLEURS ÉCRANS ET SYSTÈMES D'AFFICHAGE UNIVERSELS

## Version 2.1 — Amendements correctifs validés

**Document de référence :** « Version 2.0 — Cahier des charges consolidé », sections 1 à 20.

**Règle de conservation :** toutes les dispositions de la version 2.0 demeurent applicables. Les présentes dispositions les complètent et les précisent. Elles ne suppriment aucune exigence, aucun critère de notation, aucun classement ni aucun livrable.

Les exigences USB 2.0 minimum, les six pondérations générales et les vingt verdicts restent inchangés.

Les arbitrages non explicitement effectués, notamment le statut éliminatoire éventuel des ports USB-A exclusivement dédiés à la recharge, demeurent en suspens. Aucun nouvel arbitrage ne doit être présumé.

---

## A1. Complément à la section 2 — Compatibilité des appareils mobiles

Pour les appareils Apple et Android, étudier explicitement les différences de compatibilité selon :

- Le modèle exact et sa génération.
- La version d'iOS, d'iPadOS, d'Android ou de GrapheneOS.
- Le connecteur physique.
- Les protocoles vidéo effectivement disponibles.
- Les modes USB hôte et périphérique.
- La reconnaissance des périphériques USB et HID.
- Les capacités de recharge.
- Les restrictions logicielles et les autorisations système.
- Le fonctionnement des hubs, docks et KVM.
- Les fonctionnalités pouvant être utilisées simultanément.

Pour les appareils mobiles en général, distinguer la possibilité de connecter un périphérique, sa reconnaissance effective, ses fonctions exploitables et ses performances réelles.

Pour les périphériques à haute fréquence d'interrogation, vérifier séparément les restrictions des appareils hôtes, systèmes, pilotes, récepteurs, hubs et KVM.

### Cas particulier de la Nintendo Switch Lite

Nintendo Switch Lite ne doit pas être présentée comme disposant d'une sortie vidéo externe native équivalente aux autres modèles Switch.

Distinguer explicitement :

1. Sortie vidéo native officiellement prise en charge.
2. Fonctionnement avec une station d'accueil officielle.
3. Compatibilité d'un adaptateur USB-C/HDMI ordinaire.
4. Modification matérielle spécialisée.
5. Capture externe ou retransmission de l'image.
6. Solution expérimentalement démontrée.
7. Solution théorique non validée.

Une modification matérielle exceptionnelle ou un dispositif de capture ne doit jamais être assimilé à une fonctionnalité native.

Préciser les coûts, risques, limitations, conséquences sur la garantie et restrictions logicielles des solutions particulières.

---

## A2. Complément à la section 4 — Certifications et architectures G-SYNC

Étudier explicitement les différences entre :

- NVIDIA G-SYNC Compatible.
- NVIDIA G-SYNC avec processeur matériel dédié.
- NVIDIA G-SYNC Ultimate.
- NVIDIA G-SYNC Pulsar.
- Implémentations utilisant un scaler ou contrôleur intégré sans module NVIDIA dédié.
- Autres architectures matériellement ou fonctionnellement comparables.

Pour chaque modèle, rechercher :

1. L'architecture matérielle réellement utilisée.
2. La présence éventuelle d'un processeur NVIDIA dédié.
3. La certification effectivement obtenue.
4. Les plages VRR réelles.
5. Les technologies d'overdrive disponibles.
6. Les performances mesurées.
7. Les restrictions HDR, VRR et strobing.
8. Les différences entre modes certifiés et non certifiés.
9. Les fonctions réellement disponibles selon le firmware.
10. Les éventuels conflits entre fonctionnalités.

Un écran G-SYNC Compatible ne doit pas être considéré comme équivalent à un écran équipé d'un processeur NVIDIA dédié sans vérification.

Inversement, un écran sans module dédié ne doit pas être automatiquement considéré comme inférieur lorsqu'il obtient de meilleures performances mesurées.

---

## A3. Complément à la section 7 — Câbles, adaptateurs et chaînes vidéo

Vérifier explicitement les caractéristiques et limitations des câbles et adaptateurs nécessaires aux configurations étudiées.

### Câbles

Étudier :

- Câbles HDMI.
- Câbles DisplayPort.
- Câbles USB-C.
- Câbles USB4.
- Câbles Thunderbolt.
- Câbles actifs et passifs.
- Câbles optiques lorsque pertinents.
- Longueurs maximales fonctionnelles.
- Certifications réellement obtenues.
- Qualité du blindage.
- Restrictions selon la longueur et la conception.
- Compatibilité des câbles avec les modes vidéo et USB simultanés.
- Limitations introduites par les câbles fournis avec les équipements.

### Adaptateurs

Étudier :

- Adaptateurs actifs et passifs.
- Convertisseurs HDMI/DisplayPort.
- Adaptateurs USB-C vidéo.
- Adaptateurs Thunderbolt et USB4.
- Convertisseurs bidirectionnels et unidirectionnels.
- Adaptateurs vidéo avec alimentation supplémentaire.
- Adaptateurs conservant ou supprimant certaines fonctions avancées.

Vérifier individuellement :

- Résolutions et fréquences.
- HDR.
- VRR.
- DSC.
- HDCP.
- CEC.
- EDID.
- Audio.
- MST.
- Recharge.
- Débits USB.
- Fonctionnement simultané.
- Sens réel de conversion.
- Éventuelle latence supplémentaire.

Ne pas présumer qu'un adaptateur transmet une fonction simplement parce que cette fonction existe sur ses deux interfaces physiques.

### Restrictions DisplayPort et macOS

Rechercher explicitement les différences de prise en charge du MST, des écrans multiples et des fonctions d'extension vidéo entre :

- Windows.
- Linux.
- macOS.
- Mac Intel.
- Mac Apple Silicon.
- Différentes générations de processeurs Apple.
- Versions du système et firmwares concernés.

Ne pas assimiler le fonctionnement d'un dock DisplayPort MST sous Windows à une compatibilité identique sous macOS.

### Vérification complète de la chaîne

La compatibilité doit être vérifiée sur l'ensemble du trajet :

**Appareil source → câble → adaptateur éventuel → dock/switch/KVM/processeur éventuel → câble → écran.**

La capacité maximale de cette chaîne est déterminée par ses contraintes réelles et par les fonctions effectivement transmissibles à chaque étape.

Ne jamais attribuer à une chaîne complète la capacité maximale annoncée pour un seul de ses composants.

---

## A4. Complément à la section 7 — HDMI 2.2, Ultra96 et bande passante certifiée

Pour HDMI 2.2 et les révisions ultérieures, distinguer :

- La version de la spécification.
- Le débit maximal théorique prévu par cette spécification.
- Le débit réellement implémenté par l'appareil source.
- Le débit réellement implémenté par l'appareil récepteur.
- Le débit certifié du câble.
- Le débit maximal des équipements intermédiaires.
- Le débit effectivement négocié.
- Les fonctionnalités qui restent utilisables simultanément.

Ne pas interpréter systématiquement le marquage Ultra96 comme la preuve d'une transmission effective à 96 Gbit/s.

Étudier les capacités et certifications correspondant aux différents niveaux de débit, notamment 64, 80 et 96 Gbit/s lorsqu'ils sont applicables.

Vérifier les exigences et résultats de certification du câble et de l'ensemble des équipements.

Distinguer les débits physiques annoncés des débits utiles réellement disponibles pour les données vidéo.

La présence d'un connecteur compatible HDMI 2.2 ne démontre pas à elle seule que l'équipement exploite toutes les capacités de la spécification.

---

## A5. Complément à la section 9 — Recharge, alimentation et fonctionnement en veille

Restaurer une étude détaillée de la recharge sur tous les ports pertinents.

Vérifier :

- La puissance maximale annoncée.
- La puissance réellement négociée.
- Les tensions et intensités disponibles.
- USB Power Delivery.
- PPS.
- EPR.
- Les autres protocoles de charge rapide pris en charge.
- Les restrictions propres aux appareils sources.
- La recharge des smartphones.
- La recharge des tablettes.
- La recharge des ordinateurs portables.
- La recharge des manettes.
- La recharge simultanée de plusieurs appareils.
- Le partage de puissance entre les ports.
- La réduction éventuelle de puissance lorsque plusieurs périphériques sont connectés.

### Alimentation en veille

Vérifier séparément le fonctionnement des ports USB dans les états suivants :

1. Écran allumé.
2. Écran en veille.
3. Veille profonde.
4. Écran éteint par son bouton.
5. Équipement alimenté mais sans source vidéo active.
6. Équipement déconnecté de son hôte USB.
7. Changement de source vidéo.
8. Changement d'hôte KVM.

Préciser si les ports conservent :

- Leur alimentation.
- Leurs fonctions de recharge.
- Leur capacité de transfert de données.
- La connexion des périphériques.
- Leur capacité de réveil ou de contrôle.

Ne pas assimiler la présence d'une alimentation USB à la disponibilité d'une liaison de données.

### Interfaces USB internes et maintenance

Les ports et interfaces exclusivement internes, réservés à la fabrication, au diagnostic matériel ou à la maintenance non accessible à l'utilisateur, doivent être identifiés séparément lorsqu'ils sont documentés.

Ils ne sont pas soumis aux exigences éliminatoires relatives aux ports de données accessibles à l'utilisateur.

Distinguer les interfaces réellement accessibles de celles nécessitant un démontage, un outillage spécialisé ou une intervention interne.

Cette précision ne modifie pas l'exigence USB 2.0 minimum des ports de données utilisateur de la version 2.0.

---

## A6. Complément à la section 9 — Interférences USB 3.x et récepteurs radio 2,4 GHz

Étudier explicitement les interférences électromagnétiques pouvant affecter les périphériques sans fil lorsque leurs récepteurs sont utilisés à proximité d'équipements USB 3.x.

Rechercher notamment :

- Les perturbations dans la bande 2,4 GHz.
- Les interférences générées par certains câbles USB SuperSpeed.
- Les perturbations liées aux SSD et stockages externes.
- La proximité entre ports USB et dongles.
- Les effets du blindage des câbles.
- Les effets du blindage des boîtiers et hubs.
- L'influence de l'emplacement physique des récepteurs.
- Les interférences entre plusieurs dongles.
- Les différences entre ports USB 2.0 et USB 3.x.
- L'effet des rallonges USB.
- L'effet de l'éloignement physique du récepteur.
- L'influence de l'activité simultanée des périphériques USB.

### Tests à comparer

Lorsque les données sont disponibles, comparer :

1. Dongle directement connecté au PC.
2. Dongle connecté à un port USB 2.0.
3. Dongle connecté à un port USB 3.x.
4. Dongle connecté à un hub USB 2.0.
5. Dongle connecté à un hub USB 3.x.
6. Dongle derrière un KVM.
7. Dongle connecté avec une rallonge USB.
8. Dongle placé près d'un SSD USB 3.x actif.
9. Deux dongles utilisés simultanément.
10. Récepteur partagé entre plusieurs périphériques.
11. Périphériques 2K, 4K et 8K lorsque pertinents.

Mesurer ou rechercher :

- Latence.
- Jitter.
- Intervalles entre rapports.
- Pertes d'événements.
- Déconnexions.
- Stabilité radio.
- Sensibilité aux interférences.
- Distance maximale fiable.
- Performances sous charge.

Ne pas conclure qu'USB 3.x offre nécessairement une meilleure expérience pour un dongle HID que l'USB 2.0.

La sélection doit reposer sur les performances réellement obtenues avec les périphériques concernés.

---

## A7. Complément à la section 10 — KVM, pilotes et reconnexions

Pour chaque KVM et système de partage des périphériques, vérifier indépendamment le fonctionnement selon les appareils hôtes et leurs systèmes d'exploitation.

Étudier :

- Windows.
- Linux.
- macOS.
- PlayStation.
- Xbox.
- Nintendo.
- Android.
- GrapheneOS.
- iOS/iPadOS lorsque pertinent.

Vérifier les différences selon :

- Les pilotes.
- Les versions des systèmes.
- Les firmwares.
- Les contrôleurs USB.
- Les modes d'émulation HID.
- Les modes de transparence USB.
- Les logiciels propriétaires.
- Les périphériques nécessitant une configuration spécifique.

### Essais après basculement

Ne pas limiter les tests à la reconnaissance initiale.

Vérifier :

1. La reconnexion automatique.
2. Le délai de reconnexion.
3. La conservation des paramètres.
4. La conservation des fréquences de rapports.
5. Les changements d'identité USB.
6. La perte éventuelle d'interfaces HID.
7. Le fonctionnement des dongles propriétaires.
8. Le comportement des périphériques composites.
9. La nécessité éventuelle de débrancher ou réinitialiser un périphérique.
10. La stabilité après plusieurs basculements successifs.
11. Le fonctionnement en sortie de veille.
12. Les différences selon le système d'exploitation.

Distinguer les limitations propres au KVM des limitations provenant de l'hôte, des pilotes ou du périphérique.

---

## A8. Complément à la section 11 — Mesures de latence audio et microphone

Pour les systèmes audio et microphones, rechercher séparément :

- Latence de sortie audio.
- Latence d'entrée microphone.
- Latence du transport du microphone.
- Latence audio aller-retour lorsque pertinente.
- Latence de conversion analogique-numérique.
- Latence de conversion numérique-analogique.
- Latence ajoutée par les périphériques USB.
- Latence ajoutée par les connexions Bluetooth.
- Latence ajoutée par les dongles RF.
- Latence ajoutée par les équipements HDMI, ARC/eARC ou intermédiaires audio.
- Variations selon les codecs, fréquences d'échantillonnage et tailles de buffer.

Préciser la méthode de mesure et les conditions des essais.

Ne pas comparer directement des mesures de latence audio réalisées avec des méthodes incompatibles.

Distinguer la disponibilité d'une entrée microphone, sa reconnaissance par l'appareil source et son fonctionnement effectif dans les communications vocales et les jeux.

---

## A9. Complément à la section 12 — Contrôle logiciel multiplateforme

Pour chaque moniteur ou équipement configurable, vérifier séparément les possibilités de contrôle sous :

- Windows.
- Linux.
- macOS.

Préciser les versions des systèmes réellement étudiées.

Rechercher :

- Les logiciels constructeurs.
- Les logiciels libres et open source.
- Les outils DDC/CI.
- Les interfaces MCCS.
- Les interfaces USB HID.
- Les API locales.
- Les interfaces réseau.
- Les logiciels compatibles avec les KVM.
- Les possibilités de contrôle de l'OSD.
- La lecture des paramètres.
- La modification des paramètres.
- La gestion des profils.
- La sauvegarde des configurations.
- La restauration des configurations.
- Les mises à jour firmware.
- Les diagnostics accessibles.
- L'automatisation locale.

Distinguer les fonctionnalités proposées officiellement, celles réellement testées et celles rendues possibles par des outils communautaires.

Ne pas présumer qu'une application disponible sous Windows possède un équivalent fonctionnel sous Linux ou macOS.

---

## A10. Complément à la section 13 — Personnalisation de l'éclairage ambiant

Pour Ambilight, Ambiglow, Hue, Govee et les solutions comparables, rechercher également :

- Les profils lumineux propres aux jeux.
- Les profils lumineux propres aux films.
- Les profils propres aux différentes entrées.
- Les profils personnalisés.
- Les profils statiques et dynamiques.
- La synchronisation avec le contenu vidéo.
- La synchronisation avec le contenu audio.
- Les possibilités de commutation automatique.
- Les profils mémorisables.
- Les réglages de couleur, intensité et zones.
- La disponibilité du contrôle local.
- L'utilisation sans compte cloud lorsque possible.

Vérifier quelles fonctions restent disponibles selon la résolution, la fréquence, le HDR, le VRR et les limitations HDCP.

Ne pas confondre les fonctionnalités directement intégrées à l'écran avec celles nécessitant un équipement externe.

---

## A11. Complément à la section 8 — Validation historique du HDMI-CEC sur PS4

Les démonstrations historiques publiées par stb-tester et les autres sources techniques doivent être analysées fonction par fonction.

L'existence d'un contrôle HDMI-CEC sur une PlayStation ne permet pas de conclure automatiquement que toutes les commandes système sont accessibles.

Vérifier séparément, avec des preuves propres à chaque fonction :

1. La mise sous tension.
2. La mise en veille.
3. La navigation dans les menus.
4. La sélection d'un élément.
5. Le retour arrière.
6. L'accès aux fonctions multimédias.
7. La validation de l'écran de connexion utilisateur.
8. Le franchissement de l'écran demandant d'appuyer sur PS.
9. La transmission effective de l'équivalent de la touche PS.
10. L'association initiale d'une DualShock 4.
11. Le fonctionnement sans manette déjà associée.
12. Le fonctionnement sur une PS4 Slim.
13. Le fonctionnement avec les firmwares ultérieurs.
14. Le fonctionnement avec HDMI-CEC préalablement activé.
15. Le fonctionnement lorsque HDMI-CEC est désactivé.

### Exigence de reproductibilité

Lorsqu'une fonction a été historiquement démontrée, préciser :

- La date.
- La source.
- La console exacte.
- Le firmware lorsqu'il est identifiable.
- L'équipement HDMI-CEC utilisé.
- Les commandes transmises.
- Les résultats observés.
- Les conditions préalables.
- Les restrictions.
- La possibilité de reproduire l'essai aujourd'hui.

Ne jamais étendre les résultats obtenus sur une génération ou un firmware à toutes les PS4.

Distinguer une connexion utilisateur réussie, la transmission réelle d'une touche PS et l'association Bluetooth d'une manette : ce sont des opérations différentes.

Les solutions proposées pour la PS4 Slim actuellement bloquée doivent privilégier les essais non destructifs et ne doivent pas présenter une simple possibilité théorique comme une résolution confirmée.

---

## A12. Complément aux sections 17 à 19 — Gestion rigoureuse des candidats

Conserver obligatoirement trois catégories de présentation distinctes :

### 1. Candidats conformes confirmés

Les exigences éliminatoires applicables sont satisfaites avec des preuves suffisantes.

Ils peuvent intégrer les classements principaux.

Une conformité conditionnelle n'est admissible dans ces classements que si les conditions nécessaires sont explicitement satisfaites et documentées dans la configuration évaluée.

### 2. Candidats non conformes confirmés

Une incompatibilité avec une exigence éliminatoire est démontrée.

Ils ne doivent pas apparaître comme conformes dans les classements principaux.

Ils peuvent être conservés dans un classement secondaire explicitement identifié comme non conforme, notamment lorsqu'ils présentent un intérêt historique ou technique.

### 3. Candidats à conformité indéterminée

Les informations restent insuffisantes, ambiguës ou contradictoires pour vérifier une exigence éliminatoire.

Ces candidats ne doivent être déclarés ni conformes ni non conformes sans preuve suffisante.

Ils sont conservés dans une catégorie distincte intitulée :

**« Candidats à conformité indéterminée »**

Pour chacun, documenter :

- Les exigences confirmées.
- Les exigences non conformes confirmées lorsqu'elles existent.
- Les exigences restant inconnues.
- Les sources consultées.
- Les recherches complémentaires effectuées.
- Les contradictions éventuelles.
- Les hypothèses restantes.
- Les vérifications encore nécessaires.
- Le niveau de confiance.
- Les raisons justifiant son maintien dans le catalogue.

Ne pas appliquer automatiquement à ces candidats la même pénalité qu'à ceux dont la non-conformité est démontrée.

Ne pas leur attribuer non plus une conformité présumée.

Réintégrer les candidats dans les classements appropriés dès que de nouvelles preuves permettent de statuer.

Les quatre statuts fonctionnels de la section 17 demeurent applicables : conforme confirmé, non conforme confirmé, conformité conditionnelle et conformité indéterminée.

---

## A13. Complément à la section 18 — Notation et niveaux de confiance

Avant d'attribuer les scores, définir et publier les sous-critères utilisés à l'intérieur des six catégories de notation.

Pour chaque sous-critère, préciser :

1. Sa définition.
2. Son poids dans la catégorie.
3. Les méthodes d'évaluation.
4. Les unités et indicateurs pertinents.
5. Les sources admissibles.
6. Les conditions des essais.
7. Le traitement des données inconnues.
8. Le traitement des fonctions non applicables.
9. La gestion des fonctionnalités conditionnelles.
10. La méthode utilisée pour éviter les doubles comptabilisations.

Appliquer les mêmes règles aux candidats comparables.

### Niveaux de confiance

Associer à chaque évaluation un niveau de confiance explicite :

- Élevé.
- Moyen.
- Faible.

Justifier ce niveau selon la qualité, le nombre, la cohérence, la date et l'indépendance des sources disponibles.

Distinguer :

- Mesures instrumentées reproductibles.
- Essais documentés.
- Spécifications officielles détaillées.
- Certifications.
- Déclarations commerciales.
- Retours d'utilisateurs.
- Hypothèses techniques.
- Informations insuffisantes.

Une fonction simplement supposée ne doit pas apporter de points.

Une fonction non documentée ne doit pas entraîner automatiquement une pénalité identique à une incompatibilité démontrée.

Lorsqu'une note complète ne peut pas être calculée de façon sérieuse, présenter les sous-scores effectivement justifiables et signaler les composantes indéterminées.

### Comparabilité des classements A et B

Conserver exactement les pondérations générales :

| Critère | Pondération |
|---|---:|
| Compatibilité consoles et appareils | 25 % |
| Qualité d'image et gaming | 20 % |
| Connectique et fonctionnalités USB | 20 % |
| Contrôle HDMI-CEC et KVM | 20 % |
| Audio, personnalisation et ergonomie | 10 % |
| Prix, fiabilité et évolutivité | 5 % |
| **Total** | **100 %** |

Les mêmes méthodes de notation doivent être appliquées aux deux classements, sous réserve des différences explicitement définies entre fonctions natives et fonctions apportées par l'architecture modulaire.

Les bonus importants doivent continuer à peser davantage que les bonus secondaires à l'intérieur des catégories pertinentes.

Aucune incompatibilité éliminatoire ne doit être masquée par une bonne moyenne pondérée.

---

## A14. Complément à la section 19 — Séparation des classements

Pour chacun des classements A et B :

1. Présenter les candidats conformes confirmés.
2. Présenter séparément les candidats à conformité indéterminée.
3. Présenter éventuellement les candidats non conformes dans une comparaison secondaire distincte.
4. Identifier les fonctions conditionnelles et les conditions nécessaires.
5. Ne pas désigner comme vainqueur confirmé un équipement dont une exigence éliminatoire reste indéterminée.
6. Ne pas masquer les limitations par les scores.
7. Fournir les niveaux de confiance.
8. Réexaminer les candidats indéterminés lorsque de nouvelles informations deviennent disponibles.

Pour le classement A, vérifier que toutes les fonctions comptabilisées appartiennent nativement à l'écran ou au téléviseur.

Pour le classement B, vérifier le fonctionnement de la chaîne complète, sans présumer l'interopérabilité à partir des seules fiches de ses composants.

Les candidats non conformes peuvent rester dans le catalogue historique et technique, mais ils ne doivent pas être présentés comme satisfaisant les exigences obligatoires.

---

## A15. Complément à la section 20 — Présentation et traçabilité

Les conclusions devront intégrer les nouvelles vérifications suivantes :

- Matrice des restrictions Apple et Android selon les modèles et versions système.
- Distinction des architectures matérielles G-SYNC.
- Inventaire des câbles et adaptateurs nécessaires.
- Vérification des certifications et débits HDMI 2.2/Ultra96.
- Restrictions macOS et DisplayPort MST.
- Recharge et alimentation des ports USB en veille.
- Inventaire séparé des interfaces USB internes de maintenance.
- Analyse des interférences USB 3.x et 2,4 GHz.
- Essais de reconnexion et de stabilité des KVM.
- Mesures distinctes des latences audio et microphone.
- Matrice de contrôle logiciel Windows/Linux/macOS.
- Profils et automatisations d'éclairage ambiant.
- Tableau de preuves HDMI-CEC fonction par fonction sur PS4.
- Classements séparés des candidats conformes, non conformes et indéterminés.
- Sous-critères de notation définis avant l'évaluation.
- Niveau de confiance justifié de chaque score.

Pour toutes les données importantes, préciser les références exactes, les dates, les conditions de test et les sources.

Les informations contradictoires doivent rester visibles tant qu'elles ne sont pas résolues.

Aucune mesure ne doit être inventée.

---

## Principe de conservation final — Version 2.1

Les présentes dispositions complètent la version 2.0 sans la remplacer.

Sont expressément conservés :

- Les vingt sections du cahier des charges consolidé.
- La recherche mondiale et multigénérationnelle.
- Le minimum USB 2.0 et les exigences quantitatives des deux classements.
- Les quatre statuts de conformité.
- Les six pondérations générales.
- La hiérarchie des bonus importants et secondaires.
- Les vingt verdicts généraux et spécialisés.
- L'analyse des périphériques 2K/4K/8K.
- Les exigences de transparence HID des hubs et KVM.
- Les distinctions entre contrôle HDMI-CEC, USB HID, Bluetooth et émulation de manette.
- La priorité accordée à la préservation du firmware et des données de la PS4 Slim.
- La séparation entre fonctions natives, logicielles et apportées par des accessoires.
- L'interdiction de présumer une compatibilité universelle sans preuves.

**Aucune disposition non validée lors de la révision ne doit être introduite implicitement.**

En cas d'ambiguïté entre une nouvelle précision et une exigence déjà définie, préserver les règles de la version 2.0 et signaler l'ambiguïté au lieu d'inventer un arbitrage.

L'objectif demeure d'identifier les meilleures solutions réellement compatibles, performantes, simultanément exploitables, fiables, évolutives et documentées, sans favoriser artificiellement une génération, une technologie ou une certification.