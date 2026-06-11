---
layout: home
nav_order: 1
title: Accueil
permalink: /
---

# Bienvenue sur notre documentation

Bienvenue dans la documentation du projet Otoo. Ce site a pour but de fournir toutes les informations nécessaires pour comprendre, utiliser et reproduire efficacement notre projet.

[Notre projet sur Onshape](https://cad.onshape.com/documents/c6ec4971b6b5d4da3d8c69bf/w/2707927c11ab40a765c09b32/e/18c3610bb8b025732a03c396){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[Notre repo GitHub](https://github.com/Makerspace-Amiens/template-project){: .btn .fs-5 .mb-4 .mb-md-0 }

### 🤖 Notre Modèle 3D (OnShape)
[![Cliquez ici pour interagir avec le modèle 3D](https://raw.githubusercontent.com/Makerspace-Amiens-2025-26/Otto-Groupe15/main/docs/images/otto_preview.png)](https://cad.onshape.com/documents/c6ec4971b6b5d4da3d8c69bf/w/2707927c11ab40a765c09b32/e/18c3610bb8b025732a03c396)
*Cliquez sur l'image ci-dessus pour ouvrir et manipuler notre robot en 3D directement sur OnShape.*

## 📝 Introduction
Dans le cadre d'un projet de première année au MakerSpace d'**UniLaSalle Amiens**, nous avons assemblé, programmé et personnalisé un robot humanoïde **Otto-MKS**. 

Ce projet s'inscrit dans le cadre des **Ottolympiades**, un tournoi de fin d'année par groupe de 2 visant à tester les capacités de nos robots à travers plusieurs épreuves compétitives. Le but de ce projet est de s'initier aux bases de la robotique et de la modélisation 3D, tout en faisant preuve de créativité et d'innovation.

Le but de ce projet est de s'initier aux bases de la robotique, de la modélisation 3D tout en faisant preuve de créativité et d'innovation.

### 🔌 Pièces et Composants fournis
Pour mener à bien la construction de l'Otto-MKS, le kit de base suivant est utilisé :

* **Carte électronique Otto-MKS :** Conçue sur mesure au MakerSpace, elle intègre un microcontrôleur ESP32, une LED, un interrupteur, des sorties pour servomoteurs, ainsi qu'un connecteur pour capteur ultrason et d'autres composants additionnels (gyroscope, écran, etc.).
* **4 × Servomoteurs :** Permettent de gérer les mouvements des jambes et des pieds pour la marche.
* **Capteur ultrason (HC-SR04) :** Permet au robot de détecter son environnement (présence, distance, obstacles).
* **Batterie 9V rechargeable :** Batterie rechargeable en USB-C aux dimensions d'une pile 9V standard pour simplifier l'alimentation.
* **Composants imprimés en 3D :** La structure corporelle (Tête, Corps, Jambes, Pieds) modélisée et modifiée sur le logiciel **OnShape**.

---

## 🛠️ Instructions de Fabrication

1. **Préparation et Inventaire :** Rassembler l'ensemble des pièces électroniques fournies par le MakerSpace et vérifier le bon fonctionnement des moteurs.
2. **Modélisation et Impression 3D :** Utiliser les fichiers de base du robot Otto sur OnShape. Effectuer les modifications esthétiques ou mécaniques souhaitées (ajout de bras, de supports de capteurs, etc.) avant de lancer l'impression 3D en PLA.
3. **Assemblage Mécanique :** * Fixer les servomoteurs dans le châssis inférieur pour les jambes et les pieds.
   * Assembler les membres imprimés en veillant au bon alignement des axes des moteurs.
4. **Montage Électronique :** Intégrer la carte électronique Otto-MKS (ESP32) dans la tête du robot, connecter le capteur ultrason sur la face avant et brancher les 4 servomoteurs sur les ports dédiés.
5. **Programmation et Connexion :** Programmer le microcontrôleur via l'IDE Arduino ou une interface visuelle pour configurer la marche, l'évitement d'obstacles et la liaison WiFi/Bluetooth.

---

## 💻 Programmation et Contrôle Bluetooth
Pour rendre le robot fonctionnel lors des épreuves des Ottolympiades, un code sur mesure a été développé avec l'IDE Arduino. Il gère le pilotage sans fil et le comportement des moteurs.

### 📲 Configuration du contrôle sans fil (RemoteXY)
Le programme s'appuie sur la bibliothèque **RemoteXY** connectée en Bluetooth BLE via l'ESP32.

* **Identifiant Bluetooth :** `lamano otto`
* **Sécurité :** L'accès est protégé par le mot de passe requis `lylianolamano`.
* **Interface :** L'application mobile transmet les coordonnées de deux joysticks virtuels lues en continu par la structure `RemoteXY`.

### ⚙️ Logique des Mouvements et Actions
La boucle principale (`void loop()`) analyse la position des joysticks pour exécuter les routines associées :
* **Joystick 1 (Navigation) :** Déclenche la marche avant, arrière ou les rotations en modifiant l'amplitude des servomoteurs principaux.

---

## 🏁 Conclusion
Ce projet d'ingénierie de première année au MakerSpace d'UniLaSalle Amiens a permis de concrétiser l'assemblage, la personnalisation 3D sur OnShape et la programmation complète du robot humanoïde **lamano otto**. Grâce à l'intégration du système de contrôle sans fil, le robot a été prêt à concourir de manière optimale lors des épreuves des Ottolympiades.



## Vidéo
Pour voir le robot en action et découvrir une présentation professionel (pas trop..) de notre projet, vous pouvez visionner notre vidéo ci dessous.
Si la vidéo ne se lance pas, veuillez copier ce lien : https://youtube.com/shorts/0be9pnPoyPI?feature=shared

<p align="center">
  <video src="https://github.com/user-attachments/assets/1c668326-d1f5-41e1-ac38-be07f81b9f73" width="700" controls></video>
</p>

<video src="images/intro_amiens.mp4" controls title="Title"  style="width: 100%;"></video>

---
