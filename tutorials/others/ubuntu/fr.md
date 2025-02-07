---
name: Ubuntu
description: Guide complet pour installer et utiliser Ubuntu comme alternative à Windows
---

![cover](assets/cover.webp)

## Introduction

Un système d'exploitation (OS) est le logiciel principal qui gère l'ensemble des ressources de votre ordinateur. Le choix d'un système d'exploitation alternatif comme Ubuntu peut offrir de nombreux avantages en termes de sécurité, de coût et de respect de la vie privée.

### Pourquoi Ubuntu ?

- **Sécurité accrue** : Les distributions Linux sont réputées pour leur sécurité et robustesse
- **Coût nul** : Ubuntu et la majorité des distributions Linux sont gratuits
- **Large communauté** : Une communauté d'utilisateurs prête à aider via forums et tutoriels
- **Respect de la vie privée** : Système open source offrant une meilleure transparence
- **Simplicité** : Interface conviviale et facilité d'utilisation
- **Écosystème riche** : Large catalogue de logiciels open source
- **Support régulier** : Mises à jour sécurisées par Canonical

## Installation et Configuration

### 1. Prérequis

**Matériel nécessaire :**
- Une clé USB d'au moins 12 Go
- Un ordinateur fonctionnant sous Windows avec au moins 25 Go de disponible

### 2. Téléchargement

- Rendez-vous sur [ubuntu.com/download](https://ubuntu.com/download)
- Choisissez la version stable (LTS recommandée)
- Téléchargez l'image ISO

![Page de téléchargement Ubuntu](fr/01.webp)
![Sélection de la version Ubuntu](fr/02.webp)

### 3. Créer une clé USB bootable

**3.1 Graver l'image ISO sur la clé USB**
Vous pouvez utiliser plusieurs outils, par exemple Balena Etcher :

- Télécharger [Balena Etcher](https://etcher.balena.io/) et l'installer
![Page de téléchargement Balena Etcher](fr/03.webp)
![Installation de Balena Etcher](fr/04.webp)

- Ouvrir Balena Etcher, puis sélectionner l'image ISO d'Ubuntu
- Sélectionner la clé USB comme support de destination
- Cliquer sur Flash et attendre la fin du processus
![Utilisation de Balena Etcher](fr/05.webp)

### 4. Installer et sécuriser Ubuntu

**4.1 Démarrage sur la clé USB**
- Éteignez l'ordinateur
- Branchez la clé USB (contenant Ubuntu)
- Allumez l'ordinateur. Sur les PC récents, le système devrait reconnaître automatiquement la clé USB de démarrage. Si ce n'est pas le cas, redémarrez en maintenant la touche d'accès au BIOS/UEFI (généralement F2, F12, ou Delete, selon la marque)
	- Dans le menu du BIOS/UEFI, sélectionnez votre clé USB comme périphérique de démarrage (Boot)
	- Sauvegardez (Save) et redémarrez

**4.2 Lancement de l'installation**
Sur l'écran d'accueil :
- Choisissez votre langue
- Sélectionnez vos paramètres d'accessibilité si nécessaire
- Choisissez votre disposition de clavier
- Connectez-vous à votre réseau (recommandé pour télécharger les mises à jour pendant l'installation)
- Choisissez entre "Essayer Ubuntu" ou "Installer Ubuntu"

**4.3 Mettre à jour Ubuntu après l'installation**

La mise à jour du système est une étape importante après une nouvelle installation. Vous avez deux options :

**Option 1 : Via l'interface graphique**
- Recherchez "Logiciels et mises à jour" dans le menu des applications
- L'application vérifiera automatiquement les mises à jour disponibles
- Suivez les instructions à l'écran pour installer les mises à jour

**Option 2 : Via le Terminal**
- Ouvrez le Terminal (Ctrl + Alt + T)
- Tapez la commande suivante pour vérifier les mises à jour disponibles :
  ```bash
  sudo apt update
  ```
- Entrez votre mot de passe lorsque demandé
- Pour installer les mises à jour, tapez :
  ```bash
  sudo apt upgrade
  ```
- Confirmez l'installation en tapant 'Y' puis Entrée

### 5. Découvrir les tâches de base

**5.1 Naviguer sur Internet**
Par défaut, vous trouverez souvent Firefox dans la barre de lancement.
Lancez Firefox et commencez à naviguer.
D'autres navigateurs (Chrome, Brave, etc.) sont installables via le Gestionnaire de logiciels ou via des paquets .deb.

**5.2 Faire du traitement de texte**
Ubuntu est fourni avec la suite LibreOffice (Writer pour le traitement de texte).
Pour l'ouvrir : Activités > Rechercher "LibreOffice Writer" ou cliquer sur l'icône si elle apparaît dans la barre.
Vous pouvez créer, modifier et enregistrer des documents dans divers formats (y compris .docx).

**5.3 Installer des applications**
Gestionnaire de logiciels (appelé "Ubuntu Software") : interface graphique pour rechercher et installer des applications.
Depuis le Terminal, utilisez la commande :
```bash
sudo apt install nom-du-paquet
```
Exemple :
```bash
sudo apt install vlc
```

### 6. Conclusion et ressources complémentaires

Vous voilà prêt à utiliser Ubuntu au quotidien : sécuriser votre système, naviguer, faire de la bureautique, installer des logiciels et maintenir votre OS à jour !