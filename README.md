# tp-Hibernate
#Gestion de l'état civil - Projet 
##Description
Le projet consiste en une application de gestion de l'état civil des citoyens de notre province. L'application utilise Hibernate comme framework de persistance et propose des fonctionnalités de gestion des données liées aux citoyens, aux mariages, et aux relations familiales.

##Couche de persistance
Classes Entités
Dans le package ma.projet.beans, nous avons développé les classes entités correspondant à notre modèle de données. Ces classes sont annotées avec les annotations Hibernate nécessaires pour la persistance des données.

##Configuration Hibernate
Nous avons créé un fichier de configuration Hibernate nommé hibernate.cfg.xml dans le package ma.projet.config pour configurer la connexion à la base de données MySQL.

##Classe HibernateUtil
La classe HibernateUtil dans le package ma.projet.util est mise en place pour gérer la session Hibernate.

##Base de données
Nous avons généré la base de données sous MySQL en utilisant les classes entités et les configurations Hibernate.

##Couche Service
Interface IDao
Nous avons créé l'interface générique IDao dans le package ma.projet.dao pour définir les opérations de base de la couche service.

##Classes de Service
Les classes de service, à savoir HommeService, FemmeService, et MariageService, implémentent l'interface IDao. Elles offrent des fonctionnalités spécifiques pour chaque entité.

##HommeService
Méthode pour afficher les épouses d'un homme entre deux dates.
Requête native pour obtenir le nombre d'enfants d'une femme entre deux dates.
##FemmeService
Méthode pour faire appel à la requête native de la question précédente.
Requête nommée pour renvoyer les femmes mariées deux fois ou plus.
Méthode pour faire appel à la requête nommée précédente.
Méthode pour renvoyer le nombre d'hommes mariés par quatre femmes entre deux dates en utilisant l'API Criteria.
Méthode pour renvoyer les mariages d'un homme donné avec un format spécifique.

##Programme de Test
Nous avons également inclus un programme de test pour valider les fonctionnalités du projet. Le programme de test permet de :

Créer des données de test : 10 femmes et 5 hommes.
Afficher la liste des femmes.
Trouver la femme la plus âgée.
Afficher les épouses d'un homme passé en paramètre.
Obtenir le nombre d'enfants d'une femme entre deux dates.
Afficher la liste des femmes mariées deux fois ou plus.
Trouver les hommes mariés par quatre femmes entre deux dates.
Afficher les mariages d'un homme passé en paramètre avec un format spécifique.
![bddtar](https://github.com/ghita-baghdad/tp-Hibernate/assets/147449053/4537f30b-25fb-4161-b230-05cc95e55f17)

#Gestion de Produits - Exercice
Description
Cet exercice consiste en la création d'une application pour la gestion des produits en utilisant Java et Hibernate. 
![Produitexo1](https://github.com/ghita-baghdad/tp-Hibernate/assets/147449053/359abf33-07b9-4978-b7a2-bffd687815c4)

#Application de Gestion de Projets - Exercice

##Description
Cet exercice a pour objectif de créer une application de gestion de projets. L'application doit permettre de gérer les projets, les tâches, les employés et les affectations de tâches aux employés. Les couches de persistance et de service sont mises en place pour permettre l'enregistrement et la récupération des données.

##Couche de Persistance
Classes Entités
Les entités nécessaires pour le modèle de données ont été développées dans le package ma.projet.classes. Les annotations Hibernate appropriées telles que @Entity, @Id, @GeneratedValue, @Column, etc., ont été utilisées.

##Configuration Hibernate
Le fichier de configuration Hibernate, hibernate.cfg.xml, a été créé dans le package ma.projet.config pour configurer la connexion à la base de données.

##Classe HibernateUtil
La classe HibernateUtil dans le package ma.projet.util a été créée pour gérer la création de l'instance de la classe SessionFactory nécessaire pour la gestion des sessions Hibernate.

##Couche de Service
Interface générique IDao
L'interface générique IDao dans le package ma.projet.dao a été créée pour définir les opérations de base que les classes de service implémenteront.

##Classes de Service
Les classes de service, à savoir ProjetService, TacheService, EmployeService, et EmployeTacheService, ont été créées dans le package ma.projet.service. Elles implémentent l'interface IDao pour offrir des fonctionnalités spécifiques.

##EmployeService
Une méthode a été créée pour afficher la liste des tâches réalisées par un employé.
Une méthode a été créée pour afficher la liste des projets gérés par un employé.
##ProjetService
Une méthode a été créée pour afficher la liste des tâches planifiées pour un projet donné.
##TacheService
Une méthode a été créée pour afficher la liste des tâches dont le prix est supérieur à 1000 DH en utilisant une requête nommée.
Une méthode a été créée pour afficher la liste des tâches réalisées entre deux dates.

##Programme de Test
Des programmes de test ont été créés pour valider les fonctionnalités décrites ci-dessus. Les programmes de test doivent couvrir les scénarios suivants :

Affichage des tâches réalisées par un employé.
Affichage des projets gérés par un employé.
Affichage des tâches planifiées pour un projet.
Affichage des tâches dont le prix est supérieur à 1000 DH.
Affichage des tâches réalisées entre deux dates.

![EXO3](https://github.com/ghita-baghdad/tp-Hibernate/assets/147449053/6caae9b8-4bd3-4f91-8e48-66ef8a4ab37d)
