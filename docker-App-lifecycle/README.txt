In this directory: 
'docker-compose.yml' is base file for docker-compose up, and if the file with name name 'docker-compose.override.yml' exists, {docker-compose up} command will pick up this override file automatically to set up the rest of the environment.

using `docker-compose -f <base yml file> -f <prod yml file> config` can generate an official yml file to be used in actual production environment.  and this can be output to a yml file from CI pipeline tool like jenkins.

In our case, 'offical.prod.yml' is such automatically generated file with combined parameters can be used in production.