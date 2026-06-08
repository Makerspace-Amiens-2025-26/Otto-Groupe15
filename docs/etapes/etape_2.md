---
layout: default
title: Assemblage
parent: Etapes de fabrication
nav_order: 2
---

# 🤖 Assemblage Mécanique et Électronique

Après la préparation des matériaux et la fin des impressions 3D sur la BambuLab, l'étape suivante consiste à assembler mécaniquement et à câbler le robot Otto-MKS.

---

## ⚙️ Étapes d'Assemblage

1. **Calibrage initial des moteurs :** Avant de fixer définitivement les palonniers, brancher les 4 servomoteurs à blanc pour les caler électroniquement à leur point neutre (90 degrés).
2. **Assemblage de la partie inférieure (Châssis & Jambes) :** * Fixer les deux servomoteurs des jambes dans les emplacements prévus à l'intérieur du corps imprimé en 3D.
   * Emboîter les jambes sur les axes des moteurs et visser les fixations sans forcer.
   * Monter les deux servomoteurs restants au niveau des pieds pour gérer l'inclinaison latérale.
3. **Intégration du Capteur Ultrason :** Insérer le capteur HC-SR04 dans les deux "yeux" situés sur la face avant de la tête imprimée d'Otto.
4. **Montage Électronique et Fixation de la Tête :**
   * Placer la carte Otto-MKS (ESP32) de manière stable dans l'emplacement de la tête.
   * Connecter proprement les connecteurs des 4 servomoteurs sur leurs ports respectifs (en respectant le codage couleur des fils : Masse/Alimentation/Signal).
   * Relier le capteur ultrason à la carte.
   * Loger la batterie 9V rechargeable dans le corps, raccorder son connecteur d'alimentation, puis clipser délicatement la tête sur le corps.

---

## 🔍 Vérifications à Effectuer

* **Alignement Géométrique :** Assurez-vous que toutes les pièces imprimées sur la BambuLab s'emboîtent sans contrainte mécanique excessive. Les jambes doivent être parfaitement perpendiculaires au corps au repos.
* **Liberté de Mouvement :** Vérifiez manuellement (hors tension) que les pieds et les jambes peuvent pivoter sans frotter contre le plastique du châssis.
* **Câblage Intérieur :** Assurez-vous qu'aucun fil électrique ne se retrouve coincé ou écrasé lors de la fermeture de la tête sur le corps du robot.

---

## 💡 Problèmes Communs et Solutions

* **Le robot boite ou ne marche pas droit :** Les palonniers des servomoteurs ont été fixés avec un décalage de quelques crans. Il faut dévisser le membre, remettre le moteur à son point neutre (90°) via le code et réassembler la jambe droite.
* **La tête ne se clipse pas correctement :** Les câbles des moteurs ou de la batterie prennent trop de place à l'intérieur. Rangez soigneusement les fils sous la carte ESP32 pour libérer de l'espace.

- Si des pièces ne s'emboîtent pas correctement, vérifiez leur alignement et leur dimension
