# NET6-MicroServices
There is a couple of microservices which implemented e-commerce modules over Catalog, Basket, Discount and Ordering microservices with NoSQL (MongoDB, Redis) and Relational databases (PostgreSQL, Sql Server) with communicating over RabbitMQ Event Driven Communication and using Ocelot API Gateway.

## Catalog API
### MongoDB
Instructions:
docker pull mongo
docker run -d -p 27017:27017 --name shopping-mongo mongo

To see logs in this container:
docker logs -f shopping-mongo

To access inside the container through interactive terminal (it):
docker exec -it shopping-mongo /bin/bash

we execute the following:
mongo
show dbs
use CatalogDb
db.createCollection('Products')

after that execute (mongo+commands.txt)


