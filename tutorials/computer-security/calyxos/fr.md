---
name: CalyxOS
description: Un système d'exploitation Android dégooglisé axé sur la confidentialité et l'utilisabilité
---

![cover](assets/cover.webp)

> ⚠️ **AVERTISSEMENT IMPORTANT (Août 2025)** : Le Calyx Institute a annoncé une pause temporaire du développement CalyxOS suite au départ de membres clés de l'équipe. Les mises à jour de sécurité sont interrompues pour une période estimée de 4-6 mois. Le Calyx Institute recommande officiellement aux utilisateurs actuels de migrer vers d'autres distributions comme GrapheneOS en attendant la reprise du développement. Ce tutoriel reste disponible à titre informatif.

Dans un monde où nos smartphones sont devenus des extensions numériques de nous-mêmes, la question de la vie privée sur mobile n'a jamais été aussi cruciale. Android, malgré sa popularité, transforme votre téléphone en dispositif de surveillance : collecte massive de données, géolocalisation permanente, télémétrie constante vers Google.

**CalyxOS** émerge comme une réponse élégante développée par le Calyx Institute, organisation à but non lucratif dédiée à la défense de la vie privée numérique. Ce système d'exploitation Android alternatif place la confidentialité au cœur de sa conception tout en visant l'équilibre entre protection des données et expérience utilisateur fluide.

Basé sur AOSP (Android Open Source Project), CalyxOS supprime tous les composants espions de Google tout en conservant la compatibilité Android via microG et un écosystème d'applications FOSS pré-installées.

### Philosophie et objectifs

Le projet CalyxOS répond à trois objectifs fondamentaux :

**Dégooglisation complète** : Suppression de tous les composants Google de collecte de données. Aucune télémétrie, synchronisation forcée ou compte Google requis.

**Compatibilité préservée** : L'intégration de microG, réimplémentation libre des services Google Play, maintient la compatibilité avec la majorité des applications Android sans compromettre la vie privée.

**Expérience utilisateur optimisée** : Interface intuitive, fonctionnalités modernes préservées, système fonctionnel "out of the box" sans configuration complexe.

### Architecture technique

CalyxOS repose sur plusieurs piliers technologiques qui garantissent sa sécurité et sa fiabilité :

**Base AOSP durcie** : Version renforcée d'Android avec correctifs de sécurité rapides et protections additionnelles.

**microG intégré** : Réimplémentation open source des API Google Play permettant aux applications de fonctionner sans pistage publicitaire.

**Verified Boot** : Mécanisme vérifiant l'intégrité du système à chaque démarrage.

**Mises à jour OTA sécurisées** : Correctifs mensuels déployés quelques jours après Google.

## Fonctionnalités principales

### Écosystème d'applications FOSS

CalyxOS se distingue par son écosystème d'applications libres pré-installées, soigneusement sélectionnées pour couvrir les besoins essentiels :

**Communication sécurisée** : Signal (messagerie chiffrée), K-9 Mail (e-mails PGP), Briar (P2P hors-ligne).

**Navigation privée** : Tor Browser (anonymat), DuckDuckGo (navigation anti-traqueurs), Organic Maps (cartographie OpenStreetMap).

**Outils de confidentialité** : CalyxVPN, RiseupVPN (chiffrement réseau), Hypatia (antivirus), Scrambled Exif (suppression métadonnées).

**Productivité** : DAVx5 (synchronisation Nextcloud), OONI Probe (détection censure), VLC et suite multimédia.

### Magasins d'applications alternatifs

CalyxOS intègre deux boutiques d'applications complémentaires qui éliminent la dépendance au Google Play Store :

**F-Droid privilégié** : Magasin d'applications open source avec installation automatique. Applications vérifiées sans traqueurs.

**Aurora Store** : Accès anonyme au catalogue Play Store complet sans compte Google via des comptes temporaires.

### Sécurité renforcée

Le système intègre plusieurs couches de protection avancées :

**Chiffrement par défaut** : Toutes les données utilisateur automatiquement chiffrées.

**ID publicitaire randomisé** : Changement régulier empêchant le suivi inter-applications.

**DNS sécurisé** : DNS Quad9 par défaut avec chiffrement DNS-over-HTTPS.

## Appareils compatibles

CalyxOS supporte officiellement un nombre limité d'appareils, principalement pour garantir la qualité et la sécurité de l'installation :

### Google Pixel

Support officiel du Pixel 3a aux modèles récents (Pixel 6, 7, 8+) grâce aux pilotes Google publiés, bootloader déverrouillable et puce Titan M pour la sécurité matérielle. CalyxOS maintient le support au-delà du cycle officiel Google.

### Autres appareils supportés

