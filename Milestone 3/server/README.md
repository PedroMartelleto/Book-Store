# Book-Store:  Server

## Build Procedures
To install all dependencies for the server, execute:

```
sudo apt-get install nodejs npm mongodb-org
npm install
```

To run the server locally, execute:
```
npm run start
```
## Admin account

To test the admin account, use the following credentials:

```
admin@email.com
admin
```

## Running the Database
If you want to run the database locally (this is NOT required to test the server, since there is a remote database available), run the following commands to install all dependencies:

```
wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
sudo apt-get update
python3 -m pip install pandas tqdm
```

To start the database, execute:
```
sudo systemctl start mongod
```

## Adding books to the local database

To populate the database with the data from the csv file, execute:
```
python3 feedDatabase.py
```
