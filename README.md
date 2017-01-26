CloudRoboticsOCCI
===================


Prototype of cloud platform for robots as a services.
-----------------------------------------------------

----------

Ce repository contient les projets Eclipse OCCIware pour contrôler un Lego mindstorm "basic" (une voiturette), un Lego mindstorm de type "Robogator" , un Turtle bot, ainsi qu'un Ardrone 1.

## OCCIware Designer ##

L'ensemble de ce projet regroupe donc les projets à importer sous l'Eclipse d'OCCIware, tel que les extensions ainsi que les connecteurs de chacun des projets.

**/!\ Attention : ** La partie de l**'ARdrone** n'as pas été correctement testé suite à des soucis technique **/!\\**

Les drivers pour Legomindstorm ainsi que Turtlebot sont directement dans le dossier **lib** de leurs **connecteurs** respectif.

Enfin, ils sont également disponible dans le dossier [maven-jars](https://github.com/PFECloudRobotics2017/CloudRoboticsOCCI/tree/master/maven-jars).

## Utilisation avec MartServer ##
Pour utiliser [MartServer](https://github.com/cgourdin/MartServer) afin de controler les robots en requête HTTP, il est nécessaire de fournir les dépendances nécessaire à MartServer. 

Par exemple, pour les lego mindstorm, MartServer à besoin de Jar build avec Maven  pour l'extension, le connecteur, ainsi que les drivers. Il en est de même pour le Turtlebot.

Il est nécessaire que chacun de ces Jar soit déclarer dans le **pom.xml** de MartServer comme une dépendance. 

Les Jars énoncé ci-dessus ce trouve dans le dossier [maven-jars](https://github.com/PFECloudRobotics2017/CloudRoboticsOCCI/tree/master/maven-jars). 

Pour que MartServer trouve les dépendances, il est également nécessaire que ces Jars soit importé sur le maven local de votre machine. Pour ce faire, mettez vous dans le répertoire  [maven-jars](https://github.com/PFECloudRobotics2017/CloudRoboticsOCCI/tree/master/maven-jars) et lancez les commandes présentes dans le fichier [command_mvn_local_import](https://github.com/PFECloudRobotics2017/CloudRoboticsOCCI/blob/master/maven-jars/command_mvn_local_import.sh).

## OCCInterface ##
Afin de faciliter l'utilisation de MartServer, il est conseillé d'utiliser [OCCInterface](https://github.com/occiware/OCCInterface).

Enfin, des **samples** on été fait afin de n'avoir que des liens à cliquer pour contrôler les robots.

Pour avoir accès au sample, remplacez le fichier **PostData.md** avec ce [fichier](https://github.com/PFECloudRobotics2017/CloudRoboticsOCCI/blob/master/OCCInterface-Samples/PostData.md) dans votre **OCCInterface**.

Si vous souhaitez changer un attribut ou rajouter une action, référez  vous donc aux exemples fournit dans le fichier.
