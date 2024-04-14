# 📦 GLPI Docker Environment

Ce repository contient tout le nécessaire pour déployer l'application GLPI avec MariaDB en utilisant Docker et Docker Compose.

## 🚀 Démarrage rapide

Pour lancer ce projet, suivez ces étapes :

### Prérequis

-   Docker
-   Docker Compose
-   Git (optionnel, recommandé pour le clonage du repository)

### 📥 Clonage du Repository

Pour obtenir le projet, exécutez cette commande dans votre terminal :

```
git clone Mickael-Salmon/glpi
```

### 📝 Configuration

1.  **Fichier .env pour MariaDB**:
    -   Dupliquez le fichier `mariadb.env.example` et renommez-le en `mariadb.env`.
    -   Modifiez les variables d'environnement dans `mariadb.env` pour correspondre à votre configuration.

### 🏗 Construction de l'Image Docker (si nécessaire)

Si vous devez reconstruire l'image Docker pour GLPI :

```
docker build -t mickaelsalmon/glpi .
```

### 🚢 Lancement des Conteneurs

Pour démarrer les conteneurs :

```
docker-compose up -d
```

### 🌐 Accéder à GLPI

Une fois les conteneurs lancés, vous pouvez accéder à GLPI en ouvrant votre navigateur à l'adresse http://localhost ou https://localhost pour HTTPS.

## ⚙️ Maintenance

### Mises à jour

Pour mettre à jour votre copie locale avec la dernière version du repository :

```
git pull origin main
```

### 🛠 Dépannage

Si vous rencontrez des problèmes, vérifiez les logs des conteneurs Docker :

```
docker logs nom_du_conteneur_glpi
```