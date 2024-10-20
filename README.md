TP 1 : Utilisation de la Programmation
Dynamique avec Java

Ce projet illustre l'utilisation de l'injection de dépendances en Java avec la capacité de chargement dynamique de classes via la réflexion. L'objectif est de simuler un design modulaire dans lequel les composants peuvent être facilement interchangeables. La solution repose sur l’utilisation d'interfaces, d’implémentations et d’un fichier de configuration pour injecter dynamiquement les dépendances au moment de l'exécution.

Fonctionnalités Principales

Interfaces DAO et Métier :

IDao : Interface définissant une méthode getValue() pour récupérer une valeur numérique.
IMetier : Interface contenant une méthode calcul() utilisant la valeur fournie par IDao.
Implémentations :

DaoImpl : Implémentation de IDao retournant une valeur fixe (ex. 100.0).
MetierImpl : Implémentation de IMetier qui utilise un objet DAO pour effectuer des calculs.
Injection de Dépendances via Réflexion :

La classe Presentation2 charge dynamiquement les classes DaoImpl et MetierImpl à partir du fichier config.txt et injecte les dépendances au moment de l’exécution.

Pré-requis :

Java JDK 11+
Maven pour la gestion des dépendances
