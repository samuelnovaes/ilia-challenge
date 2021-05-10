# ilia-challenge

## How to run

```
git clone https://github.com/samuelnovaes/ilia-challenge.git
git submodule init
git submodule update
docker-compose up -d
```

## API endpoints

- `http://localhost:3001` - Wallet micro-service
- `http://localhost:3002` - User micro-service

## Env var
Each micro-service needs the following environment variables
```
PORT
MONGO_URL
PRIVATE_KEY
KAFKA_BROKER
```
Example
```
PORT=3002
MONGO_URL=mongodb://root:ILIACHALLENGE@172.16.0.3:27018/iliachallenge
PRIVATE_KEY=ILIACHALLENGE
KAFKA_BROKER=172.16.0.8:9092
```
These variables can be defined in the docker-compose file

## Insomnia workspace
You can import the project workspace in Insomnia from the `insomnia.json` file. 