# Code Metrics and Call Graph Generator

Ce projet Java analyse le code source Java afin d'extraire des métriques et de générer un graphe d'appel illustrant les relations entre les méthodes.

## Table des matières

- [Fonctionnalités](#fonctionnalités)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Génération du graphe d'appel](#génération-du-graphe-dappel)
- [Auteurs](#auteurs)

## Fonctionnalités

- Analyse des fichiers Java dans un répertoire spécifié.
- Extraction de métriques :
  - Nombre total de classes.
  - Nombre total de méthodes.
  - Nombre total de lignes de code.
  - Moyenne des méthodes par classe.
  - Moyenne des attributs par classe.
- Génération d'un fichier DOT pour visualiser le graphe d'appel des méthodes.

## Prérequis

- **Java Development Kit (JDK)** 11 ou supérieur.
- **Maven** pour la gestion des dépendances.
- **Graphviz** pour visualiser le graphe d'appel.

## Installation

1. **Clonez le dépôt** :

   ```bash
   git clone https://github.com/votre-utilisateur/code-metrics.git
   cd code-metrics
Compilez le projet avec Maven : mvn clean install
2. **Utilisation** :
 - Exécutez le programme : "java -cp target/code-metrics-1.0-SNAPSHOT.jar org.example.Main" 

 - Entrez le chemin du dossier contenant le code source Java lorsque vous y êtes invité.
 - Résultats : Les métriques et le graphe d'appel seront affichés dans la console et un fichier callgraph.dot sera généré dans le répertoire de travail.
Génération du graphe d'appel

## **Génération du graphe d'appel** :

Pour créer une image du graphe d'appel, utilisez Graphviz :

Installez Graphviz (si ce n'est pas déjà fait) :
Générez l'image à partir du fichier DOT : dot -Tpng callgraph.dot -o callgraph.png

 **Auteur** :

Azouze Ibrahim
