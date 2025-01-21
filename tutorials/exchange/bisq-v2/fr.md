---
name: Bisq 2
description: Guide complet pour utiliser Bisq 2 et échanger des bitcoins en P2P
---

![cover](assets/cover.webp)

## Introduction

Les échanges de pair-à-pair (P2P) sans KYC sont essentiels pour préserver la confidentialité et l'autonomie financière des utilisateurs. Ils permettent des transactions directes entre individus sans nécessiter de vérification d'identité, ce qui est crucial pour ceux qui valorisent la vie privée. Pour une compréhension plus approfondie des concepts théoriques, consultez le cours BTC204 :

https://planb.network/courses/btc204

### Qu'est-ce que Bisq 2 ?

Bisq 2 est la nouvelle version du célèbre échange décentralisé Bisq, lancée en 2024. Contrairement à sa version précédente, Bisq 2 a été développé pour supporter plusieurs protocoles d'échange, offrant ainsi plus de flexibilité aux utilisateurs.

**Nouvelles fonctionnalités clés :**
- Support de plusieurs réseaux de confidentialité (Tor, I2P)
- Possibilité de créer plusieurs identités pour une meilleure confidentialité
- Interface REST API pour les bots de trading
- Support de plusieurs types de portefeuilles
- Système de rôles avec caution obligatoire en BSQ

Ce guide se concentre exclusivement sur "Bisq Easy", le seul protocole actuellement disponible. Bisq Easy a été conçu spécialement pour les nouveaux utilisateurs de Bitcoin. Ce protocole permet aux utilisateurs d'acheter et de vendre des bitcoins contre des devises fiduciaires sur une plateforme décentralisée de pair à pair. Les transactions sont limitées à l'équivalent de 600 USD (avec un minimum de 6 USD), et la sécurité des échanges repose sur la réputation des vendeurs de BTC. Bisq Easy ne comporte ni frais de trading ni exigence de dépôt de garantie. Il est prévu que Bisq Easy remplace Bisq 1 pour les échanges en monnaie fiduciaire inférieurs à 600 USD (ou équivalent).

**Caractéristiques principales :**
- Application de bureau multi-plateforme
- Plusieurs protocoles d'échange disponibles
- Réseau P2P décentralisé
- Focus sur la confidentialité (pas de KYC, utilisation de Tor)
- Non-custodial (vous gardez le contrôle de vos fonds)
- Open source (AGPL)

### Différences avec Bisq 1

**Pour les acheteurs :**
- Pas de dépôt de garantie requis
- Pas de frais de trading
- Pas de frais miniers
- Sécurité basée sur la réputation des vendeurs
- Limites de trading plus basses (équivalent à 600 USD)

**Pour les vendeurs :**
- Pas de dépôt de garantie requis
- Construction d'une réputation nécessaire
- Possibilité de brûler des BSQ ou de créer des obligations BSQ
- Prime de vente potentiellement plus élevée (10-15% au-dessus du marché)

**Note importante :** Une fois que le protocole Bisq Multisig sera implémenté dans Bisq 2, l'ancienne version de Bisq pourra être progressivement abandonnée. Bisq 1 continuera cependant d'être utilisé comme outil de gestion du DAO Bisq et pour les échanges BSQ-BTC.

### Processus d'échange

- Le créateur de l'offre définit les termes de l'échange
- Une fois que les traders se sont mis d'accord sur les conditions (méthode de paiement et prix), l'échange commence
- Le vendeur transmet ses coordonnées bancaires à l'acheteur, et l'acheteur envoie son adresse Bitcoin au vendeur
- L'acheteur effectue le paiement en monnaie fiduciaire et notifie le vendeur
- Une fois le paiement reçu, le vendeur envoie les bitcoins à l'adresse de l'acheteur
- L'échange est terminé lorsque l'acheteur reçoit les bitcoins

### Règles importantes

- Avant l'échange des détails de paiement, l'échange peut être annulé sans justification
- Après l'échange des détails, ne pas respecter ses obligations peut entraîner un bannissement
- Pour les virements, ne JAMAIS utiliser les termes "Bisq" ou "Bitcoin" dans le motif du paiement
- Les traders doivent se connecter au moins une fois par jour pour suivre le processus
- En cas de problème, les traders peuvent faire appel à un médiateur

## Installation et Configuration

### 1. Télécharger et Vérifier Bisq 2

![Téléchargement de Bisq 2](assets/fr/01.webp)

