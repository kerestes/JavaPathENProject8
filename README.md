# TourGuide Project

Tour Guide est une application qui propose des réductions aux voyages des utilisateurs basées sur les points obtenus lors de voyages précédents.

## Preréquis

Pour que le projet fonctionne, vous devez avoir installé :

    - Java 17 (JDK)
    - Maven
    - GpsUtil Module
    - RewardCentral Module
    - TripPricer Module

Pour installer les modules, il suffit de se placer dans le fichier principal du projet et lancer les commande :

    - mvn install:install-file -Dfile=./TourGuide/libs/gpsUtil.jar -DgroupId=gpsUtil -DartifactId=gpsUtil -Dversion=1.0.0 -Dpackaging=jar
    - mvn install:install-file -Dfile=./TourGuide/libs/RewardCentral.jar -DgroupId=rewardCentral -DartifactId=rewardCentral -Dversion=1.0.0 -Dpackaging=jar
    - mvn install:install-file -Dfile=./TourGuide/libs/TripPricer.jar -DgroupId=tripPricer -DartifactId=tripPricer -Dversion=1.0.0 -Dpackaging=jar

## Deploy en local

Pour avoir le code source et le faire rouler en local, il suffit de :

    - Cloner le repositoire
    - Lancer les commandes d'installations des modules

## Deploy en production

Pour lancer le projet en production, il suffit de :

    - Faire un commit ou un pull request (celui-là va déclencher le gitActions workflow)
    - Prendre le fichier .jar dans le dernier workflow sur gitActions
    - Lancer la commande **java -jar tourguide-0.0.1-SNAPSHOT.jar** dans le serveur