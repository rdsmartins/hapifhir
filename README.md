# HAPI-FHIR Images  #

### docker pull mimi50/hapifhir ###


## RUN: ##

#### run hapi-fhir exposing port: ####
> docker run --name hapi  -p 8080:8080 mimi50/hapifhir

#### To persist the data: ####
> docker run --name hapi  -p 8080:8080 -v /your/host/hapi/directory:/opt/hapi-fhir/target mimi50/hapifhir

#### To enter the image shell: ####
> docker exec -it  hapi /bin/bash

#### To stop the image: ####
> docker stop hapi

#### To view the Hapi Fhir web admin ####
> http://0.0.0.0:8080

#### Example: ####
> docker run --name hapi -p 8080:8080 -v /home/vagrant/docker/hapi/2.4:/opt/hapi-fhir/target mimi50/hapifhir