**Fairphone 4 et 5** : Ces smartphones éthiques et modulaires bénéficient d'un support CalyxOS complet, parfait pour les utilisateurs soucieux de durabilité.

**Motorola série G** : Quelques modèles milieu de gamme (Moto G32, G42, G52) sont supportés, élargissant l'accessibilité de CalyxOS.

### Limitations importantes

**Bootloader verrouillé** : Les appareils vendus par certains opérateurs (notamment Verizon) ont un bootloader définitivement verrouillé, rendant impossible l'installation de CalyxOS.

**Support limité** : Contrairement à LineageOS, il n'existe pas de ports communautaires pour d'autres modèles. Le support officiel est requis pour bénéficier des garanties de sécurité.

## Installation

### Prérequis essentiels

Avant de procéder à l'installation, assurez-vous de disposer de :

- Un smartphone compatible avec bootloader déverrouillable
- Un ordinateur (Windows, macOS ou Linux) avec connexion internet
- Un câble USB de qualité pour relier le téléphone au PC
- Une sauvegarde complète de vos données importantes
- Au moins 50% de charge sur votre appareil
- Environ 30 minutes de temps disponible

**Activation des options développeur** : Dans les paramètres Android, rendez-vous dans "À propos du téléphone" et tapez 7 fois sur le numéro de build pour activer le mode développeur. Activez ensuite "Déverrouillage OEM" et "Débogage USB" dans les options développeur.

### Installation avec l'outil automatique

CalyxOS propose un installateur web simplifié qui automatise l'ensemble du processus :

**Téléchargement** : Sur calyxos.org/get, téléchargez device-flasher et l'image CalyxOS.

**Installation automatique** : Branchez le téléphone via USB, lancez device-flasher qui détecte l'appareil et guide le processus : déverrouillage bootloader, flash système, reverrouillage sécurisé pour Verified Boot.

### Points de vigilance

⚠️ **Ne jamais débrancher** le câble USB pendant l'installation sous peine de corrompre le système.

⚠️ **Vérifier avant le verrouillage** : Assurez-vous que CalyxOS démarre correctement avant de reverrouiller le bootloader. Un mauvais verrouillage peut rendre l'appareil inutilisable.

⚠️ **Patience au premier démarrage** : Le premier lancement peut prendre plusieurs minutes pour optimiser les applications. C'est normal.

## Configuration initiale

### Assistant de démarrage

Au premier allumage, CalyxOS vous guide à travers une configuration simplifiée :

L'assistant configure la langue, Wi-Fi, verrouillage d'écran et propose d'activer microG (recommandé pour la compatibilité) ainsi que les applications FOSS pré-sélectionnées.

### Configuration post-installation

**Mises à jour système** : Rendez-vous immédiatement dans Paramètres > Système > Mise à jour du système pour appliquer les derniers correctifs de sécurité disponibles.

**Vérification microG** : Ouvrez l'application microG Settings pour vérifier l'activation des services essentiels : Service Core, détection d'emplacement, et réception des notifications push.

**F-Droid et Aurora Store** : Lancez F-Droid pour synchroniser le catalogue d'applications libres, et configurez Aurora Store en mode anonyme pour accéder aux applications propriétaires si nécessaire.

## Utilisation quotidienne

### Navigation et communication

CalyxOS transforme votre expérience mobile en privilégiant la confidentialité sans sacrifier la fonctionnalité :

**Navigation** : DuckDuckGo (anti-traqueurs) et Tor Browser (anonymat complet).

**Communication** : Signal (chiffrée de bout en bout), K-9 Mail (PGP support).

**Cartographie** : Organic Maps (OpenStreetMap hors-ligne), Transportr (transports en commun).

### Gestion des applications

Le système de double boutique facilite la gestion de vos applications :

F-Droid met à jour automatiquement les apps open source en arrière-plan. Aurora Store nécessite des vérifications manuelles pour les apps propriétaires. Hypatia analyse les nouvelles installations.

## Avantages et limitations

### Points forts

**Protection de la vie privée par défaut** : Aucune donnée personnelle n'est transmise à Google ou aux GAFAM. Tous les réglages privilégient la confidentialité sans configuration manuelle.

**Expérience utilisateur préservée** : Interface familière d'Android, performances fluides, compatibilité applicative élevée grâce à microG. La transition depuis Android stock s'effectue sans difficulté majeure.

**Écosystème cohérent** : Applications pré-installées soigneusement sélectionnées, magasins d'applications complémentaires, mises à jour automatiques. Tout fonctionne "out of the box".

**Support communautaire** : Documentation complète, communauté active, organisation à but non lucratif garantissant la pérennité du projet.

### Contraintes à considérer

**Compatibilité matérielle limitée** : Support officiel restreint principalement aux Google Pixel. Impossible d'installer sur la majorité des smartphones Android.

