# DCAT-validator
DCAT Validator

Source: https://www.itb.ec.europa.eu/docs/guides/latest/validatingRDF/index.html

Place the files keeping the structure at root.

cd /validator

docker build -t dcat-validator .

docker run -d --name dcat-validator -p 8080:8080 dcat-validator:latest

Access the page at : http://LOCALSERVERIP:8080/shacl/dcat/upload
