# Phase 5 – Architecture et Concurrence (2–3 mois)

### Clean Code et Principes SOLID
- **Clean Code** : Nommage clair, fonctions courtes, commentaires utiles, formatage cohérent.  
- **SOLID** :  
  - SRP (Single Responsibility Principle)  
  - OCP (Open/Closed Principle)  
  - LSP (Liskov Substitution Principle)  
  - ISP (Interface Segregation Principle)  
  - DIP (Dependency Inversion Principle)  

**Exemple** : Refactoriser un service du Gestionnaire de Tâches pour respecter les principes SOLID.  

### Design Patterns
- **Patterns** : Factory (création), Singleton (instance unique), Builder (construction d’objets), Strategy (comportement), Observer (événements).  
- **Application** : Choisir des patterns adaptés au contexte du projet.  

**Exemple** : Utiliser Strategy pour différents algorithmes de priorisation des tâches.  

### Threads et Concurrence
- **Concepts** : Thread, Runnable, ExecutorService, ForkJoinPool.  
- **Techniques** : Créer et gérer des pools de threads, tâches asynchrones.  

**Exemple** : Traiter les rapports de tâches en parallèle avec ExecutorService.  

### Synchronisation et Problèmes de Concurrence
- **Mécanismes** : `synchronized`, `Lock`, `ReentrantLock`, `ConcurrentHashMap`.  
- **Problèmes** : Deadlock, race condition, starvation.  

**Exemple** : Implémenter un accès sécurisé à une liste de tâches partagée.  

### Introduction aux Microservices
- **Concepts** : Architecture de microservices, communication REST, découverte de services.  
- **Outils** : Spring Cloud (par exemple, Eureka pour la découverte de services).  

**Exemple** : Diviser le Gestionnaire de Tâches en microservices (tâches et utilisateurs).  

### Fondamentaux des Files de Messages (Optionnel)
- **Concepts** : Publisher/subscriber, queues, topics.  
- **RabbitMQ** : Configuration, envoi et consommation de messages.  

**Exemple** : Notifier les utilisateurs des mises à jour des tâches via RabbitMQ.  

### Optimisation des Performances
- **Caching** : Spring Cache avec Redis pour réduire les accès à la base de données.  
- **JVM Tuning** : Concepts de base (heap, garbage collection).  

**Exemple** : Implémenter un cache pour les requêtes fréquentes dans le système de tâches.  

### Introduction à DevOps/Cloud : Docker et CI/CD
- **Docker** : Conteneurs, images, Dockerfile, Docker Compose.  
- **CI/CD** : Configurer des pipelines avec GitHub Actions pour la construction et le déploiement.  

**Exemple** : Créer un Dockerfile pour l’application de tâches et déployer via GitHub Actions.  

### Observabilité
- **Outils** : Prometheus (métriques), Grafana (visualisation), ELK Stack (logs).  
- **Concepts** : Surveillance des performances, logs centralisés, alertes.  

**Exemple** : Surveiller le temps de réponse de l’API des tâches avec Prometheus et Grafana.  

### Sécurité : OWASP Top Ten
- **Concepts** : Injection, échecs d’authentification, exposition de données sensibles.  
- **Pratiques** : Validation des entrées, sanitisation, configuration sécurisée.  

**Exemple** : Protéger l’API des tâches contre les injections SQL et XSS.  

### Projet Final
**Système Avancé de Gestion de Tâches**  
- Backend : Améliorer l’API des tâches (Phase 4) avec des microservices (tâches et utilisateurs).  
- Architecture : Refactoriser avec Clean Code, SOLID et design patterns (par exemple, Strategy).  
- Concurrence : Traiter les rapports en parallèle avec ExecutorService.  
- **Optionnel** : Ajouter une communication entre microservices via RabbitMQ et un caching avec Redis pour les requêtes fréquentes.  
- DevOps : Empaqueter en Docker, configurer CI/CD avec GitHub Actions.  
- Observabilité : Ajouter Prometheus et Grafana pour les métriques.  
- Sécurité : Implémenter des protections contre les OWASP Top Ten.  
- Git : Commits par fonctionnalité (par exemple, `feature/microservices`, `feature/concurrency`).  
- Publier : Sur GitHub avec un README détaillé (configuration, architecture, déploiement).  

### Ressources
- *The Pragmatic Programmer* (Livre)  
- *Effective Java* (Livre)  
- *Java Concurrency in Practice* (Livre)  
- [Spring Cloud Documentation](https://spring.io/projects/spring-cloud)  
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)  
- [Redis University](https://university.redis.com/)  
- [Docker Official Docs](https://docs.docker.com/)  
- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)  
- [Grafana Documentation](https://grafana.com/docs/)  
- [ELK Stack Guide](https://www.elastic.co/what-is/elk-stack)  
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)  
- [GitHub Actions Documentation](https://docs.github.com/en/actions)  