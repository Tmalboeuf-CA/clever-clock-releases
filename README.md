# Clever Clock : installeurs

Ce dépôt ne contient que les installeurs de Clever Clock, publiés dans ses
[releases](../../releases/latest). L'application installée y cherche elle-même ses mises à jour.

## Installer

Télécharger le fichier de la [dernière version](../../releases/latest) :

- **Linux** : `Clever-Clock-<version>.AppImage`. Le rendre exécutable (clic droit › Propriétés ›
  Permissions, ou `chmod +x Clever-Clock-*.AppImage`) puis le lancer. Sur Ubuntu, `libfuse2` est
  nécessaire (`sudo apt install libfuse2` s'il manque).
- **Windows** : `Clever-Clock-Setup-<version>.exe`. L'installeur n'est pas signé : à l'alerte
  « Windows a protégé votre ordinateur », cliquer sur « Informations complémentaires » puis
  « Exécuter quand même ».
- **macOS** (Intel et Apple Silicon) : `Clever-Clock-<version>.dmg`. L'ouvrir et glisser Clever
  Clock dans Applications. L'application n'est pas signée par Apple : au premier lancement, macOS
  la bloque ; aller dans Réglages Système › Confidentialité et sécurité, puis cliquer sur « Ouvrir
  quand même ». Si macOS indique que l'application est « endommagée », lancer dans un Terminal :
  `xattr -dr com.apple.quarantine "/Applications/Clever Clock.app"`.

## Mises à jour

Automatiques : l'application cherche les nouvelles versions au démarrage puis toutes les 4 heures,
les télécharge en arrière-plan et les installe à sa fermeture (ou tout de suite avec le bouton
« Redémarrer » de la barre latérale).

Sur macOS, l'application non signée ne peut pas se remplacer elle-même : elle annonce la nouvelle
version avec un bouton « Télécharger ». Installer le nouveau `.dmg` comme la première fois, en
remplaçant l'ancienne application ; les données sont conservées.

## Configuration

Pour récupérer les clients et projets d'un collègue : il les exporte depuis Réglages › Partager la
configuration › Exporter, puis vous les importez au même endroit.
