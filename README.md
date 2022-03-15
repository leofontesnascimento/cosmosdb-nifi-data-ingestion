# cosmosdb-nifi-data-ingestion
This simple Proof Of Concept (POC) aims to validate an integration between Azure CosmosDB and Apache NiFi into a Data Ingestion. Have fun!

## Setup Environment

Open your console and enter in project directory (The local where you have been cloned the repository `cosmosdb-nifi-data-ingestion`)

1. Enter in nifi directory
```
cd  nifi/
```
2. Create the docker network
```
make network-create NETWORK=poc 
```
3. Setup the NiFi docker service
```
make build start 
```
4. Enter in cosmos directory
```
cd ../cosmos/
```
5. Setup the NiFi docker service
```
make build start 
```
6. Check if all services has been executed successfully
```
docker ps 
```

## Access Services

### Cosmos DB
```
https://localhost:8081/_explorer/index.html
```

### Apache NiFi
```
http://localhost:8443/nifi
```