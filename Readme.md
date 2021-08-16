# SQL / Docker Debug Environment

# Installation
Clone the repo
```bash
git clone https://github.com/ransbachm/mysql_env/
cd mysql_env
```

# Startup
Start with

```bash
docker-compose up
```

Or in detached mode

```bash
docker-compose up -d
```
# Usage

If started you can use

[Portainer (Port 9000)](http://localhost:9000) \
[Php Myadmin (Port 8080)](http://localhost:8080)

Or get a SQL shell in the container

```
docker exec -it mysql_env_debug-mysql_1 mysql -p
```

Or a SQL shell in the host (must have mysql / mariadb client installed)

```bash
mysql -p -u mysql_env_debug-mysql_1
```
