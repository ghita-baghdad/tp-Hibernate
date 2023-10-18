# tp-Hibernate :

# Gestion de l'État Civil - Projet
Ce projet consiste en une application de gestion de l'état civil des citoyens de notre province. L'application utilise Hibernate comme framework de persistance et propose des fonctionnalités de gestion des données liées aux citoyens, aux mariages, et aux relations familiales.

# Configuration Hibernate
Le projet repose sur Hibernate, un framework de persistance pour la gestion des données. La configuration Hibernate est essentielle pour établir la connexion avec la base de données MySQL. Le fichier de configuration hibernate.cfg.xml dans le package ma.projet.config est utilisé à cette fin.

# Couche de Persistance
Classes Entités
Les classes entités, situées dans le package ma.projet.beans, représentent le modèle de données. Elles sont annotées avec les annotations Hibernate nécessaires pour permettre la persistance des données.

# Base de Données
La base de données sous MySQL est générée en utilisant les classes entités et les configurations Hibernate. Cela garantit que les données sont stockées de manière cohérente.

# Couche Service
Interface IDao
L'interface générique IDao, située dans le package ma.projet.dao, définit les opérations de base pour la couche de service. Cette interface est implémentée par les classes de service spécifiques.

# Classes de Service

_HommeService :

-Méthode pour afficher les épouses d'un homme entre deux dates et creation d'une requête native pour obtenir le nombre d'enfants d'une femme entre deux dates.

_FemmeService :

Creation d'une requête nommée pour renvoyer les femmes mariées deux fois ou plus.
Méthode pour renvoyer le nombre d'hommes mariés par quatre femmes entre deux dates en utilisant l'API Criteria.
Méthode pour renvoyer les mariages d'un homme donné avec un format spécifique.

_Programme de Test :
Un programme de test est inclus pour valider les differentes fonctionnalités du projet. Le programme de test permet de :

Créer des données de test : 10 femmes et 5 hommes.
Afficher la liste des femmes.
Trouver la femme la plus âgée.
Afficher les épouses d'un homme passé en paramètre.
Obtenir le nombre d'enfants d'une femme entre deux dates.
Afficher la liste des femmes mariées deux fois ou plus.
Trouver les hommes mariés par quatre femmes entre deux dates.
Afficher les mariages d'un homme passé en paramètre avec un format spécifique.

# Voici le modele conceptuel de la base de donnée du projet :
![bddtar](https://github.com/ghita-baghdad/tp-Hibernate/assets/147449053/4537f30b-25fb-4161-b230-05cc95e55f17)


# Gestion de Produits - Exercice 1

# Description :
Cet exercice consiste en la création d'une application pour la gestion des produits en utilisant Java et Hibernate. 

![Produitexo1](https://github.com/ghita-baghdad/tp-Hibernate/assets/147449053/359abf33-07b9-4978-b7a2-bffd687815c4)

# Application de Gestion de Projets - Exercice 3

# Description :
Cet exercice a pour objectif de créer une application de gestion de projets. L'application doit permettre de gérer les projets, les tâches, les employés et les affectations de tâches aux employés. Les couches de persistance et de service sont mises en place pour permettre l'enregistrement et la récupération des données.

# Couches de Persistance
Classes Entités
Les classes entités nécessaires pour le modèle de données ont été développées dans le package ma.projet.classes. Ces classes sont annotées avec les annotations Hibernate appropriées telles que @Entity, @Id, @GeneratedValue, @Column, etc., pour permettre leur persistance dans la base de données.

# Configuration Hibernate
Le fichier de configuration Hibernate, hibernate.cfg.xml, a été créé dans le package ma.projet.config pour configurer la connexion à la base de données. Ce fichier est essentiel pour établir une connexion réussie avec la base de données.

# Classe HibernateUtil
La classe HibernateUtil dans le package ma.projet.util a été créée pour gérer la création de l'instance de la classe SessionFactory, nécessaire pour la gestion des sessions Hibernate. Cette classe est cruciale pour la gestion de la persistance des données.

# Couche de Service
Interface Générique IDao
L'interface générique IDao, située dans le package ma.projet.dao, a été créée pour définir les opérations de base que les classes de service implémenteront. Cela permet d'assurer une structure cohérente dans la couche de service.

# Classes de Service
Les classes de service, à savoir ProjetService, TacheService, EmployeService, et EmployeTacheService, ont été créées dans le package ma.projet.service. Elles implémentent l'interface IDao pour offrir des fonctionnalités spécifiques liées à la gestion de projets, tâches, employés, et affectations de tâches.

_EmployeService:
Une méthode a été créée pour afficher la liste des tâches réalisées par un employé.
Une méthode a été créée pour afficher la liste des projets gérés par un employé.

_ProjetService:
Une méthode a été créée pour afficher la liste des tâches planifiées pour un projet donné.

_TacheService :
Une méthode a été créée pour afficher la liste des tâches dont le prix est supérieur à 1000 DH en utilisant une requête nommée.
Une méthode a été créée pour afficher la liste des tâches réalisées entre deux dates.

# Programme de Test
Des programmes de test ont été créés pour valider les fonctionnalités décrites ci-dessus. Les programmes de test couvrent les scénarios suivants :

Affichage des tâches réalisées par un employé.
Affichage des projets gérés par un employé.
Affichage des tâches planifiées pour un projet.
Affichage des tâches dont le prix est supérieur à 1000 DH.
Affichage des tâches réalisées entre deux dates.

![EXO3](https://github.com/ghita-baghdad/tp-Hibernate/assets/147449053/6caae9b8-4bd3-4f91-8e48-66ef8a4ab37d)
