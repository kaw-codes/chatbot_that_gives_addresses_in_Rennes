# Avatar : Chatbot

## Description

Chatbot interactif, voici ses fonctionnalités : 

- Il permet de demander l'adresse d'un lieu dans Rennes. Les adresses sont stockées dans la base de données openData ”vivre à Rennes" : `partie2/vAr.xml`.
- Le bot est capable de politesse : dites-lui bonjour !
- Même avec quelques fautes d'orthographe, il comprendra votre requête.
- Il peut parler 5 langues : Français, Anglais, Espagnol, Allemand et Italien.
- Si une requête peut contenir plusieurs réponses (exemple : "piscine"), il vous proposera tous les lieux possibles correspondant.
- Recherche de restaurant par interrogation du site "Linternaute".
- Il peut  aussi vous répondre à l'oral ! Pour cela, activez sa voix.

L'application a été développée en groupe de 8 étudiants : la Team BACCHUS.

Elle a été écrite en Scala, dans le cadre du cours Génie Logiciel en 2e année de Licence Informatique  à l'ISTIC, Université de Rennes (note du projet : 18/20).

## Installation

- Regarder si la version 17 de Java est disponible sur la machine :

  `update-java-alternatives --list`

- Si elle n'y est pas, installer la version 17 de Java :

  `sudo apt install openjdk-17-jdk`

- Enable Java 17 :

  `sudo update-alternatives --config java`
  
- Installer sbt : https://www.scala-sbt.org/1.x/docs/Installing-sbt-on-Linux.html

## Usage

- à la racine, exécuter :

  `sbt`

- puis :
  
  `compile`

  `run`

- vous aurez le choix entre 6 fonctionnalités.
- choisissez la 6e pour dialoguer avec l'Avatar.

## Ma contribution

Ma contribution portant sur la partie `analyse_phrase`, je me suis occupé du traitement de la requête de l'utilisateur pour renvoyer des couples (lieu, adresse) correspondant. Ils seront ensuite traité par le module `construction_result`, dont je me suis aussi occupé, chargé de construire la réponse de l'Avatar.
