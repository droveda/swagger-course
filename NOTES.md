# Swagger Course

## Basico
* https://swagger.io/
* https://swagger.io/resources/open-api/
* https://www.openapis.org/
* https://mockapi.io/

## Running swagger editor locally using docker
* https://github.com/swagger-api/swagger-editor
* docker pull swaggerapi/swagger-editor
* docker run -d -p 80:8080 swaggerapi/swagger-editor
* docker run -d -p 80:8080 -v $(pwd):/tmp -e SWAGGER_FILE=/tmp/my_api.yml swaggerapi/swagger-editor
* docker run -d -p 80:8080 -e URL=/foo/swagger.json -v /bar:/usr/share/nginx/html/foo swaggerapi/swagger-editor

## Using Swagger UI
* https://github.com/swagger-api/swagger-ui
* docker pull swaggerapi/swagger-ui
* docker run -p 80:8080 swaggerapi/swagger-ui
* docker run -p 80:8080 -e SWAGGER_JSON=/foo/swagger.json -v /bar:/foo swaggerapi/swagger-ui
