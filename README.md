# agent-api

AAFC DINA agent module implementation.

See DINA agent module [specification](https://github.com/DINA-Web/agent-specs).


## Documentation

To generate the complete documentation:
```
mvn clean compile
```

The single HTML page will be available at `target/generated-docs/index.html`

## To Run

For testing purpose or local development a [Docker Compose](https://docs.docker.com/compose/) and `.env` file are available in the `local` folder.

Create a new `docker-compose` and `.env` file from the example:
```
cp local/docker-compose.yml.example docker-compose.yml
cp local/*.env .
```

Start the app (default port is 8082):
```
docker-compose up --build
```

Once the services have started you can access the endpoints at http://localhost:8082/api/v1/agent

Cleanup:
```
docker-compose down
```
