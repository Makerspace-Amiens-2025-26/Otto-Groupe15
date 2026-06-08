---
layout: default
title: Préparation des Matériaux
parent: Etapes de fabrication
nav_order: 1
---

# 🛠️ Préparation des Matériaux

Cette section décrit la première étape essentielle du processus de fabrication : l'inventaire des composants électroniques et le lancement des impressions de la structure.

---

## 📋 Liste des Matériaux et Pièces

### 🔌 Électronique et Motorisation (Kit MakerSpace)
* **Carte électronique Otto-MKS** (Microcontrôleur ESP32 intégré)
* **4 × Servomoteurs** (SG90 ou équivalents pour les articulations)
* **Capteur ultrason** (HC-SR04 pour la détection de distance)
* **Batterie 9V rechargeable** (Alimentation principale via USB-C)

### 🧱 Structure Imprimée en 3D (À réaliser)
* **Fichiers CAO personnalisés sur OnShape** (Tête, Corps, Jambes, Pieds)
* **Filament PLA** (Couleurs au choix pour la personnalisation)

### 🧰 Outils nécessaires
* Jeu de petits tournevis de précision (cruciforme)
* Pince coupante ou pince plate (pour ajuster les câbles et supports si besoin)
* Ordinateur avec l'IDE Arduino installé et câble de programmation

---

## 🖨️ Procédure de Préparation et Impression 3D

1. **Vérification du Kit Électronique :** Déballer l'ensemble des composants fournis par le MakerSpace et faire une vérification visuelle des broches et des câbles pour s'assurer que rien n'est endommagé.
2. **Configuration du Slicer et Impression :** Importer les fichiers STL issus de OnShape dans le logiciel de découpe (Bambu Studio). Configurer les paramètres (remplissage à 15-20% en grille, pas de support requis pour la majorité des pièces d'origine Otto).
3. **Lancement sur BambuLab :** Lancer la fabrication sur l'imprimante 3D **BambuLab**. Grâce à sa vitesse et sa précision, les tolérances d'emboîtement des pièces de structure (jambes et pieds) seront optimales.
4. **Post-traitement des pièces :** Une fois l'impression terminée, retirer délicatement les pièces du plateau texturé. Nettoyer les bavures légères de filament ou les bordures (*brims*) si vous en avez configuré.

---

## ⚠️ Conseils de Sécurité

* **Précautions Impression 3D :** Ne touchez pas la buse chaude ni le plateau de la BambuLab immédiatement après l'impression pour éviter tout risque de brûlure.
* **Sécurité Électronique :** Ne jamais manipuler ou brancher les servomoteurs sur la carte électronique Otto-MKS pendant que la batterie 9V est connectée et active sous tension.

---

Une fois cette étape terminée, passez à l'[Assemblage](/assemblage).
