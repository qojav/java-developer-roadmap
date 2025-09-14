# Phase 6 – Projets Finaux (En continu)

### Projet 1 : CRUD Complet avec Authentification
- **Objectif** : Construire une API RESTful robuste avec authentification sécurisée et tests.  
- **Technologies** : Spring Boot, Spring Data JPA (PostgreSQL), Spring Security (JWT), JUnit 5, Testcontainers.  
- **Fonctionnalités** : CRUD pour les entités (par exemple, tâches, utilisateurs), authentification avec roles (ADMIN, USER), documentation avec Swagger.  
- **Optionnel** : Ajouter une interface Thymeleaf pour visualiser/gérer les tâches.  
- **Exemple** : API pour gérer des projets (entités : `Project`, `Task`, `User`) avec des endpoints protégés.  

### Projet 2 : Téléchargement de Fichiers
- **Objectif** : Ajouter une fonctionnalité de téléchargement de fichiers à l’API du Projet 1.  
- **Technologies** : Spring Boot (`MultipartFile`), Amazon S3 ou stockage local, validation des fichiers.  
- **Fonctionnalités** : Télécharger des images/documents associés aux tâches, valider le type/taille.  
- **Exemple** : Permettre le téléchargement de pièces jointes (par exemple, PDF, PNG) pour les tâches dans l’API.  

### Projet 3 : Déploiement dans le Cloud
- **Objectif** : Déployer l’API sur une plateforme cloud avec CI/CD.  
- **Technologies** : Railway, Heroku, ou AWS (Elastic Beanstalk), GitHub Actions, Docker.  
- **Fonctionnalités** : Empaqueter en JAR/Docker, configurer les variables d’environnement, automatiser le déploiement.  
- **Optionnel** : Implémenter un caching avec Redis pour optimiser les requêtes fréquentes.  
- **Exemple** : Déployer l’API du projet sur Railway avec PostgreSQL et CI/CD.  

### Projet 4 : Microservices
- **Objectif** : Diviser l’API du Projet 1 en microservices orchestrés.  
- **Technologies** : Spring Cloud (Eureka, Gateway), Docker Compose, REST pour la communication.  
- **Fonctionnalités** : Microservices pour `Tasks` et `Users`, avec découverte de services.  
- **Optionnel** : Utiliser RabbitMQ pour une communication asynchrone entre microservices.  
- **Exemple** : Séparer la logique des tâches et des utilisateurs en deux services, orchestrés avec Docker.  

### Projet 5 : Intégration d’API Externe
- **Objectif** : Consommer une API externe pour enrichir les fonctionnalités.  
- **Technologies** : Spring RestTemplate ou WebClient, authentification API (par exemple, OAuth2).  
- **Fonctionnalités** : Intégrer une API publique (par exemple, envoyer des notifications par email avec SendGrid).  
- **Optionnel** : Ajouter une query GraphQL pour récupérer les tâches/utilisateurs et stocker les métadonnées dans MongoDB.  
- **Exemple** : Ajouter des notifications par email pour la complétion des tâches.  

### Meilleures Pratiques pour le Portfolio
- **Git** : Commits par fonctionnalité (par exemple, `feature/crud`, `feature/upload`), branches claires.  
- **Documentation** : README avec description, configuration, endpoints, déploiement et captures d’écran.  
- **Publication** : Héberger sur GitHub avec une licence open-source (par exemple, MIT).  

### Ressources
- [GitHub Guides](https://guides.github.com)  
- [Spring Boot Official Docs](https://spring.io/projects/spring-boot)  
- [Baeldung – Spring Boot Tutorials](https://www.baeldung.com)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [Docker Official Docs](https://docs.docker.com)  
- [Railway Documentation](https://docs.railway.app)  
- [Heroku Dev Center](https://devcenter.heroku.com)  
- [AWS Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk)  
- [SendGrid API Docs](https://docs.sendgrid.com)  
- [Awesome Open Source](https://awesomeopensource.com)  
- [Practical MongoDB Aggregations](https://university.mongodb.com/courses/MongoDB-Aggregations)