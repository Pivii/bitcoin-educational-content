---
name: Peach
description: Guide complet pour utiliser Peach et échanger des bitcoins en P2P
---

![cover](assets/cover.webp)

# Introduction

Les échanges de pair-à-pair (P2P) sans KYC sont essentiels pour préserver la confidentialité et l'autonomie financière des utilisateurs. Ils permettent des transactions directes entre individus sans nécessiter de vérification d'identité, ce qui est crucial pour ceux qui valorisent la vie privée. Pour une compréhension plus approfondie des concepts théoriques, consultez le cours BTC204 :

https://planb.network/courses/btc204

## Qu'est-ce que Peach ?

Peach est une plateforme d'échange P2P qui permet aux utilisateurs d'acheter et de vendre des bitcoins sans KYC. Elle offre une interface intuitive et des fonctionnalités de sécurité avancées. Comparée à d'autres solutions comme Bisq, HodlHodl, et Robosat, Peach se distingue par sa simplicité d'utilisation et ses frais réduits.

### Avantages de Peach :

- **Pas de KYC requis** : Préserve la confidentialité des utilisateurs.
- **Aucun accès aux données bancaires** : Peach n'a pas accès à vos informations bancaires ni à votre identité.
- **Interface intuitive** : Facile à utiliser pour les utilisateurs intermédiaires.
- **Open Source** : Le code source est public et vérifiable par la communauté.

### Inconvénients de Peach :

- **Liquidité limitée** : Moins de volume d'échange comparé à des plateformes plus établies.
- **Risque réglementaire** : L'application est gérée par une entreprise suisse et est donc soumise à la réglementation suisse qui pourrait évoluer et potentiellement censurer l'application.

## Confidentialité et Données Collectées

### Quelles informations Peach collecte-t-elle ?

Peach s'efforce de stocker le minimum absolu de données sur ses utilisateurs. Voici un aperçu des données conservées sur ses serveurs :

- Un hash de votre identifiant unique d'application (AdID)
- Un hash de vos données de paiement
- Vos conversations chiffrées
- Les données des transactions pour s'assurer que les utilisateurs anonymes ne dépassent pas la limite de trading (types de méthodes de paiement utilisées, montants d'achat et de vente)
- Les adresses utilisées pour envoyer et recevoir depuis le compte séquestre
- Données d'utilisation (Firebase & Google Analytics), uniquement si vous y avez consenti

Pour rappel un hash est une donnée rendue méconnaissable, similaire à un chiffrement. Les mêmes données produiront toujours le même hash, permettant de détecter les doublons sans connaître les données d'origine.

*Pour plus d'explication sur le hachage, vous pouvez consulter cet ebook rédigé par Loïc Morel :

