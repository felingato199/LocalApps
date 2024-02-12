# Configurtation of Local third Apps
## List of  confilist Apps
- Listcore
- MainAppBackend
- MainAppFronted


## OS variables config
Create a file for each config in path configs
### Listcore
```
DEBUG="false"
ALLOWED_HOSTS='["10.0.2.15", "web"]'
CSRF_TRUSTED_ORIGINS='["http://10.0.2.15:8090", "http://web"]'
webhookactualizador='http://110.0.2.15:8008/webhook'
DB_ENGINE=django.db.backends.postgresql
DB_NAME=
DB_USER=
DB_PASSWORD=
DB_HOST=
DB_PORT=
TOKEN=
webhookmasivo=
MONGODB=
DATABASE='list_core'
CELERY_BROKER_URL=
```
### MainAppBackend
```
MONGO_URI=
MONGO_CORE_URI=
DATABASE=
JWT_ACCESS_TOKEN_EXPIRES=
JWT_SECRET_KEY=b9af1c569765df83702b87f0766ea84e4182b7cd
JWT_REFRESH_TOKEN_EXPIRES=
REDIS_URI=
LIST_KERNEL_URI=
EMAIL_USER=
EMAIL_PASSWORD=
EMAIL_HOST=
EMAIL_PORT=
HASHCODE=sdflkjjs457d
BROKER=
BROKER_CONNECTION_RETRY_ON_STARTUP='true'
RESULT_PERSISTENT='true'
ENABLE_UTC='true'
RESULT_BACKEND=
CONFILIST_URL=http://192.168.0.103:8091
USER_EMAIL=
USER_PASSWORD=
SYSTEM_EMAIL=
```
### MainAppFronted
```

```

## Volumes
### Listcore
No need 
### MainAppBackend
list_core_pg_data
No need


## Network
confilist_apps_network
```
docker network create confilist_apps_network
```

# Note: No use the default .envs files, only are examples, each information file is very easy to hack.

## Deploy:
- in path docker deploy execute:  
```
docker compose up -d
```
- check all good:
```
docker compose ps
```

