# Installation de macOS sur VMware avec un processeur AMD
  
## Résumé

Ce projet est un résumé de toutes les ressources que j'ai pu trouver sur Internet pour créer une machine virtuelle macOS sur VMware avec un processeur AMD. Après avoir essayé plusieurs versions de macOS, y compris macOS 13, macOS 14.3 et macOS 14.6, j'ai constaté que seule la version 12 (Monterey) fonctionnait de manière stable avec ma configuration.

L'objectif de ce **Répertoire** est de partager mon expérience et les solutions qui ont finalement fonctionné pour moi, dans l'espoir d'aider d'autres utilisateurs avec des configurations similaires. Ce guide couvre les étapes d'installation de macOS 12 sur VMware avec un processeur AMD, ainsi que les astuces pour optimiser la machine virtuelle.

## Ma configuration

* **Carte mère :** MSI B550 PRO-VDH WI-FI
* **Processeur :** AMD Ryzen 7 5700X
* **Mémoire vive :** Corsair 4x8Go 3200MHz
* **Carte graphique :** NVidia GTX 1070

## Sommaire
1. [Introduction](#introduction)
2. [Prérequis](#prérequis)
3. [Création de la machine virtuelle](#création-de-la-machine-virtuelle)
4. [Installation de macOS](#installation-de-macos)
5. [Installation de VMware Tools](#installation-de-vmware-tools)
6. [Modifications post-installation](#modifications-post-installation)
7. [FAQ et Discussion](#faq-et-discussion)
8. [Suggestions et Améliorations](#suggestions-et-améliorations)

## Introduction

Ce guide vous montre comment installer macOS Monterey (12) sur VMware avec un processeur AMD. L'installation de macOS sur des processeurs AMD est souvent plus complexe que sur Intel en raison des différences d'architecture, mais avec les bons outils et les bonnes configurations, c'est tout à fait réalisable.

## Prérequis

Avant de commencer, voici ce dont vous aurez besoin :
- VMware Workstation Pro (ou VMware Player)
- Unlocker pour VMware
- ISO de macOS Monterey (version 12)
- Clover Configurator pour les réglages post-installation
- Un fichier `darwin.iso` pour installer les VMware Tools

Assurez-vous que la virtualisation est activée dans le BIOS de votre carte mère. Vous devrez également activer certaines options sous Windows pour permettre un fonctionnement optimal de la VM.  
Voir [Virtualisation](https://github.com/clemeeento/macOS-VMware-AMD/blob/main/1%20-%20Virtualisation.md) pour plus de détails.

## Création de la machine virtuelle

Suivez les instructions détaillées dans la section [Création de la machine virtuelle](https://github.com/clemeeento/macOS-VMware-AMD/blob/main/2%20-%20Cr%C3%A9ation%20de%20la%20VM.md) pour configurer VMware, créer une VM avec macOS Monterey, et effectuer les ajustements nécessaires dans le fichier `.vmx`.

## Installation de macOS

L'installation de macOS suit un processus relativement standard une fois la machine virtuelle configurée. Cependant, vous devrez effectuer certaines étapes spécifiques (comme l'utilisation de l'Utilitaire de disque pour formater le disque virtuel en APFS). Voir [Installation de macOS](https://github.com/clemeeento/macOS-VMware-AMD/blob/main/3%20-%20Installation%20de%20macOS.md) pour plus de détails.

## Installation de VMware Tools

L'installation des VMware Tools est essentielle pour bénéficier de fonctionnalités supplémentaires telles que le redimensionnement de la résolution d'écran et l'amélioration des performances générales. Suivez les instructions dans la section [Installation de VMware Tools](https://github.com/clemeeento/macOS-VMware-AMD/blob/main/4%20-%20Installation%20de%20VMware%20Tools.md).

## Modifications post-installation

Pour désactiver les mises à jour automatiques et faire fonctionner le Mac App Store, suivez les étapes décrites dans [Modifications post-installation](https://github.com/clemeeento/macOS-VMware-AMD/blob/main/5%20-%20Modifications%20Post-Installation.md). Ces ajustements sont essentiels pour une utilisation fluide de macOS dans un environnement virtuel.

## FAQ et Discussion

### Questions fréquentes

J'ai créé une section de **Discussion** sur ce projet pour permettre à d'autres utilisateurs de poser des questions et de partager leurs expériences. Si vous rencontrez des problèmes ou si vous avez des questions sur l'installation ou la configuration, n'hésitez pas à ouvrir un sujet dans la section **FAQ et Discussion**. J'essaierai de répondre à toutes les questions dans la mesure du possible.

## Suggestions et Améliorations

Cette section est ouverte à tous ceux qui souhaitent contribuer à l'amélioration de ma VM ou à l'installation d'autres versions plus récentes de macOS sur VMware avec un processeur AMD. Si vous avez des suggestions ou des astuces pour améliorer les performances, ou même si vous avez réussi à installer une version plus récente de macOS, je serais heureux d'en discuter et d'intégrer vos idées dans ce guide.

Je vous invite également à partager vos conseils dans la section **Suggestions et Améliorations** afin que la communauté puisse en bénéficier.

---

Merci d'avoir lu ce guide, et j'espère que mon expérience pourra vous aider dans vos propres tentatives d'installation de macOS sur VMware avec un processeur AMD !
