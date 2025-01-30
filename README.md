# DCAT-validator
DCAT Validator
Full documentation: https://www.itb.ec.europa.eu/docs/guides/latest/validatingRDF/index.html



Deploying this DCAT-validator will allow to validate RDF against HealthDCAT-AP SHACL file.

Installation using docker compose :

Copy content of validator and docker-compose.yml file to desire location

docker compose up -d




Installation using docker :

Copy content of validator to desire location (docker-compose.yml not needed)

cd ./validator

docker build -t dcat-validator .

docker run -d --name dcat-validator -p 8080:8080 dcat-validator:latest



Access the DCAT-validator :

WebInterface : http://LOCALSERVERIP:8080/shacl/dcat/upload

Swagger interface :  http://LOCALSERVERIP:8080/shacl/swagger-ui.html
