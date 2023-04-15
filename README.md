Using CLi for Persistent Volume

1) Mongo-DB
docker run --name mongodb -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=password -v myvol/data/db --network mynet -d mongo

2) Mongo-express
docker run --name express1 -p 8081:8081 -e ME_CONFIG_MONGODB_ADMINUSERNAME=admin -e ME_CONFIG_MONGODB_ADMINPASSWORD=password -e ME_CONFIG_MONGODB_SERVER=mongodb --network mynet --restart=always  mongo-express

Using Docker-Compose :

Attached the file in repo 
