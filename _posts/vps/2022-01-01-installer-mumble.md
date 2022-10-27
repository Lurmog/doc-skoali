---
layout: post
title: "Installer un serveur Mumble sur un VPS (Debian/Ubuntu)"
description: "Installation d'un serveur Mumble sur un VPS Debian ou Ubuntu"
date: 2022-01-01 15:30:00 +0100
category: vps
---

Afin d’installer un serveur mumble sur votre VPS, suivez ces étapes : 

Faites sudo `sudo apt update && sudo apt upgrade`

Ensuite, faites `sudo apt install mumble-server`

Puis faites `sudo dpkg reconfigure mumble-server`

À la première question, sélectionnez Yes afin que votre serveur Mumble démarre au démarrage de la machine

À la deuxième question, si vous souhaitez que Mumble ai une haute priorité sur les ressources, sélectionnez Yes, autrement, sélectionnez No

Ensuite, il vous sera demandé le mot de passe “Super utilisateur”, entrez celui de votre choix

Pour le démarrer, faites sudo systemctl start mumble-server

Félicitations, vous avez installé votre serveur Mumble !
