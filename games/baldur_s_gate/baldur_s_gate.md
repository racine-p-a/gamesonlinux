# Baldur's Gate

[En français plus bas](baldur_s_gate.md#baldurs-gate-enhanced-edition-version-gog)

## Baldur's Gate: Enhanced Edition (GOG version)

### Installation

You can download a `.sh` file on [GOG website](https://www.gog.com/game/baldurs_gate_enhanced_edition). It should be
at least version `2.6.6.0` or higher/later.

Once it's downloaded, make it executable and launch it.
```bash
# The name might change if the version changes.
./baldur_s_gate_enhanced_edition_2_6_6_0_47291.sh
```

Follow the installer instructions, and it should be ok.

### Problems

#### Missing dependencies

If you have a message like this one :
```text
BaldursGate: error while loading shared libraries: libssl.so.1.0.0: cannot open shared object file: No such file or directory
```

This means you don't have the correct libraries.

Debian users, just install them.
Ubuntu users, add the debian repository and install them.

In this very specific case for ubuntu, follow these steps :
```bash
sudo nano /etc/apt/sources.list
```

And add this line at the end of the file
```text
deb http://security.ubuntu.com/ubuntu xenial-security main
```

Update the repositories list.
```bash
sudo apt update
```

And download the version required.
```bash
sudo apt install libssl1.0.0
```

### Bonus

#### Extract files from the game

You can extract any asset (map, sounds, music, ...) using
[NearInfinity](https://github.com/racine-p-a/NearInfinity/releases/tag/v2.1-20170413). Download the last version
and launch it :
```bash
java -jar NearInfinity.jar
```

Browse to your game files and watch all assets sorted.

## Baldur's Gate: Enhanced Edition (version GOG)

### Installation

Téléchargez le fichier `.sh` sur [le site de GOG](https://www.gog.com/game/baldurs_gate_enhanced_edition) ou
récupérez-le dans la médiathèque familiale.

Une fois téléchargé, rendez-le exécutable et lancez-le.
```bash
# Le nom du fichier peut varier en fonction de sa version.
./baldur_s_gate_enhanced_edition_2_6_6_0_47291.sh
```

Suivez simplement les instructions.

### Problèmes

#### Dépendances absentes

Ce genre de message apparaît :
```text
BaldursGate: error while loading shared libraries: libssl.so.1.0.0: cannot open shared object file: No such file or directory
```
Cela signifie qu'il vous manque des dépendances.

Pour debian, installez-les.
Pour Ubuntu, ajoutez les dépôts de debian et installez-les.

Dans ce cas, sur ubuntu, il faudra faire :
```bash
sudo nano /etc/apt/sources.list
```

Et ajoutez cette ligne à la fin du fichier :
```text
deb http://security.ubuntu.com/ubuntu xenial-security main
```

Mettez à jour la liste des paquets :
```bash
sudo apt update
```

Enfin installez la dépendance manquante :
```bash
sudo apt install libssl1.0.0
```

### Bonus

#### Extraire des fichiers du jeu

Vous pouvez extraire n'importe quel composant du jeu (cartes, sons, musique, ...) avec
[NearInfinity](https://github.com/racine-p-a/NearInfinity/releases/tag/v2.1-20170413). Téléchargez et lancez-le.
```bash
java -jar NearInfinity.jar
```

L'application vous demandera dans quel dossier se trouve le jeu. Une fois que vous lui aurez indiqué, vous pourrez
parcourir les données à votre guise.
Notez toutefois que l'application ne lira que les fichiers de base en anglais. Pour extraire les fichiers d'une autre
langue, une solution possible est de remplacer les fichiers en anglais par ceux que l'on souhaite (pensez à faire une
sauvegarde des fichiers anglais). 