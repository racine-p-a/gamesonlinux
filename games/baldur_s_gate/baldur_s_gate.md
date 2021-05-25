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

Et ajoutez cette ligne ào la fin du fichier :
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