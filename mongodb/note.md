
# Server Operations
## Commands for server start/stop
```
# Start server
sudo service mongod start

# Start server (blocking)
sudo mongod --directoryperdb --dbpath ~/dev/mongodb/data/db --logpath ~/dev/mongodb/log/mongo.log --logappend

# Check the mondbd process has started successfully
cat /var/log/mongodb/mongod.log | grep "initandlisten"

# Stop server
sudo service mongod stop

# Restart server
sudo service mongod restart

# Start mongo shell
mongo --host 127.0.0.1:27017
```

## Configuration
```
# Config path for mongod
/etc/mongod.conf
```

# Database Operations
## Admin
```
# Create an admin user
db.createUser({
  user: "username",
  pwd: "password",
  roles: ["readWrite", "dbAdmin"]
  });
```

## Database-level
```
# List all Databases
show dbs

# (Create and) use a Database
use helloworld

# See current db
db
```
