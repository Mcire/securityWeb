
# securityWeb
c'est un projet JEE 
#  Consigne
Il était question de réaliser les tâches suivantes :
Listes des taches
 ![image](https://user-images.githubusercontent.com/95756307/213943080-24f41559-5fc7-400e-afa5-d3c1721a26ee.png)

# La concrétisation

Pour commencer nous avons créé un projet Maven web nommé securityweb dans Eclipse.
# Dépendance
 ![image](https://user-images.githubusercontent.com/95756307/213943120-7b30ee53-18b0-4a71-a4e2-78d410a6a2d9.png)

Ces dépendances sont enregistrées dans le fichier pom.xml et sur pour rôle :

- La première dépendance est pour Hibernate, qui est un Framework populaire pour le mapping objet-relationnel (ORM) en Java. 
- La seconde dépendance est pour le connecteur MySQL/J, qui est un pilote qui permet aux applications Java de se connecter à des bases de données MySQL. 
- Les troisième et quatrième dépendance sont pour la bibliothèque de balises standard Jakarta (JSTL), qui est une collection de balises personnalisées qui peuvent être utilisées pour simplifier les tâches courantes dans les JSPs. 
# Dossiers
Ce projet est structuré en plusieurs dossier :
## Le dossier config
Dans le dossier config nous avons le fichier HibernateUtil.java qui est utilisée pour configurer et créer des sessions Hibernate et il permet aussi de configurer la connexion à la base de donnée MySQL.
La classe possède une méthode statique appelée "getSessionFactory" qui renvoie l'usine de sessions. Cette méthode une fois appelle crée les sessions et assure l’interaction avec la base de données.
## Le dossier entities 
Dans ce dossier nous avons deux fichiers (comptes.java et droits.java) qui représente chacune une entité de la base de données. 
Le dossier "entities" est utilisé pour stocker les classes Java qui représentent les entités de la base de données. Ces classes sont annotées avec des annotations Hibernate pour indiquer à Hibernate comment mapper les classes aux tables de la base de données.

## Le dossier dao
Dans le dossier dao (acronyme pour Data Access Object), nous avons deux fichiers (comptedao.java et droitdao.java) qui stockent les classes Java qui gèrent les opérations de base de données.
Ces classes sont responsables de la communication avec la base de données en utilisant les sessions Hibernate et les objets de mapping des entités. A l’intérieur nous avons définis des méthodes pour la création, la lecture, (la mise à jour et la suppression ).
## Le dossier dto
Dans le dossier dto (Data Transfer Object), nous avons deux fichiers (comptedto.java et droitdto.java) qui définissent les méthodes qui doivent être implémentées par les classes dao qui l'implémentent.
## Le dossier controller
Dans notre dossier controller nous avons nos différentes servlets qui gèrent la logique métier et les routes(chemins) … un servlet est une classe Java qui est utilisée pour gérer les requêtes HTTP et les interactions avec l'utilisateur. 
Dans nos servlets, nous avons :
- Des annotations comme @WebServlet qui est utilisée pour déclarer une classe Java comme servlet et pour configurer les URL (URL patterns) qui doivent être mappées à cette servlet.
+ La méthode doGet() qui est une méthode de la classe HttpServlet qui est utilisée pour gérer les requêtes HTTP de type GET.
- La méthode doPost() est une méthode de la classe HttpServlet qui est utilisée pour gérer les requêtes HTTP de type POST.
- La méthode sendRedirect de la classe HttpServletResponse qui permet de rediriger une requête HTTP vers une autre URL. Elle prend en paramètre une chaîne de caractères qui représente l'URL de destination.

## Le dossier webapp
Dans le dossier webapp nous avons les fichiers de l’application web .Ainsi nous avons :
- Le META-INF avec le fichier "MANIFEST.MF", qui contient des informations sur la version, les dépendances et les classes de l'application.
- Le dossier ressource qui contient des fichiers css, JavaScript ,images pour nos différents Template.
- Le WEB-INF contient le web.xml qui est le fichier de configuration pour notre application web et nos fichier JSP qui représente nos vues ou « views »

#La solution

## La page de connexion
 ![image](https://user-images.githubusercontent.com/95756307/213943184-75fdecce-8e30-4b1a-93a6-03199dd710d2.png)

## La liste des comptes
 ![image](https://user-images.githubusercontent.com/95756307/213943204-f63d404b-04de-47cb-9402-522ce7370856.png)

## Ajouter un compte
 ![image](https://user-images.githubusercontent.com/95756307/213943220-c8b2eec5-9ba7-42f2-afa4-e2a9776522be.png)

## Liste des droits
 ![image](https://user-images.githubusercontent.com/95756307/213943231-65e84d82-788c-456b-8530-de3fe40960df.png)

## Ajouter un droit
 ![image](https://user-images.githubusercontent.com/95756307/213943239-3cf1aca2-4821-4b6a-be99-1438ebd57c34.png)

## La base de données
 
![image](https://user-images.githubusercontent.com/95756307/213943248-87898f25-4138-4883-a625-7925b6ad8fc8.png)
