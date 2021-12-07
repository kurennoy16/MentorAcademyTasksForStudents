# Microservices simple task

Create 2 services ‘Client-api’ and ‘domain service’. 

## DOMAIN SERVICE
You need to create domain service. It should allocate any port (on your decision) and have 2 endpoints:
1. List all ports
2. Upsert ports (if port doesn’t exist - create, if exists - update)
Ports should be stored in Postgres DB.


## CLIENT-API SERVICE
You need to create client api service. It should provide the ability to upload json file and send ports to domain-service.
You need to create 2 endpoints:
1. List ports
2. Upload ‘ports.json’ and make appropriate calls to the domain.

### REQUIREMENTS:
* Provide Docker file for each service.
* Provide the ability to config your services via Env vars or config file.
* Description how to run your services in Readme.md 

### BONUS POINTS:
* Docker-compose file
* Ability to filter ports by id and name
* Unit tests
* N2n tests
* gRPC protocol for domain service
* Use golangci lint

