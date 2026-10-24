# Termoria

**Toutes vos connexions distantes dans une seule fenêtre, pour Windows.**
SSH, Bureau à distance (RDP), VNC, Telnet, port série et consoles web : une application légère (installateur de moins de 10 Mo), rapide et pensée pour le quotidien des administrateurs.

![Termoria : arbre des sessions, terminal SSH et explorateur de fichiers](docs/termoria-sombre.png)

## Télécharger

➡️ **[Dernière version](https://github.com/jpiperault/Termoria-releases/releases/latest)** : téléchargez `Termoria_x.y.z_x64-setup.exe` et lancez-le.

- Installation pour l'utilisateur courant, **sans droits administrateur**.
- Windows 10 et 11 (64 bits).
- Termoria **se met ensuite à jour tout seul** : une bannière propose chaque nouvelle version, rien ne s'installe sans votre accord.

## Ce que fait Termoria

**Connexions**
- **SSH** compatible OpenSSH 10 : clé privée (y compris les clés PuTTY `.ppk`), mot de passe ou agent (Pageant / OpenSSH), mode compatibilité pour les anciens équipements.
- **Bureau à distance (RDP)** dans un onglet, avec presse-papiers partagé et écran adapté à la taille de la fenêtre, ou dans le client Windows au choix.
- **VNC**, **Telnet**, **port série** (ports COM détectés automatiquement) et **consoles web**.

**Au quotidien**
- **Explorateur de fichiers SFTP** à côté du terminal : glisser-déposer de fichiers et de dossiers entiers, édition d'un fichier distant dans votre éditeur habituel avec renvoi automatique.
- **Écran partagé** jusqu'à 4 sessions, et **saisie multiple** pour taper la même commande sur plusieurs serveurs.
- **Commandes enregistrées** (Ctrl+Maj+P), **tunnels SSH** (port local, proxy SOCKS), **reconnexion automatique**.
- **Supervision** : pastille verte ou rouge et latence pour chaque serveur.
- **Dossiers et sous-dossiers**, **couleurs par dossier** (repérez la production d'un coup d'œil), thème clair ou sombre, 9 palettes de terminal.
- **Import** depuis `~/.ssh/config`, PuTTY et mRemoteNG.

![Écran partagé en thème clair](docs/termoria-ecran-partage-clair.png)

**Sécurité**
- Mots de passe rangés dans le **Gestionnaire d'identifiants Windows**, jamais en clair sur le disque.
- **Verrouillage** par mot de passe maître ou **Windows Hello**, au démarrage et après inactivité.
- Clés des serveurs SSH vérifiées : une clé qui change bloque la connexion.
- Mises à jour **signées**.

## Éditions

Termoria est **gratuit pour un usage personnel**, avec tous les protocoles.
Une édition **Pro** (enregistrement des sessions, alertes de supervision, synchronisation entre PC…) et une édition **Équipes** sont en préparation. Pendant l'avant-première, toutes les fonctions sont débloquées.

## Signaler un problème

Ouvrez une [issue](https://github.com/jpiperault/Termoria-releases/issues) en décrivant ce que vous faisiez, le message affiché et la version de Termoria (en bas à droite de la fenêtre).

---

© Termoria. Tous droits réservés. Termoria s'appuie sur des logiciels libres (Tauri, russh, IronRDP, xterm.js, vnc-rs…), sous licences MIT et Apache 2.0.
