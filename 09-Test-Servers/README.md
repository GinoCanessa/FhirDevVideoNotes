# Server Testing

This set of videos covers setting up various FHIR servers for testing.

## Azure FHIR Server

* Video
  * [Local Test Server - Azure](https://youtu.be/o7mBoNGO-WY)
* Links
  * [GitHub](https://github.com/microsoft/fhir-server/tree/main/samples/docker)
  * [Docker Hub](https://hub.docker.com/_/microsoft-healthcareapis-r4-fhir-server)
* Commands (don't forget to set the password!)
  * `docker network create fhir_network`
  * `docker run --net fhir_network --name fhir_sql -e SA_PASSWORD=<SA_PASSWORD> -e ACCEPT_EULA="Y" -d mcr.microsoft.com/mssql/server`
  * `docker run --net fhir_network -e FhirServer__Security__Enabled="false" -e SqlServer__ConnectionString="Server=tcp:fhir_sql,1433;Initial Catalog=FHIR;Persist Security Info=False;User ID=sa;Password=<SA_PASSWORD>;MultipleActiveResultSets=False;Connection Timeout=30;" -e SqlServer__AllowDatabaseCreation="true" -e SqlServer__Initialize="true" -e SqlServer__SchemaOptions__AutomaticUpdatesEnabled="true" -e DataStore="SqlServer" -p 8080:8080 -d mcr.microsoft.com/healthcareapis/r4-fhir-server azure-fhir-api`
* Default Endpoint (R4):
  * http://localhost:8080/

## HAPI FHIR Server

* Video
  * [Local Test Server - HAPI](https://youtu.be/EaJpJ0aQjiM)
* Links
  * [GitHub](https://github.com/hapifhir/hapi-fhir-jpaserver-starter)
  * [Docker Hub](https://hub.docker.com/r/hapiproject/hapi)
* Commands
  * `docker run -p 8080:8080 hapiproject/hapi:latest`
* Default Endpoint (R4):
  * http://localhost:8080/fhir/

## IBM FHIR Server

* Video
  * [Local Test Server - IBM](https://youtu.be/eirDH6BPD3g)
* Links
  * [GitHub](https://github.com/IBM/FHIR)
  * [Docker Hub](https://hub.docker.com/r/ibmcom/ibm-fhir-server)
* Commands
  * `docker run -p 9443:9443 -e BOOTSTRAP_DB=true ibmcom/ibm-fhir-server`
* Default Endpoint (R4):
  * https://localhost:9443/fhir-server/api/v4

## Spark FHIR Server

* Video
  * [Local Test Server - Spark](https://youtu.be/lQGOgQHfDJc)
* Links
  * [GitHub](https://github.com/FirelyTeam/spark)
* Commands
  * `curl 'https://raw.githubusercontent.com/FirelyTeam/spark/r4/master/.docker/docker-compose.example.yml' > docker-compose.yml`
  * `docker compose up`
* Default Endpoint (R4):
  * https://localhost:5555/fhir

