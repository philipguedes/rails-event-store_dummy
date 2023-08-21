# Rails Event Store - Dummy App

### Build the image

```bash
docker build -t res-dummy -f Dockerfile.dev --no-cache --build-arg USER=$USER --build-arg UID=$UID .
```

### Run image

```bash
docker-compose up
```

### Create database

```bash
docker-compose exec api rails db:create
```

### Run migration

```bash
docker-compose exec api rails generate rails_event_store_active_record:migration --data-type=jsonb
```