# Rails Event Store - Dummy App

This repo was created to help reproduce [issue #1650](https://github.com/RailsEventStore/rails_event_store/issues/1650)

## Steps to reproduce

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