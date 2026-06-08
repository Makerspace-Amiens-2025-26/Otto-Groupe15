---
title: Objectifs du projet
---

# 🎯 Objectifs du projet

## 📝 Introduction
Le projet Otto-MKS représente notre première immersion concrète dans le domaine de la robotique mobile et de l'ingénierie collaborative au sein d'UniLaSalle Amiens. Ce document détaille le cadre, les ambitions ainsi que les critères techniques requis pour la réussite de notre robot humanoïde.

---

## 🏛️ Contexte du Projet
Développé au cours de la première année universitaire, ce projet s'articule autour des **Ottolympiades**. Ce tournoi de fin d'année met en compétition des équipes de deux étudiants. 

L'enjeu est de concevoir un robot capable de s'adapter à plusieurs épreuves physiques et d'agilité. Ce défi nous pousse à lier la théorie vue en cours à la pratique en atelier (MakerSpace), en nous confrontant aux réalités de l'assemblage mécanique, du prototypage rapide et du développement informatique.

---

## 🚀 Objectifs du Projet
La réalisation de l'Otto-MKS poursuit plusieurs objectifs majeurs :

* **Apprentissage technique :** Maîtriser les bases de la programmation sur microcontrôleur (ESP32) avec l'IDE Arduino et comprendre la gestion des signaux (capteurs ultrason, servomoteurs).
* **Conception et Modélisation 3D :** Prendre en main le logiciel de CAO **OnShape** pour modifier la structure du robot d'origine, comprendre les contraintes de l'impression 3D (tolérances, orientation des pièces) et personnaliser l'esthétique du robot.
* **Esprit d'innovation :** Optimiser l'algorithme de déplacement et l'interface de contrôle pour maximiser les performances d'Otto lors des épreuves.
* **Gestion de projet :** Travailler efficacement en binôme, documenter rigoureusement notre avancée sur GitHub et respecter un cahier des charges strict.

---

## 🔍 Existant
Le projet s'appuie sur la communauté internationale *Otto DIY*, qui fournit des plans en open-source pour un robot marcheur basique. 

Le MakerSpace d'UniLaSalle Amiens a fait évoluer cet existant en créant une version customisée : **l'Otto-MKS**. La base matérielle fournie comprend une carte électronique propriétaire intégrant un puissant module **ESP32** (WiFi/Bluetooth) et des composants d'alimentation optimisés, remplaçant la classique carte Arduino Nano pour offrir beaucoup plus de flexibilité et de puissance de calcul.

---

## 📋 Cahier des Charges
Pour participer aux Ottolympiades, notre robot doit impérativement respecter les exigences suivantes :

### 1. Contraintes Mécaniques et Design
* **Structure :** Le robot doit être entièrement assemblé avec les pièces imprimées en PLA (tête, corps, jambes, pieds).
* **Stabilité :** La calibration des axes des 4 servomoteurs doit être parfaite pour garantir la marche sans chute.
* **Personnalisation :** Intégrer au moins une modification esthétique ou fonctionnelle sur OnShape par rapport au modèle standard fourni.

### 2. Contraintes Électroniques et Logicielles
* **Alimentation :** Autonomie assurée par la batterie 9V rechargeable en USB-C.
* **Navigation :** Intégration fonctionnelle du capteur ultrason HC-SR04 pour la détection de l'environnement.
* **Pilotage sans fil :** Connexion Bluetooth BLE stable avec l'application mobile via la bibliothèque **RemoteXY**.

### 3. Critères de Performance (Épreuves)
* **Contrôle :** Réponse instantanée et précise aux commandes des joysticks virtuels (marche avant, arrière, pivots gauche/droite).
* **Sécurité :** Configuration obligatoire d'un appairage sécurisé (Nom du Bluetooth : `lamano otto`, Mot de passe : `lylianolamano`) pour éviter toute interférence ou piratage durant le tournoi.
