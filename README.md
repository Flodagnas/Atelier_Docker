# Atelier_Docker

## Prérequis
Avant de commencer, assurez-vous d'avoir les éléments suivants installés sur votre système :    

. Docker Desktop (si vous utilisez Windows ou macOS) ou Docker Engine (si vous utilisez Linux)    
. Un éditeur de texte de votre choix (par exemple, Visual Studio Code)    
## Objectifs
Dans ce TP, vous allez :

### Créer votre première image Docker
Exécuter un conteneur à partir de votre image   
Comprendre les concepts de base de Docker   
Utiliser Docker Compose pour exécuter une application multi-conteneurs    
#### 1. Créer votre première image Docker    
Dans cette partie, vous allez créer votre première image Docker. Pour cela, vous allez créer un fichier Dockerfile dans un répertoire vide. Ce fichier contiendra les instructions nécessaires pour créer votre image.    

Voici un exemple de fichier Dockerfile simple qui utilise une image de base Ubuntu pour créer une image qui exécute la commande echo :    
```
FROM ubuntu
CMD echo "Hello Docker!"
```

Pour créer votre image, ouvrez une fenêtre de terminal et naviguez jusqu'au répertoire où se trouve votre Dockerfile.   
Exécutez ensuite la commande suivante :
```
docker build -t myimage .
```
Cette commande crée une nouvelle image Docker à partir de votre Dockerfile et lui donne le nom myimage. Le . à la fin de la commande spécifie que Docker doit utiliser le répertoire courant comme contexte de construction.    
#### 2. Exécuter un conteneur à partir de votre image    
Maintenant que vous avez créé votre image, vous allez l'utiliser pour exécuter un conteneur. Pour cela, exécutez la commande suivante :   
```
docker run myimage
```
Cette commande démarre un nouveau conteneur à partir de votre image myimage et exécute la commande echo. Vous devriez voir le message "Hello Docker!" s'afficher dans votre terminal.   
#### 3. Comprendre les concepts de base de Docker    
Maintenant que vous avez créé et exécuté une image Docker, il est important de comprendre les concepts de base de Docker.   

Docker est une plateforme de conteneurisation qui permet d'isoler des applications dans des conteneurs. Les conteneurs sont des instances exécutables d'images Docker qui contiennent tout le nécessaire pour exécuter l'application, y compris le code, les bibliothèques et les dépendances.    

Voici quelques termes de base que vous devez connaître :    

. Image : un modèle de fichier binaire qui contient tout ce qui est nécessaire pour exécuter une application, y compris le code, les bibliothèques et les dépendances.
. Conteneur : une instance exécutable d'une image Docker.
. Dockerfile : un fichier qui contient des instructions pour créer une image Docker.
. docker build : une commande qui crée une image Docker à partir d'un Dockerfile.
. docker run : une commande qui démarre un conteneur à partir d'une image Docker.
. docker ps : une commande qui liste tous les conteneurs en cours d'exécution.
. docker stop : une commande qui arrête un
