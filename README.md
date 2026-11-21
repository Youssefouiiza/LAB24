# TP 24 : Conteneurisation Spring Angular

Application Smart Home conteneurisée avec Docker : backend Spring Boot + MySQL, frontend Angular servi par Nginx, et phpMyAdmin, orchestrés avec `docker-compose`.

```bash
cd smarthouse
docker-compose build
docker-compose up -d
docker-compose ps
```

## 1. Images Docker

![Images Docker](smarthouse/screenshots/1-docker-images.png)

Les images `smarthouse-frontend` et `smarthouse-backend` construites avec `docker-compose build`, ainsi que `mysql` et `phpmyadmin`, sont disponibles dans Docker Desktop et utilisées par les conteneurs en cours d'exécution.

## 2. Application frontend sur http://localhost

![Frontend Angular](smarthouse/screenshots/2-frontend-localhost.png)

L'application Angular servie par Nginx affiche les appareils récupérés depuis le backend Spring Boot.

## 3. phpMyAdmin sur http://localhost:8081

![phpMyAdmin](smarthouse/screenshots/3-phpmyadmin-8081.png)

phpMyAdmin montre la base `smart-house` avec les tables `appareil` et `categorie` créées par le backend et remplies avec les données de l'application.
