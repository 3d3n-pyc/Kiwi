# KIWI

Kiwi est un script Python conçu pour vérifier le style de code et nettoyer les fichiers temporaires dans un répertoire de livraison. Il utilise Docker pour exécuter un vérificateur de style de code et génère un rapport des erreurs de style de code trouvées.


## Prérequis

- Python 3.x
- Docker
- Accès à internet pour télécharger le token et l'image Docker


## Installation

Clonez le dépôt et accédez au répertoire du projet :

```bash
  git clone https://github.com/3d3n-pyc/Kiwi.git
  cd Kiwi
```

Installer les dépendances :

```bash
  pip install requests
```

Ajoutez le script [kiwi](kiwi) dans le répertoire `/bin/` :

```bash
  sudo cp kiwi /bin/
```


## Utilisation

Le script [kiwi](kiwi) peut être exécuté avec différentes options pour nettoyer les fichiers temporaires ou changer le répertoire de livraison.

Options
- `-c`, `--clean` : Supprime les fichiers temporaires dans le répertoire de livraison.
- `-p <path>`, `--path <path>` : Change le répertoire de livraison.
- `-h`, `--help` : Affiche l'aide et les options disponibles.


## Exemples

Pour nettoyer les fichiers temporaires :

```bash
kiwi -c
```

Pour changer le répertoire de livraison :

```bash
kiwi -p /chemin/vers/repertoire
```

Pour afficher l'aide :

```bash
kiwi -h
```


## Fonctionnalités

- **Nettoyage des fichiers temporaires** : Supprime les fichiers temporaires tels que `#*#`, `*~`, `*.o`, `*.hi`, `*.a`, `*.so` dans le répertoire de livraison.
- **Vérification du style de code** : Utilise Docker pour exécuter un vérificateur de style de code et génère un rapport des erreurs de style de code trouvées.
- **Affichage des erreurs** : Affiche les erreurs de style de code avec des descriptions et des couleurs pour une meilleure lisibilité.
- **ASCII Art** : Affiche un joli art ASCII d'un kiwi si aucune erreur de style de code n'est trouvée.


## Auteurs

- [@EtienneP-26](https://www.github.com/EtienneP-26) et [@tombaes](https://www.github.com/tombaes) (ASCII Art)
- [@3d3n-pyc](https://www.github.com/3d3n-pyc)


## License

Ce projet est sous licence [MIT](https://choosealicense.com/licenses/mit/). Voir le fichier [LICENSE](LICENSE) pour plus de détails.