[Bitcoin et la cryptographie](https://www.pandul.fr/_files/ugd/23ab18_7cf468f563804bf586d8ade77cb5ab96.pdf)

*Ou bien suivre sur ce cours : 

https://planb.network/fr/courses/cyp201



### Qui peut voir mes détails de paiement ?

- Seule votre contrepartie peut voir vos détails de paiement
- Les données sont transmises via les serveurs Peach mais sont entièrement chiffrées de bout en bout
- En cas de litige, vos détails de paiement et l'historique des conversations seront visibles par le médiateur Peach assigné

# Installation et Configuration

## 1. Installer l'application Peach

![Installation de Peach](assets/fr/01.webp)

1. Téléchargez l'application depuis [Peach Bitcoin](https://peachbitcoin.com/fr/quick-start/).
2. Suivez les instructions d'installation sur votre appareil.
3. Lors de l'installation, vous serez invité à choisir si vous souhaitez partager certaines données pour améliorer l'application Peach. (Mockup 1)
4. Sur l'écran suivant (Mockup 2), vous aurez deux options : 
   - Si vous êtes un nouvel utilisateur, cliquez sur "New user" pour créer un nouveau profil
   - Si vous avez déjà un compte, utilisez "Restore" pour restaurer votre profil existant
5. Si vous avez un code de parrainage, vous pouvez l'entrer à ce moment-là.
6. Pour la restauration d'un compte existant (Mockup 3), vous aurez besoin : 
   - De votre fichier de sauvegarde (backup)
   - Du mot de passe permettant de déchiffrer ce fichier

## 2. Comment sécuriser son portefeuille

### Comprendre votre compte Peach

Un compte Peach n'est pas un compte traditionnel avec identifiant et mot de passe. C'est un fichier stocké localement sur votre téléphone, ce qui signifie que Peach n'a pas besoin de stocker vos données ni de connaître votre identité : vous gardez le contrôle. Ce fichier contient toutes vos données, des clés de votre portefeuille bitcoin à vos détails de paiement.

Cette approche garantit une meilleure confidentialité mais implique aussi plus de responsabilité. La perte de votre téléphone sans sauvegarde signifie la perte d'accès à votre compte Peach et à vos fonds. Il est donc crucial de sauvegarder ce fichier et de le protéger avec un mot de passe robuste.

### Créer vos sauvegardes

![Accéder aux sauvegardes](assets/fr/02.webp)

1. Accédez aux paramètres depuis l'onglet en bas à droite de l'écran d'accueil (Mockup 4)
2. Sélectionnez l'option "backups" dans le menu des paramètres (Mockup 5)

![Processus de sauvegarde](assets/fr/03.webp)

3. Deux types de sauvegardes sont disponibles :

#### Sauvegarde du fichier de compte (Mockup 6)
- Cliquez sur "Create new backup"
- Créez un mot de passe fort pour chiffrer votre fichier de sauvegarde
- Conservez ce fichier dans un endroit sûr

#### Sauvegarde de la phrase de récupération (Mockup 7)
- Suivez les instructions pour afficher votre phrase de récupération
- Notez soigneusement les mots dans l'ordre exact
- Stockez cette sauvegarde dans un lieu sécurisé, idéalement différent de celui du fichier de compte

### Différences entre les deux types de sauvegardes

**La sauvegarde du fichier** permet de restaurer votre compte Peach complet, incluant :
- Votre portefeuille
- Vos méthodes de paiement
- L'historique des conversations
- Les données de paiement
- L'historique des transactions avec les détails des contreparties

**La phrase de récupération** permet uniquement de récupérer :
- L'accès à votre compte
- Vos fonds bitcoin

Vous perdrez :
- L'historique des conversations
- Les données de paiement
- Les informations des contreparties dans l'historique des transactions

Il est recommandé de réaliser les deux types de sauvegardes pour une sécurité optimale.

## 3. Configurer ses moyens de paiements

Pour maximiser vos opportunités d'échange sur Peach, il est important de configurer vos méthodes de paiement préférées. Voici comment procéder :

### Accéder aux méthodes de paiement

1. Ouvrez l'application Peach
2. Allez dans **Paramètres > Méthodes de paiement**
3. Choisissez entre paiement en ligne ou en espèces (rencontres)

### Types de méthodes de paiement disponibles

#### 1. Virements Bancaires
- SEPA (standard ou instantané)
- Remplissez vos coordonnées bancaires SEPA

#### 2. Portefeuilles en ligne
- Plusieurs options disponibles selon votre pays
- Suivez les instructions pour ajouter vos identifiants

#### 3. Cartes Cadeaux
- Amazon
- Steam
- Sélectionnez le pays d'émission de la carte

#### 4. Options Nationales
Systèmes de paiement spécifiques par pays :
- Satispay (Italie)
- MB Way (Portugal)
- Bizum (Espagne)
- Faster Payments (Royaume-Uni)

### Conseils d'utilisation

- Vous pouvez configurer plusieurs méthodes de paiement simultanément
- Plus vous ajoutez de méthodes, plus vous aurez accès à un large éventail d'offres
- Vérifiez bien l'exactitude de vos informations avant de les enregistrer
- Vous pouvez modifier ou supprimer vos méthodes de paiement à tout moment

> **Note de sécurité** : Vos informations de paiement sont chiffrées et ne sont partagées qu'avec votre partenaire d'échange lors d'une transaction.

# Acheter et Vendre des Bitcoins

## 1. Comment Acheter des Bitcoins

1. Parcourez les offres disponibles dans l'application.
2. Sélectionnez une offre et suivez les instructions pour effectuer l'achat.
3. Transférez vos bitcoins vers un portefeuille froid pour plus de sécurité.

## 2. Comment Vendre des Bitcoins

1. Créez une offre de vente dans l'application.
2. Attendez qu'un acheteur réponde à votre offre.
3. Suivez les instructions pour finaliser la vente.

# Ressources Utiles

- Vidéo explicative : [YouTube](https://youtu.be/ziwhv9KqVkM)
- Guide de démarrage rapide : [Peach Bitcoin](https://peachbitcoin.com/fr/quick-start/)
