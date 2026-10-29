# Portunia

**Toutes vos connexions distantes dans une seule fenêtre, pour Windows.**
SSH, Bureau à distance (RDP), VNC, Telnet, FTP, port série, shells locaux et consoles web : une application légère (installateur de moins de 10 Mo), rapide et pensée pour le quotidien des administrateurs.

> Portunia s'appelait **Termoria** jusqu'à la version 0.39. Une installation de Termoria passe à Portunia par la mise à jour automatique et garde ses sessions, son coffre et ses réglages.

![Portunia : arbre des sessions, terminal SSH et explorateur de fichiers](docs/termoria-sombre.png)

## Télécharger

➡️ **[Dernière version](https://github.com/jpiperault/Portunia-releases/releases/latest)** : téléchargez `Portunia_x.y.z_x64-setup.exe` et lancez-le.

- Installation pour l'utilisateur courant, **sans droits administrateur**.
- Windows 10 et 11 (64 bits).
- Portunia **se met ensuite à jour tout seul** : une bannière propose chaque nouvelle version, rien ne s'installe sans votre accord.

## Ce que fait Portunia

**Connexions**
- **SSH** compatible OpenSSH 10 : clé privée (y compris les clés PuTTY `.ppk`), mot de passe ou agent (Pageant / OpenSSH), serveurs de rebond enchaînés, mode compatibilité pour les anciens équipements.
- **Bureau à distance (RDP)** dans un onglet, avec presse-papiers partagé et écran adapté à la taille de la fenêtre, ou dans le client Windows au choix.
- **VNC**, **Telnet**, **port série** (ports COM détectés automatiquement), **FTP / FTPS** et **consoles web**.
- **Shells locaux** : PowerShell, Invite de commandes, distributions WSL, Git Bash.
- **Connexion rapide** : tapez `ssh deploy@10.0.1.12`, `rdp srv-01` ou une simple adresse, sans créer de session.

**Au quotidien**
- **Explorateur de fichiers SFTP** à côté du terminal : glisser-déposer de fichiers et de dossiers entiers, édition d'un fichier distant dans votre éditeur habituel avec renvoi automatique.
- **Écran partagé** jusqu'à 4 sessions, et **saisie multiple** pour taper la même commande sur plusieurs serveurs.
- **Commandes enregistrées** (Ctrl+Maj+P), **tunnels SSH** (port local, proxy SOCKS, port distant), **X11**, **reconnexion automatique**.
- **Notes par session** en Markdown, **identifiants partagés** entre sessions, **outils réseau** (ping, traceroute, test de ports, DNS, Wake-on-LAN).
- **Supervision** : pastille verte ou rouge et latence pour chaque serveur.
- **Dossiers et sous-dossiers**, **couleurs par dossier** (repérez la production d'un coup d'œil), thème clair ou sombre, 9 palettes de terminal.
- **Import** depuis `~/.ssh/config`, PuTTY et mRemoteNG.

![Écran partagé en thème clair](docs/termoria-ecran-partage-clair.png)

**Bastion Heimdia**
Portunia se connecte au bastion SSH [Heimdia](https://github.com/jpiperault/Heimdia-releases) : contrôle d'accès, double authentification, comptes des serveurs gardés dans un coffre, sessions enregistrées et journal infalsifiable. Les serveurs autorisés apparaissent dans la barre latérale et s'ouvrent d'un clic.

**Sécurité**
- Mots de passe rangés dans le **Gestionnaire d'identifiants Windows**, jamais en clair sur le disque ; données chiffrées dès qu'un mot de passe maître est défini.
- **Verrouillage** par mot de passe maître ou **Windows Hello**, au démarrage et après inactivité.
- Clés des serveurs SSH vérifiées : une clé qui change bloque la connexion.
- Mises à jour **signées**.

## Éditions

Portunia est **gratuit pour un usage personnel**, avec tous les protocoles.

- **Pro** : enregistrement des sessions, tableau de bord des serveurs, commande sur plusieurs serveurs, conteneurs Docker et Kubernetes, alertes de supervision, stockage S3.
- **Équipes** : administration du bastion Heimdia depuis Portunia.

Pendant l'avant-première, toutes les fonctions sont débloquées.

## Signaler un problème

Ouvrez une [issue](https://github.com/jpiperault/Portunia-releases/issues) en décrivant ce que vous faisiez, le message affiché et la version de Portunia (en bas à droite de la fenêtre).

---

© Portunia. Tous droits réservés. Portunia s'appuie sur des logiciels libres (Tauri, russh, IronRDP, xterm.js, vnc-rs…), sous licences MIT et Apache 2.0.
