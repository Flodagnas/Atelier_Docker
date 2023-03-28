# Atelier_Docker

## Prérequis
Avant de commencer, assurez-vous d'avoir les éléments suivants installés sur votre système :

. Docker Desktop (si vous utilisez Windows ou macOS) ou Docker Engine (si vous utilisez Linux)
. Un éditeur de texte de votre choix (par exemple, Visual Studio Code)
##Objectifs
Dans ce TP, vous allez :

### Créer votre première image Docker
Exécuter un conteneur à partir de votre image
Comprendre les concepts de base de Docker
Utiliser Docker Compose pour exécuter une application multi-conteneurs
1. Créer votre première image Docker
Dans cette partie, vous allez créer votre première image Docker. Pour cela, vous allez créer un fichier Dockerfile dans un répertoire vide. Ce fichier contiendra les instructions nécessaires pour créer votre image.

Voici un exemple de fichier Dockerfile simple qui utilise une image de base Ubuntu pour créer une image qui exécute la commande echo :
