# 🧩 Kay Discord Studio — Téléchargements

Crée ton propre bot Discord **sans écrire une ligne de code**, en assemblant des blocs.

---

## 📥 Télécharger

Les liens téléchargent toujours **la dernière version**.

| Système | Téléchargement |
|---|---|
| 🪟 **Windows** 10 / 11 (64 bits) | **[Kay-Discord-Studio-Setup.exe](../../releases/latest/download/Kay-Discord-Studio-Setup.exe)** |
| 🍎 **macOS** Apple Silicon (M1 à M4) | **[Kay-Discord-Studio-mac-arm64.dmg](../../releases/latest/download/Kay-Discord-Studio-mac-arm64.dmg)** |
| 🍎 **macOS** Intel | [Kay-Discord-Studio-mac-x64.dmg](../../releases/latest/download/Kay-Discord-Studio-mac-x64.dmg) |
| 🐧 **Linux** Ubuntu, Debian, Mint… | **[Kay-Discord-Studio-linux-amd64.deb](../../releases/latest/download/Kay-Discord-Studio-linux-amd64.deb)** |
| 🐧 **Linux** autres distributions | [Kay-Discord-Studio-linux-x86_64.AppImage](../../releases/latest/download/Kay-Discord-Studio-linux-x86_64.AppImage) |

Toutes les versions publiées sont dans l’onglet **[Releases](../../releases)**.

---

## 🚀 Installation et premier lancement

Au premier lancement, colle ta **clé bêta** obtenue sur le serveur Discord communautaire (salon `#obtenir-la-bêta`).

### 🪟 Windows

1. Lance **`Kay-Discord-Studio-Setup.exe`** : pas besoin de droits administrateur.
2. *SmartScreen :* tant que l’application n’est pas signée, Windows peut afficher « Windows a protégé votre ordinateur ». Clique sur **« Informations complémentaires »** puis **« Exécuter quand même »**.

### 🍎 macOS

1. Ouvre le **.dmg** et glisse **Kay Discord Studio** dans **Applications**.
2. *Gatekeeper :* tant que l’application n’est pas notarisée par Apple, macOS refuse la première ouverture.
   Ouvre **Réglages Système → Confidentialité et sécurité**, descends jusqu’à « Kay Discord Studio a été bloqué » et clique sur **« Ouvrir quand même »**.
   Si macOS indique que l’application est « endommagée », lance une fois dans le Terminal :
   ```bash
   xattr -cr "/Applications/Kay Discord Studio.app"
   ```

### 🐧 Linux

- **.deb** (Ubuntu, Debian, Mint, Pop!_OS…) :
  ```bash
  sudo apt install ./Kay-Discord-Studio-linux-amd64.deb
  ```
  L’application apparaît ensuite dans le menu des applications.
- **AppImage** (toutes distributions) :
  ```bash
  chmod +x Kay-Discord-Studio-linux-x86_64.AppImage
  ./Kay-Discord-Studio-linux-x86_64.AppImage
  ```
  Sur Ubuntu 24.04 et plus récent, si rien ne s’ouvre, ajoute `--no-sandbox` (ou préfère le .deb).
- Pour garder ton token chiffré, un trousseau doit être actif (GNOME Keyring ou KWallet, présents par défaut sur les bureaux courants).

---

## ✨ Fonctionnalités principales

- 🪄 **Éditeur visuel par blocs** : commandes slash, boutons, menus déroulants, formulaires (modales).
- 🧱 **Messages Discord modernes (Components V2)** avec aperçu en direct.
- 🛡️ **Sécurité clé en main** : captcha à clavier, anti-spam, filtre de liens, détection de raid et de comptes récents.
- 🎫 **Système de tickets complet** : panneau personnalisable, prise en charge, statuts, membres et archives.
- 🖼️ **Cartes d’arrivée et de départ** générées automatiquement avec aperçu fidèle.
- 🗄️ **Base de données intégrée** (SQLite sans installation, ou PostgreSQL, MySQL, MongoDB) et minuteurs persistants.
- 🎮 **Apprentissage guidé** : 43 missions, badges et niveaux de progression.
- 🚀 **Export prêt à héberger 24 h/24** (Node.js / Docker).

---

## 🩺 L’application ne s’affiche pas correctement ?

Cette version affiche toujours quelque chose à l’écran : un démarrage en cours, puis — si la licence de ton ordinateur ne peut pas être lue — un message d’erreur avec un bouton **« Réessayer »**.

Si un message s’affiche ou si la fenêtre reste noire, joins à ton signalement le fichier :

| Système | Fichier |
|---|---|
| Windows | `%APPDATA%\Kay Discord Studio\kds-debug.log` (à coller dans la barre d’adresse de l’Explorateur) |
| macOS | `~/Library/Application Support/Kay Discord Studio/kds-debug.log` |
| Linux | `~/.config/Kay Discord Studio/kds-debug.log` |

Il contient le détail technique du démarrage et permet de comprendre ce qui s’est passé sur ton ordinateur.

---

## 💬 Besoin d’aide ou envie de signaler un bug ?

Rends-toi sur le serveur Discord officiel de **Kay Discord Studio** :
- utilise `/bug` pour signaler un problème ;
- utilise `/idee` pour proposer une amélioration ;
- ouvre un ticket dans `#support` pour obtenir de l’aide.
