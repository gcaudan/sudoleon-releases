# SudoLéon

Jeu de sudoku pour Android, écrit en Rust avec une interface [Slint](https://slint.dev).

Ce dépôt publie les versions de l'application : chaque
[release](https://github.com/gcaudan/sudoleon-releases/releases) contient l'apk
signé et ses notes de version. Le code source est dans un dépôt privé.

## Sommaire

- [Fonctionnalités](#fonctionnalités)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Mise à jour](#mise-à-jour)
- [Vérifier la signature](#vérifier-la-signature)
- [Licence](#licence)

## Fonctionnalités

- Grilles Facile, Moyen et Difficile, générées à solution unique.
- Mode chronométré, annulation, gomme, notes et complétion automatique des notes.
- Indices étape par étape et avance rapide sur les singles nus.
- Page Techniques : 19 techniques de résolution, avec exemples générés.
- Thème clair, sombre ou système ; portrait et paysage.

## Prérequis

- Android 7.0 (API 24) ou plus récent.
- Processeur 64 bits ARM (`arm64-v8a`).

## Installation

1. Ouvrir la [dernière release](https://github.com/gcaudan/sudoleon-releases/releases/latest)
   depuis le téléphone.
2. Télécharger `sudoleon-vX.Y.Z.apk`.
3. Ouvrir le fichier et autoriser l'installation d'applications depuis le navigateur
   si Android le demande.

## Mise à jour

Installer le nouvel apk par-dessus l'ancien : la partie en cours et les réglages
sont conservés, toutes les versions étant signées par la même clé.

## Vérifier la signature

Empreinte SHA-256 du certificat de signature :

```
08:FA:54:DF:2A:2F:63:D9:92:EE:DC:28:0E:D9:BD:0E:FC:81:01:0A:96:D5:11:AD:B7:3D:FC:21:1F:C7:06:6A
```

Avec les outils du SDK Android :

```bash
apksigner verify --print-certs sudoleon-vX.Y.Z.apk
```

## Licence

[MIT](LICENSE), © 2026 gcaudan. Les licences des composants
embarqués sont consultables dans l'application (À propos → Licences open source).
