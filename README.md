# WordPress Docker Project


This repository provides a simple and reproducible Docker-based setup to run a WordPress website with a MariaDB database.

### Prerequisites

- Docker & Docker Compose installed

## Table of Contents

- [Quickstart](#quickstart)
- [Usage](#usage)


## Quickstart

1. Clone the repository:
```bash
git clone https://github.com/Bodev13/wordpress.git
cd wordpress
````
2. Create and set up .env file
3. Build and start the Wordpress server container:

```bash
docker-compose up --build
```
4. Visit the wordpress locally:

```bash
http://localhost:8080
````
5. On your cloud vm:
```bash
http://your_cloud_vm:8080
````
6. Stop the containers:
```bash
docker-compose down -v
```


## Usage

his will get the app running in a Docker container on your local machine and on the V-Server.

### Set the environment variables:

```bash
WORDPRESS_PORT=8080
ALLOWED_HOSTS=your_cloud_vm_ip,localhost,127.0.0.1,0.0.0.0

WORDPRESS_DB_NAME=wordpress
WORDPRESS_DB_USER=wpuser
WORDPRESS_DB_PASSWORD=wppassword!

MYSQL_DATABASE=wordpress
MYSQL_USER=wpuser
MYSQL_PASSWORD=wppassword!
MYSQL_ROOT_PASSWORD=rootpass
```
### Build and start the Wordpress server container:

```bash
docker-compose up --build
```

### Access the Wordpress website:
```bash
https://your_cloud_vm:8080
````