- Rendez-vous sur [bisq.network](https://bisq.network/downloads/)
- Téléchargez la version Bisq 2 correspondant à votre système d'exploitation (faire défiler la page vers le bas)
- Vérifiez l'authenticité du fichier téléchargé (fortement recommandé). Pour un guide détaillé sur la vérification des signatures, consultez le tutoriel suivant : 

https://planb.network/tutorials/others/general/integrity-authenticity-21d0420a-be02-4663-94a3-8d487f23becc

### 2. Installation selon votre système

Veuillez suivre les étapes d'installation appropriées pour votre système d'exploitation. En cas de difficulté lors de l'installation, vous pouvez consulter le guide détaillé sur le [wiki officiel de Bisq](https://bisq.wiki/Downloading_and_installing).

### 3. Premier Démarrage

![Configuration initiale](assets/fr/02.webp)

image 01 et 02 et 03

- Lancez Bisq 2
- Choisissez si vous souhaitez partager des données d'utilisation
- Créez un nouveau profil en choisissant un nom ainsi qu'un avatar

### 4. Configuration des Méthodes de Paiement

![Configuration des paiements](assets/fr/03.webp)
image 03 et 04

La configuration préalable des méthodes de paiement est optionnelle, mais recommandée pour gagner du temps lors des échanges. Vous pouvez également configurer vos méthodes de paiement directement pendant un trade en communiquant avec votre partenaire d'échange.

Si vous souhaitez les configurer à l'avance :
- Accédez aux paramètres
- Sélectionnez "Payment Accounts"
- Ajoutez vos méthodes de paiement préférées :
  - SEPA (virements européens)
  - Revolut
  - Wise
  - PayPal
  - Et bien d'autres...

### 5. Sécurisation du Compte

![Sécurisation du compte](assets/fr/04.webp)

**Sauvegarde des données :**
- Contrairement à Bisq 1, Bisq 2 n'intègre pas de portefeuille Bitcoin pour l'instant : les transactions se font donc via vos propres portefeuilles externes
- Il est néanmoins recommandé de sauvegarder régulièrement votre dossier de données Bisq 2
- Pour localiser votre dossier de données, consultez le [wiki officiel de Bisq](https://bisq.wiki/Backing_up_application_data#Back_up_the_entire_Bisq_data_directory)

**Gestion des identités :**
- Bisq 2 permet de créer plusieurs identités
- Chaque identité peut être utilisée pour différents types de transactions
- Vos identités sont stockées dans le dossier de données

## Acheter et Vendre des Bitcoins

### Comment Acheter des Bitcoins

![Processus d'achat](assets/fr/05.webp)

**Option 1 : Prendre une offre existante**
- Sur l'écran principal, sélectionnez "Bisq Easy" puis "Getting started"
- Cliquez sur "Start trade wizard"
- Choisissez "Buy Bitcoin" et sélectionnez votre devise
- Configurez vos méthodes de paiement préférées (SEPA, Revolut, etc.)
- Définissez le montant (entre 6 et 600 USD équivalent)
- Sélectionnez une offre dans la liste (privilégiez les vendeurs avec une réputation élevée)
- Vérifiez les détails et confirmez le trade

**Option 2 : Créer votre propre offre**
- Sélectionnez "Bisq Easy" puis "Offerbook"
- Choisissez votre paire de trading (ex: BTC/EUR)
- Cliquez sur "Create offer"
- Suivez l'assistant de création d'offre :
  - Sélectionnez les méthodes de paiement acceptées
  - Définissez le montant (fixe ou plage)
  - Vérifiez le récapitulatif et publiez l'offre

![Finalisation de l'achat](assets/fr/06.webp)

Une fois l'échange initié :
- Recevez les coordonnées bancaires du vendeur
- Envoyez votre adresse Bitcoin au vendeur
- Effectuez le paiement (sans mentionner "Bisq" ou "Bitcoin")
- Notifiez le vendeur du paiement effectué
- Attendez la réception des bitcoins

### Comment Vendre des Bitcoins

![Création d'une offre de vente](assets/fr/07.webp)

**Option 1 : Créer une offre de vente**
- Sélectionnez "Bisq Easy" puis "Offerbook"
- Cliquez sur "Create offer" et choisissez "Sell Bitcoin"
- Configurez votre offre :
  - Sélectionnez la devise (EUR, USD, etc.)
  - Choisissez les méthodes de paiement acceptées
  - Définissez le montant (entre 6 et 600 USD équivalent)
  - Fixez votre prix (fixe ou % par rapport au marché)
- Vérifiez les détails et publiez l'offre

**Option 2 : Prendre une offre d'achat existante**
- Parcourez les offres d'achat dans l'onglet "Offerbook"
- Filtrez par devise et méthode de paiement
- Sélectionnez une offre qui vous convient
- Vérifiez les détails et acceptez l'offre

![Gestion des ventes](assets/fr/08.webp)

**Processus de vente :**
1. Une fois l'échange initié :
   - Envoyez vos coordonnées bancaires à l'acheteur
   - Attendez l'adresse Bitcoin de l'acheteur
   - Vérifiez que l'adresse est valide

2. Après notification du paiement :
   - Vérifiez la réception du paiement sur votre compte
   - Confirmez que le montant et les détails correspondent
   - Envoyez les bitcoins à l'adresse fournie
   - Marquez la transaction comme complétée

3. Finalisation :
   - Attendez la confirmation de l'acheteur
   - Laissez un feedback sur la transaction
   - Construisez votre réputation pour les futures ventes

**Note importante :** En tant que vendeur, vous devez être particulièrement vigilant concernant les risques de rétrofacturation. Privilégiez les méthodes de paiement sécurisées et vérifiez toujours que le paiement est bien reçu avant d'envoyer les bitcoins.

## Bonnes Pratiques et Sécurité

### Conseils de Sécurité

**Pour les acheteurs :**
- Commencez par de petits montants
- Vérifiez la réputation des vendeurs (score minimum de 30 000)
- Utilisez uniquement les méthodes de paiement suggérées
- Vérifiez que le vendeur est actif avant d'envoyer le paiement
- Utilisez uniquement les coordonnées bancaires fournies dans le chat de l'échange
- Ne communiquez jamais en dehors de la plateforme Bisq 2
- Conservez les preuves de paiement
- N'envoyez jamais d'informations sensibles

**Pour les vendeurs :**
- Soyez vigilant avec les nouveaux comptes
- Évitez les méthodes de paiement sensibles aux rétrofacturations (PayPal, Venmo)
- Vérifiez que les détails du compte correspondent à l'acheteur
- Limitez la communication au chat Bisq 2
- Ouvrez une médiation en cas de doute

### Construction de la Réputation (pour les vendeurs)

- Effectuez des transactions régulières
- Maintenez une communication professionnelle
- Envisagez de créer une obligation BSQ
- Répondez rapidement aux acheteurs

### Résolution des Litiges

- Contactez votre contrepartie via le chat
- Si nécessaire, ouvrez un litige
- Fournissez toutes les preuves demandées
- Suivez les instructions du médiateur

### Protection de la vie privée :
- Aucune inscription ou vérification d'identité centralisée requise
- Toutes les connexions passent par le réseau Tor (et bientôt I2P)
- Aucun serveur central ne stocke les données
- Les détails des transactions sont uniquement lisibles par les parties concernées

### Protection contre la censure :
- Réseau P2P entièrement distribué
- Utilisation du réseau Tor (et bientôt I2P) pour la résistance à la censure
- Projet open source géré par une DAO, sans entité légale centralisée

## Avantages et Inconvénients

### Avantages de Bisq 2

- **Confidentialité maximale** : Pas de KYC, utilisation de Tor
- **Décentralisation** : Pas de serveur central
- **Sécurité** : Code open source, non-custodial
- **Interface intuitive** : Plus simple que Bisq 1
- **Flexibilité** : Multiple protocoles d'échange

### Inconvénients de Bisq 2

- **Liquidité limitée** : Nouveau protocole en phase de démarrage
- **Limites de trading** : Maximum de 600 USD par transaction (Bisq easy)
- **Desktop uniquement** : Pas d'application mobile


## Futurs Protocoles

Bien que Bisq Easy soit actuellement le seul protocole disponible, plusieurs autres protocoles sont en développement pour Bisq 2 :

### Protocoles d'Échange Prévus

- **Bisq Lightning** : Protocole d'échange basé sur un système d'entiercement utilisant la cryptographie à calcul multipartite sur le réseau Lightning.

- **Bisq MuSig** : Migration du protocole principal de Bisq 1 vers Bisq 2, utilisant un multisig 2-sur-2 avec dépôts de garantie.

- **BSQ Swaps** : Échanges atomiques instantanés entre BSQ et BTC.

- **Liquid Swaps** : Échange d'actifs sur le réseau Liquid (USDT, BTC-L) via des swaps atomiques.

- **Monero Swaps** : Échanges atomiques entre Bitcoin et Monero.

- **Liquid MuSig** : Version du protocole multisig utilisant L-BTC pour des frais réduits et une meilleure confidentialité.

- **Submarine Swaps** : Échanges entre Bitcoin sur le réseau Lightning et Bitcoin on-chain.

- **Stablecoin Swaps** : Échanges atomiques entre Bitcoin et stablecoins USD.

- **Options Multisig** : Création d'options put et call P2P avec blocage de BTC dans une transaction multisig on-chain.

- **Contrats Ouverts Multisig** : Permet la création de contrats conditionnels personnalisés utilisant un système multisig 2-sur-3 avec arbitrage.

Ces protocoles sont en cours de développement et seront progressivement intégrés à Bisq 2, offrant ainsi une plus grande flexibilité aux utilisateurs selon leurs besoins spécifiques.

## Ressources Utiles

- Site officiel : [bisq.network](https://bisq.network)
- Documentation : [Bisq Wiki](https://bisq.wiki)
- Support : [Forum Bisq](https://bisq.community)
- Code source : [GitHub](https://github.com/bisq-network)
