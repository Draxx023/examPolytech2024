# Exam Docker	

1) Forker et cloner le projet https://github.com/vbenji/examPolytech2024

2) Définir un service une base de donnée MySQL dans un fichier docker-compose.yml  
MySQL version 8

3) Configurer la/les bonnes variables d'envrionnements pour la base de donnée

4) Utiliser un volume pour la persistance des données de la base de donnée

5) Créer un Dockerfile pour le projet java et builder votre image  
Java 8 - Port 8448  
ajouter l'instruction LABEL maintainer="prenom"

6) Définir le service pour le projet java dans le docker-compose.yml

7) Utiliser un network pour connecter la base de donnée au service java dans votre docker-compose.yml

8) Configurer la/les bonnes variables d'envrionnements pour que le service java puisse contacter la base de données

9) Modifier le projet angular pour variabiliser l'url d'appel au service java

10) Créer le dockerfile pour l'angular et builder votre image  
node 10  
ajouter l'instruction LABEL maintainer="prenom"

11) Définir le service associé dans le docker-compose.yml avec la/les bonnes variables d'environnements

12) Configurer les healthchecks et les depends_on dans le docker-compose.yml  
Pour mysql vous pouvez utiliser la commande "mysqladmin ping -h localhost"

13) Faire fonctionner les containers ensemble et faire valider

14) Pusher vos deux images sur la registry avec la nomenclature java:prenom et angular:prenom  
Un l'url et le token de connexion vous sera donner pendant l'exam.

15) Rédiger un workflow github action qui permet de builder vos deux docker images

--- 

Dans un fichier txt simple à coté de votre docker-compose.yml répondez aux questions suivantes:  
16) Qu'est ce que Docker ? A quoi cela sert-il ?
    Docker est un outil qui permet de conteneuriser des applications informatiques, comme des services web, des bases de données, etc. Il fournit une interface complète qui donne la possiblité de définir les dépendances d'une application quelconque et la lancer dans un "environment" indépendant de l'environment du hôte, tout en fournissant des fonctionnalités pour la persistance des données, pour les connexions réseau entre conteneurs et avec le hôte lui même. 
    Docker sert à satisfaire un besoin essentiel dans le monde du développement: la portabilité des applications, et ce qui est mieux, c'est qu'il permet d'automatiser cette portabilité, en donnant la possibilité de définir tous les besoins possibles des applications à conteneuriser, et la possibilité de lancer celle-ci sur n'importe quelle machine supportant docker.
17) Qu'est ce que la CI et la CD ? Pourquoi est-ce utile ?
    La CI/CD est un concept DevOps qui est: Continuos Integration / Continuos Delivery (ou deploy mais moi je préfère delivery). Dans d'autres mots, ce concept pose les bases pour l'automatisation du process de validation, packaging, et deploiement des applications informatiques. Il permet dans la phase CI d'intégrer d'une manière automatisée et controllé le nouveau code à la code base existante, à travers des phases de validation comme les pull request, la validation de test, etc. La partie CD permet d'automatiser le process de deploiement à travers la validation des étapes de build et deploy, pour que les nouvelles versions qui ont été validés puissent être livrés sur leurs environment de production spécifiques.
18) Qu'avez vous pensez du cours ? 
    C'est un cours complet qui traite d'une manière pratique et efficace docker, docker compose et github actions, ce qui n'est pas toujours facile. J'ai bien apprécié le travail sur les cas pratiques directs, en utilisant des applcations réelles qu'on connait très bien (cf Michelin). Globalement, c'est un cours que j'ai apprécie vu le fait que docker c'est un sujet récurrent dans mon entreprise. 
19) Surprenez moi
    
20) Créer un repo sur github et pusher votre code
