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

