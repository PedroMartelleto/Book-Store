# Book-Store:  Server

## Build Procedures
To install all dependencies of the server and the database, execute:
```
wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
sudo apt-get update
sudo apt-get install nodejs npm mongodb-org
npm install

```

To start the database, execute:
```
sudo systemctl start mongod
```

To populate the database with the data from the csv file, execute:
```
python3 feedDatabase.py
```

To run the server locally, in the same machine as a running database, execute:
```
MONGO_URL="mongodb://127.0.0.1" PORT=3333 PWD_SECRET_KEY="test-secret-key" JWD_SECRET_KEY="test-jwd-secret-key" npm run start
```

To execute the automated tests while a server and a database are running, execute:

```
npm run test
```