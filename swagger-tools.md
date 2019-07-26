
Use the following docker calls to work on API

run the editor:

docker run -d -p 1280:8080 swaggerapi/swagger-editor:v3.6.31

call to generate code.

docker run -it  --user `id -u $USER` -v /home/sage/git/k8beltester:/data openapitools/openapi-generator-cli:v4.0.3 generate -i /data/openapi.json -g go -o /data/src 
