# swaggerelasticbeanstalk
Dockerized Swagger Codegen and Swagger Editor for AWS Elastic Beanstalk 

Runs on AWS Elastic Beanstalk

2 Docker images pulled from Docker Hub for Swagger

"swaggerapi/swagger-editor:latest" for Editor UI --> accessible on port 80 on the load balanced URL

"swaggerapi/swagger-generator:latest" for server and client side code generator --> accessible on port 80 on the load balanced URL

".ebextensions/elb-listeners-setting.json" --> CFN to have ELB settings. 

Important --> Update the defaults.orig.json to configure the actual url of your elastic load balanced application and save it as default.json.