**Services Google manquants** : Google Pay, Android Auto, Assistant Google et Chromecast ne fonctionnent pas. Certaines applications bancaires très strictes peuvent refuser de fonctionner.

**Mode privé permanent** : Impossibilité de rester connecté aux comptes web d'une session à l'autre. Vous devez vous reconnecter à chaque utilisation pour une sécurité maximale.

## Bonnes pratiques

### Optimisation de la confidentialité

**Contrôle réseau** : Datura Firewall limite les accès de chaque application.

**Permissions granulaires** : Révisez régulièrement les autorisations (localisation, caméra, microphone).

**Apps FOSS prioritaires** : NewPipe (YouTube), AntennaPod (podcasts), Simple Notes.

### Sécurité opérationnelle

**Sauvegardes** : Codes 2FA séparés du téléphone, SeedVault vers Nextcloud.

**Mises à jour** : Appliquez rapidement les correctifs système.

**Migration progressive** : Installation parallèle → migration par catégorie → validation → basculement définitif.

## CalyxOS vs GrapheneOS : Quelle différence ?

CalyxOS et GrapheneOS adoptent deux philosophies distinctes :

**CalyxOS** privilégie l'**équilibre confidentialité/utilisabilité** avec Android dégooglisé accessible, expérience proche du standard.

**GrapheneOS** vise la **sécurité absolue** pour utilisateurs à haut risque (journalistes, activistes) acceptant la complexité.

### Différences techniques majeures

| Aspect | CalyxOS | GrapheneOS |
|--------|---------|------------|
| **Services Google** | microG intégré par défaut | Aucun service Google/microG |
| **Compatibilité apps** | Très élevée (90%+ des apps) | Limitée (70% sans services Google) |
| **Durcissement système** | Standard Android + améliorations | Durcissement extrême (50+ modifications) |
| **Notifications push** | Fonctionnelles via microG | Problématiques sans Google Play Services |
| **Configuration initiale** | Assistée avec apps pré-installées | Manuelle, système minimal |
| **Mises à jour** | Automatiques OTA | Automatiques OTA |
| **Support matériel** | Pixel + Fairphone + Motorola | Pixel uniquement |

### Écosystème et sécurité

**CalyxOS** : Système complet dès l'installation avec apps pré-intégrées. Sécurité Android standard + améliorations (Verified Boot, DNS sécurisé).

**GrapheneOS** : Système minimal à configurer manuellement. Plus de 50 modifications de sécurité au niveau noyau pour protection maximale contre attaques sophistiquées.

### Public cible et cas d'usage

### Recommandation

Compte tenu de la situation actuelle (pause de développement depuis août 2025), **GrapheneOS devient l'option recommandée** pour la majorité des utilisateurs recherchant un Android sécurisé et dégooglisé.

**GrapheneOS** offre un développement actif, des mises à jour régulières et une sécurité de premier plan, bien qu'avec une courbe d'apprentissage plus prononcée.

En attendant la reprise de CalyxOS, GrapheneOS constitue la meilleure alternative pour maintenir sa confidentialité mobile.

## Conclusion

CalyxOS représente une solution mature et équilibrée pour reprendre le contrôle de sa vie privée numérique sans renoncer au confort d'utilisation d'Android. En proposant un système d'exploitation dégooglisé, sécurisé et accessible, le Calyx Institute offre une alternative crédible aux utilisateurs soucieux de confidentialité.

La philosophie "privacy by default" de CalyxOS, combinée à son écosystème d'applications FOSS pré-intégrées et à sa compatibilité préservée via microG, en fait un choix judicieux pour quiconque souhaite échapper à la surveillance commerciale sans sacrifier la praticité quotidienne.

Face à GrapheneOS qui vise la sécurité absolue au prix de concessions d'usage, CalyxOS démontre qu'il est possible de concilier protection des données et ergonomie moderne. Pour les possesseurs de smartphones compatibles, cette distribution Android alternative constitue un pas décisif vers une souveraineté numérique retrouvée.

## Ressources

### Documentation officielle
- [Site officiel CalyxOS](https://calyxos.org) - Présentation et téléchargements
- [Guide d'installation](https://calyxos.org/get) - Instructions par modèle d'appareil  
- [Documentation complète](https://calyxos.org/docs) - FAQ et guides d'utilisation
- [Comparatif avec GrapheneOS](https://calyxos.org/docs/faq/#grapheneos) - Différences techniques

### Communauté
- [Matrix](https://matrix.to/#/#calyxos:matrix.org) - Chat communautaire officiel
- [Reddit r/CalyxOS](https://reddit.com/r/CalyxOS) - Discussions et entraide
- [Mastodon](https://fosstodon.org/@calyxinstitute) - Actualités du projet
